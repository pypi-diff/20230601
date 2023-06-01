# Comparing `tmp/bittensor-5.0.0.tar.gz` & `tmp/bittensor-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-5.0.0.tar", last modified: Thu May 18 16:44:04 2023, max compression
+gzip compressed data, was "bittensor-5.1.0.tar", last modified: Thu Jun  1 21:17:45 2023, max compression
```

## Comparing `bittensor-5.0.0.tar` & `bittensor-5.1.0.tar`

### file list

```diff
@@ -1,115 +1,124 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.288592 bittensor-5.0.0/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1087 2022-07-09 15:48:08.000000 bittensor-5.0.0/LICENSE
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4395 2023-05-18 16:44:04.288592 bittensor-5.0.0/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3369 2023-05-18 16:31:28.000000 bittensor-5.0.0/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bin/
--rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1297 2022-10-11 20:24:30.000000 bittensor-5.0.0/bin/btcli
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15485 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor/_axon/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18031 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_axon/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_cli/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6777 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3879 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/cli_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_cli/commands/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      613 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    24917 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7512 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3900 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/list.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7371 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6968 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    16312 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7542 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/register.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10946 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4312 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11043 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7699 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17524 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_cli/commands/wallets.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_config/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5981 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_config/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5896 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_config/config_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dataset/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10949 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26660 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5443 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3581 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dataset/thread_queue.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dendrite/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10128 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/dendrite.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_dendrite/text_prompting/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10806 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5215 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite_pool.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_ipfs/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2890 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_ipfs/ipfs_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_keyfile/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1885 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    22206 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_keyfile/keyfile_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_logging/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13062 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_logging/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_metagraph/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    12792 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_metagraph/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_prometheus/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8080 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_prometheus/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_proto/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/_proto/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37015 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6201 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_proto/bittensor_pb2_grpc.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_serializer/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6062 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_serializer/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10739 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_serializer/serializer_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_subtensor/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13432 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    25954 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2344 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/errors.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1119 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17093 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26886 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6020 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14263 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10108 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6376 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18378 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7537 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15505 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    45395 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18999 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_subtensor/subtensor_mock.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_synapse/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6713 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/synapse.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_synapse/text_prompting/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10680 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/miner.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7260 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_synapse/text_prompting/synapse.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_threadpool/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4477 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8594 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_tokenizer/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2485 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_tokenizer/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.284592 bittensor-5.0.0/bittensor/_wallet/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6891 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    41320 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2286 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/_wallet/wallet_mock.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.288592 bittensor-5.0.0/bittensor/utils/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8536 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3443 2023-04-20 18:56:12.000000 bittensor-5.0.0/bittensor/utils/_register_cuda.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8699 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/balance.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4445 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/codes.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      518 2023-04-20 18:56:12.000000 bittensor-5.0.0/bittensor/utils/formatting.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7999 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/networking.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    35796 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/registration.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    32876 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3351 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/stats.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      630 2022-07-09 15:48:08.000000 bittensor-5.0.0/bittensor/utils/test_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    75481 2023-03-23 20:47:08.000000 bittensor-5.0.0/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9929 2023-05-18 16:31:28.000000 bittensor-5.0.0/bittensor/utils/weight_utils.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:44:04.280592 bittensor-5.0.0/bittensor.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4395 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2970 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1044 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-05-18 16:44:04.000000 bittensor-5.0.0/bittensor.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-18 16:44:04.288592 bittensor-5.0.0/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3429 2023-05-18 16:31:28.000000 bittensor-5.0.0/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.724586 bittensor-5.1.0/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1087 2022-07-09 15:48:08.000000 bittensor-5.1.0/LICENSE
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    22530 2023-06-01 21:17:45.724586 bittensor-5.1.0/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    21504 2023-06-01 17:36:43.000000 bittensor-5.1.0/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bin/
+-rwxrwxr-x   0 eduardo   (1000) eduardo   (1000)     1297 2022-10-11 20:24:30.000000 bittensor-5.1.0/bin/btcli
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15787 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor/_axon/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18273 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_axon/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor/_blacklist/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4759 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_blacklist/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor/_cli/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6777 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3879 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/cli_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor/_cli/commands/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      613 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    24509 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7970 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3900 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7371 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6968 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    16284 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7397 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10904 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4285 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11000 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7687 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17326 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_cli/commands/wallets.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_config/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7537 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_config/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8101 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_config/config_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_dataset/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11193 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26660 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5443 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3581 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dataset/thread_queue.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_dendrite/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dendrite/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10240 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_dendrite/dendrite.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_dendrite/text_prompting/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dendrite/text_prompting/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10806 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5215 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_ipfs/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.1.0/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2890 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_ipfs/ipfs_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_keyfile/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1885 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    22206 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_keyfile/keyfile_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_logging/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13306 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_logging/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_metagraph/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    12893 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_metagraph/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_neuron/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_neuron/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5752 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_neuron/base_huggingface_miner.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9731 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_neuron/base_miner_neuron.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3186 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_neuron/base_prompting_miner.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6986 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_neuron/base_validator.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_priority/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3529 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_priority/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_prometheus/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8330 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_prometheus/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_proto/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-07-09 15:48:08.000000 bittensor-5.1.0/bittensor/_proto/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    37015 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6201 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_proto/bittensor_pb2_grpc.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_serializer/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6062 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10739 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_serializer/serializer_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_subtensor/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    13661 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    25954 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2344 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/errors.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1119 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    17093 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    26886 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6020 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    14263 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10108 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6376 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18378 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7537 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    15505 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    45582 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    18999 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_subtensor/subtensor_mock.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_synapse/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_synapse/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6713 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_synapse/synapse.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_synapse/text_prompting/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_synapse/text_prompting/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7270 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_synapse/text_prompting/synapse.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_threadpool/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4723 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8594 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_tokenizer/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2485 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_tokenizer/__init__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.720586 bittensor-5.1.0/bittensor/_wallet/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7105 2023-06-01 21:04:08.000000 bittensor-5.1.0/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    41320 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2286 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/_wallet/wallet_mock.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.724586 bittensor-5.1.0/bittensor/utils/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8536 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3443 2023-04-20 18:56:12.000000 bittensor-5.1.0/bittensor/utils/_register_cuda.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     8699 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/balance.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4445 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/codes.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      518 2023-04-20 18:56:12.000000 bittensor-5.1.0/bittensor/utils/formatting.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7999 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/networking.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    35796 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/registration.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    32876 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3351 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/stats.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      630 2022-07-09 15:48:08.000000 bittensor-5.1.0/bittensor/utils/test_utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    75481 2023-03-23 20:47:08.000000 bittensor-5.1.0/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9929 2023-05-18 16:31:28.000000 bittensor-5.1.0/bittensor/utils/weight_utils.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-01 21:17:45.716586 bittensor-5.1.0/bittensor.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    22530 2023-06-01 21:17:45.000000 bittensor-5.1.0/bittensor.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3183 2023-06-01 21:17:45.000000 bittensor-5.1.0/bittensor.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-01 21:17:45.000000 bittensor-5.1.0/bittensor.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1044 2023-06-01 21:17:45.000000 bittensor-5.1.0/bittensor.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       10 2023-06-01 21:17:45.000000 bittensor-5.1.0/bittensor.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-06-01 21:17:45.724586 bittensor-5.1.0/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     3429 2023-05-18 16:31:28.000000 bittensor-5.1.0/setup.py
```

### Comparing `bittensor-5.0.0/LICENSE` & `bittensor-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bin/btcli` & `bittensor-5.1.0/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/__init__.py` & `bittensor-5.1.0/bittensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from langchain.llms.base import LLM
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '5.0.0'
+__version__ = '5.1.0'
 version_split = __version__.split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
@@ -164,14 +164,16 @@
 from bittensor._metagraph import metagraph as metagraph
 from bittensor._prometheus import prometheus as prometheus
 from bittensor._subtensor import subtensor as subtensor
 from bittensor._tokenizer import tokenizer as tokenizer
 from bittensor._serializer import serializer as serializer
 from bittensor._dataset import dataset as dataset
 from bittensor._threadpool import prioritythreadpool as prioritythreadpool
+from bittensor._blacklist import blacklist  as blacklist
+from bittensor._priority import priority as priority
 
 # ---- Classes -----
 from bittensor._cli.cli_impl import CLI as CLI
 from bittensor._config.config_impl import Config as Config
 from bittensor._subtensor.chain_data import DelegateInfo as DelegateInfo
 from bittensor._wallet.wallet_impl import Wallet as Wallet
 from bittensor._keyfile.keyfile_impl import Keyfile as Keyfile
@@ -203,15 +205,18 @@
 # ---- Dendrites -----
 from bittensor._dendrite.dendrite import Dendrite
 from bittensor._dendrite.dendrite import DendriteCall
 from bittensor._dendrite.text_prompting.dendrite import TextPromptingDendrite as text_prompting
 from bittensor._dendrite.text_prompting.dendrite_pool import TextPromptingDendritePool as text_prompting_pool
 
 # ---- Base Miners -----
-from bittensor._synapse.text_prompting.miner import BasePromptingMiner
+from bittensor._neuron.base_miner_neuron import BaseMinerNeuron
+from bittensor._neuron.base_validator import BaseValidator
+from bittensor._neuron.base_prompting_miner import BasePromptingMiner
+from bittensor._neuron.base_huggingface_miner import HuggingFaceMiner
 
 # ---- Errors and Exceptions -----
 from bittensor._keyfile.keyfile_impl import KeyFileError as KeyFileError
 
 # ---- Errors and Exceptions -----
 from bittensor._keyfile.keyfile_impl import KeyFileError as KeyFileError
```

### Comparing `bittensor-5.0.0/bittensor/_axon/__init__.py` & `bittensor-5.1.0/bittensor/_axon/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             placeholder1 = 0,
             placeholder2 = 0,
         )
 
     def __init__(
         self,
         wallet: "bittensor.Wallet",
-        metagraph: "bittensor.Metagraph",
+        metagraph: Optional["bittensor.Metagraph"] = None,
         config: Optional["bittensor.config"] = None,
         port: Optional[int] = None,
         ip: Optional[str] = None,
         external_ip: Optional[str] = None,
         external_port: Optional[int] = None,
         max_workers: Optional[int] = None,
         server: "grpc._server._Server" = None,
@@ -155,14 +155,19 @@
         print(cls.__new__.__doc__)
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None):
         """Accept specific arguments from parser"""
         prefix_str = "" if prefix is None else prefix + "."
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).axon = bittensor.defaults.axon
+
         bittensor.prioritythreadpool.add_args(parser, prefix=prefix_str + "axon")
         try:
             parser.add_argument(
                 "--" + prefix_str + "axon.port",
                 type=int,
                 help="""The local port this axon endpoint is bound to. i.e. 8091""",
                 default=bittensor.defaults.axon.port,
@@ -286,29 +291,29 @@
         """
         super().__init__()
         self.nonces = {}
         self.blacklist = blacklist
         self.receiver_hotkey = receiver_hotkey
 
 
-    def parse_signature_v2(self, signature: str) -> Union[Tuple[int, str, str, str, int], None]:
+    def parse_signature_v2(self, signature: str) -> Optional[Tuple[int, str, str, str]]:
         r"""Attempts to parse a signature using the v2 format"""
         parts = signature.split(".")
         if len(parts) != 4:
             return None
         try:
             nonce = int(parts[0])
         except ValueError:
             return None
         sender_hotkey = parts[1]
         signature = parts[2]
         receptor_uuid = parts[3]
         return (nonce, sender_hotkey, signature, receptor_uuid)
 
-    def parse_signature(self, metadata: Dict[str, str]) -> Tuple[int, str, str, str, int]:
+    def parse_signature(self, metadata: Dict[str, str]) -> Tuple[int, str, str, str]:
         r"""Attempts to parse a signature from the metadata"""
         signature = metadata.get("bittensor-signature")
         version = metadata.get('bittensor-version')
         if signature is None:
             raise Exception("Request signature missing")
         if int(version) < 370:
             raise Exception("Incorrect Version")
@@ -440,11 +445,11 @@
         r""" Returns a torch tensor of the subnet info.
         """
         return torch.nn.ParameterDict(
             self.__dict__
         )
 
     @classmethod
-    def from_parameter_dict( cls, parameter_dict: 'torch.nn.ParameterDict' ) -> 'SubnetInfo':
-        r""" Returns a SubnetInfo object from a torch parameter_dict.
+    def from_parameter_dict( cls, parameter_dict: 'torch.nn.ParameterDict' ) -> 'axon_info':
+        r""" Returns an axon_info object from a torch parameter_dict.
         """
         return cls( **dict(parameter_dict) )
```

### Comparing `bittensor-5.0.0/bittensor/_cli/__init__.py` & `bittensor-5.1.0/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/cli_impl.py` & `bittensor-5.1.0/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/__init__.py` & `bittensor-5.1.0/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/delegates.py` & `bittensor-5.1.0/bittensor/_cli/commands/delegates.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
             delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
             show_delegates( delegates, prev_delegates = prev_delegates)
             delegate_index = Prompt.ask("Enter delegate index")
             config.delegate_ss58key = str(delegates[int(delegate_index)].hotkey_ss58)
             console.print("Selected: [yellow]{}[/yellow]".format(config.delegate_ss58key))
 
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         # Get amount.
         if not config.get('amount') and not config.get('stake_all'):
             if not Confirm.ask("Stake all Tao from account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to stake")
@@ -277,18 +277,15 @@
             default=False,
         )
         bittensor.wallet.add_args( undelegate_stake_parser )
         bittensor.subtensor.add_args( undelegate_stake_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        # if config.subtensor.get('network') == bittensor.defaults.subtensor.network and not config.no_prompt:
-        #     config.subtensor.network = Prompt.ask("Enter subtensor network", choices=bittensor.__networks__, default = bittensor.defaults.subtensor.network)
-
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if not config.get('delegate_ss58key'):
             # Check for delegates.
             with bittensor.__console__.status(":satellite: Loading delegates..."):
                 subtensor = bittensor.subtensor( config = config )
@@ -406,19 +403,19 @@
             default=False,
         )
         bittensor.wallet.add_args( nominate_parser )
         bittensor.subtensor.add_args( nominate_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
+        if not config.is_set('wallet.hotkey') and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
 
 class MyDelegatesCommand:
 
     @staticmethod
@@ -523,13 +520,13 @@
             default=False,
         )
         bittensor.wallet.add_args( delegate_stake_parser )
         bittensor.subtensor.add_args( delegate_stake_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.get( 'all', d=None ) and not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/inspect.py` & `bittensor-5.1.0/bittensor/_cli/commands/inspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,33 +117,43 @@
                     ''
                 )
 
             hotkeys = _get_hotkey_wallets_for_wallet( wallet )
             for netuid in netuids:
                 for neuron in neuron_state_dict[netuid]:
                     if neuron.coldkey == wallet.coldkeypub.ss58_address:
+                        hotkey_name: str = ''
+
+                        hotkey_names: List[str] = \
+                            [ wallet.hotkey_str for wallet in filter( 
+                                lambda hotkey: hotkey.hotkey.ss58_address == neuron.hotkey,
+                                hotkeys
+                            ) ]
+                        if len(hotkey_names) > 0:
+                            hotkey_name = f'{hotkey_names[0]}-' 
+                        
                         table.add_row(
                             '',
                             '',
                             '',
                             '',
                             '',
                             str( netuid ),
-                            str( neuron.hotkey ),
+                            f'{hotkey_name}{neuron.hotkey}',
                             str( neuron.stake ),
                             str( bittensor.Balance.from_tao(neuron.emission) )
                         )
 
         bittensor.__console__.print(table)
 
 
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if not config.get( 'all', d=None ) and config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.get( 'all', d=None ) and not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         inspect_parser = parser.add_parser(
             'inspect',
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/list.py` & `bittensor-5.1.0/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/metagraph.py` & `bittensor-5.1.0/bittensor/_cli/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/misc.py` & `bittensor-5.1.0/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/overview.py` & `bittensor-5.1.0/bittensor/_cli/commands/overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         )
         overview_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
         bittensor.wallet.add_args( overview_parser )
         bittensor.subtensor.add_args( overview_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt and not config.get( 'all', d=None ):
+        if not config.is_set('wallet.name') and not config.no_prompt and not config.get( 'all', d=None ):
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         if config.netuid != []:
             if not isinstance(config.netuid, list):
                 config.netuid = [int(config.netuid)]
             else:
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/register.py` & `bittensor-5.1.0/bittensor/_cli/commands/register.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,19 +79,19 @@
         bittensor.wallet.add_args( register_parser )
         bittensor.subtensor.add_args( register_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
         check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
+        if not config.is_set('wallet.hotkey') and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
         if not config.no_prompt:
             check_for_cuda_reg_config(config)
 
 class RecycleRegisterCommand:
@@ -154,19 +154,19 @@
         )
 
         bittensor.wallet.add_args( recycle_register_parser )
         bittensor.subtensor.add_args( recycle_register_parser )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.subtensor.get('network') == bittensor.defaults.subtensor.network and not config.no_prompt:
+        if not config.is_set('subtensor.network') and not config.no_prompt:
             config.subtensor.network = Prompt.ask("Enter subtensor network", choices=bittensor.__networks__, default = bittensor.defaults.subtensor.network)
 
         check_netuid_set( config, subtensor = bittensor.subtensor( config = config ) )
 
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
+        if not config.is_set('wallet.hotkey') and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/stake.py` & `bittensor-5.1.0/bittensor/_cli/commands/stake.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,19 +133,19 @@
             return subtensor.add_stake( wallet=wallet, hotkey_ss58 = final_hotkeys[0][1], amount = None if config.get('stake_all') else final_amounts[0], wait_for_inclusion = True, prompt = not config.no_prompt )
 
         subtensor.add_stake_multiple( wallet = wallet, hotkey_ss58s=[hotkey_ss58 for _, hotkey_ss58 in final_hotkeys], amounts =  None if config.get('stake_all') else final_amounts, wait_for_inclusion = True, prompt = False )
 
 
     @classmethod
     def check_config( cls, config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
+        if not config.is_set('wallet.hotkey') and not config.no_prompt and not config.wallet.get('all_hotkeys') and not config.wallet.get('hotkeys'):
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
         # Get amount.
         if not config.get('amount') and not config.get('stake_all') and not config.get('max_stake'):
             if not Confirm.ask("Stake all Tao from account: [bold]'{}'[/bold]?".format(config.wallet.get('name', bittensor.defaults.wallet.name))):
                 amount = Prompt.ask("Enter Tao amount to stake")
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/transfer.py` & `bittensor-5.1.0/bittensor/_cli/commands/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         r""" Transfer token of amount to destination."""
         wallet = bittensor.wallet( config = cli.config )
         subtensor = bittensor.subtensor( config = cli.config )
         subtensor.transfer( wallet = wallet, dest = cli.config.dest, amount = cli.config.amount, wait_for_inclusion = True, prompt = not cli.config.no_prompt )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
         # Get destination.
         if not config.dest:
             dest = Prompt.ask("Enter destination public key: (ss58 or ed2519)")
             if not bittensor.utils.is_valid_bittensor_address_or_public_key( dest ):
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/unstake.py` & `bittensor-5.1.0/bittensor/_cli/commands/unstake.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 from bittensor.utils.balance import Balance
 from typing import List, Union, Optional, Dict, Tuple
 from .utils import get_hotkey_wallets_for_wallet
 console = bittensor.__console__
 
 class UnStakeCommand:
 
-    @classmethod
-    def check_config( cls, config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name and not config.no_prompt:
+    @classmethod   
+    def check_config( cls, config: 'bittensor.Config' ):        
+        if config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if not config.get('hotkey_ss58address') and config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
+        if not config.get( 'hotkey_ss58address', d=None ) and config.is_set('wallet.hotkey') and not config.no_prompt and not config.get('all_hotkeys') and not config.get('hotkeys'):
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
         # Get amount.
         if not config.get('hotkey_ss58address') and not config.get('amount') and not config.get('unstake_all') and not config.get('max_stake'):
             hotkeys: str = ''
             if config.get('all_hotkeys'):
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/utils.py` & `bittensor-5.1.0/bittensor/_cli/commands/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,22 @@
         # check if value is a valid choice or all the values in a list of ints are valid choices
         return value == "All" or \
             value in self.choices or \
             all( val.strip() in self.choices for val in value.replace(',', ' ').split( ))
 
 
 def check_netuid_set( config: 'bittensor.Config', subtensor: 'bittensor.Subtensor', allow_none: bool = False ):
-    if subtensor.network =='finney':
+    if subtensor.network != 'nakamoto':
         all_netuids = [str(netuid) for netuid in subtensor.get_subnets()]
         if len(all_netuids) == 0:
             console.print(":cross_mark:[red]There are no open networks.[/red]")
             sys.exit()
 
         # Make sure netuid is set.
-        if config.get('netuid', 'notset') == 'notset':
+        if not config.is_set('netuid'):
             if not config.no_prompt:
                 netuid = IntListPrompt.ask("Enter netuid", choices=all_netuids, default=str(all_netuids[0]))
             else:
                 netuid = str(bittensor.defaults.netuid) if not allow_none else 'None'
         else:
             netuid = config.netuid
```

### Comparing `bittensor-5.0.0/bittensor/_cli/commands/wallets.py` & `bittensor-5.1.0/bittensor/_cli/commands/wallets.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             # Password can be "", assume if None
             json_password = cli.config.get('json_password', "")
 
         wallet.regenerate_coldkey( mnemonic = cli.config.mnemonic, seed = cli.config.seed, json = (json_str, json_password), use_password = cli.config.use_password, overwrite = cli.config.overwrite_coldkey )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
         if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
@@ -124,15 +124,15 @@
     def run ( cli ):
         r""" Creates a new coldkeypub under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
         wallet.regenerate_coldkeypub( ss58_address=cli.config.get('ss58_address'), public_key=cli.config.get('public_key_hex'), overwrite = cli.config.overwrite_coldkeypub )
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
         if config.ss58_address == None and config.public_key_hex == None:
             prompt_answer = Prompt.ask("Enter the ss58_address or the public key in hex")
             if prompt_answer.startswith("0x"):
                 config.public_key_hex = prompt_answer
             else:
@@ -200,19 +200,19 @@
             # Password can be "", assume if None
             json_password = cli.config.get('json_password', "")
 
         wallet.regenerate_hotkey( mnemonic = cli.config.mnemonic, seed=cli.config.seed, json = (json_str, json_password), use_password = cli.config.use_password, overwrite = cli.config.overwrite_hotkey)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
+        if not config.is_set('wallet.hotkey') and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
         if config.mnemonic == None and config.get( 'seed', d=None ) == None and config.get( 'json', d=None ) == None:
             prompt_answer = Prompt.ask("Enter mnemonic, seed, or json file location")
             if prompt_answer.startswith("0x"):
                 config.seed = prompt_answer
             elif len(prompt_answer.split(" ")) > 1:
@@ -291,19 +291,19 @@
     def run( cli ):
         """ Creates a new hotke under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
         wallet.create_new_hotkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_hotkey)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
-        if config.wallet.get('hotkey') == bittensor.defaults.wallet.hotkey and not config.no_prompt:
+        if not config.is_set('wallet.hotkey') and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default = bittensor.defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         new_hotkey_parser = parser.add_parser( 'new_hotkey',  help='''Creates a new hotkey (for running a miner) under the specified path.''')
         new_hotkey_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
@@ -347,15 +347,15 @@
     def run ( cli ):
         r""" Creates a new coldkey under this wallet."""
         wallet = bittensor.wallet(config = cli.config)
         wallet.create_new_coldkey( n_words = cli.config.n_words, use_password = cli.config.use_password, overwrite = cli.config.overwrite_coldkey)
 
     @staticmethod
     def check_config( config: 'bittensor.Config' ):
-        if config.wallet.get('name') == bittensor.defaults.wallet.name  and not config.no_prompt:
+        if not config.is_set('wallet.name') and not config.no_prompt:
             wallet_name = Prompt.ask("Enter wallet name", default = bittensor.defaults.wallet.name)
             config.wallet.name = str(wallet_name)
 
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         new_coldkey_parser = parser.add_parser(
             'new_coldkey',
```

### Comparing `bittensor-5.0.0/bittensor/_config/__init__.py` & `bittensor-5.1.0/bittensor/_config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import sys
 from argparse import ArgumentParser, Namespace
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 import bittensor
 import yaml
 from loguru import logger
+import pandas as pd
 
 from . import config_impl
 
 logger = logger.opt(colors=True)
 
 class config:
     """
@@ -111,17 +112,58 @@
                 else:
                     head[keys[0]] = config_impl.Config()
                     head = head[keys[0]]
                     keys = keys[1:]
             if len(keys) == 1:
                 head[keys[0]] = arg_val
 
+        # Get defaults for this config
+        is_set_map = cls.__fill_is_set_list__(_config, bittensor.defaults)
+
+        _config['__is_set'] = is_set_map
+
+        _config.__fill_with_defaults__(is_set_map, bittensor.defaults)
+
         return _config
 
     @staticmethod
+    def __fill_is_set_list__(_config: 'bittensor.Config', defaults: 'bittensor.Config') -> Dict[str, bool]:
+        """Creates an is_set map
+        Args:
+            _config (bittensor.Config):
+                Config to generate is_set mapping.
+            defaults (bittensor.Config):
+                The bittensor defaults
+        Returns:
+            is_set_map (Dict[str, bool]):
+                A map from flattened param name to whether this param was set in a flag.
+        """
+        is_set_map = {}
+        config_d = _config.__dict__
+        # Only defaults we are concerned with
+        defaults_filtered = {}
+        for key in config_d.keys():
+            if key in defaults.keys():
+                defaults_filtered[key] = getattr(defaults, key)
+        # Avoid erroring out if defaults aren't set for a submodule
+        if defaults_filtered == {}:
+            return is_set_map
+
+        flat_config = pd.json_normalize(config_d, sep='.').to_dict('records')[0]
+        flat_defaults = pd.json_normalize(defaults_filtered, sep='.').to_dict('records')[0]
+        for key, _ in flat_defaults.items():
+            if key in flat_config:
+                is_set_map[key] = True
+            else:
+                is_set_map[key] = False
+        
+        return is_set_map
+
+
+    @staticmethod
     def __parse_args__( args: List[str], parser: ArgumentParser = None, strict: bool = False) -> Namespace:
         """Parses the passed args use the passed parser.
         Args:
             args (List[str]):
                 List of arguments to parse.
             parser (argparse.ArgumentParser):
                 Command line parser object.
@@ -146,8 +188,7 @@
         bittensor.wallet.add_args( parser )
         bittensor.subtensor.add_args( parser )
         bittensor.axon.add_args( parser )
         bittensor.metagraph.add_args( parser )
         bittensor.dataset.add_args( parser )
         bittensor.prometheus.add_args( parser )
         return bittensor.config( parser )
-
```

### Comparing `bittensor-5.0.0/bittensor/_dataset/__init__.py` & `bittensor-5.1.0/bittensor/_dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,18 @@
         return bittensor.config( parser )
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).dataset = bittensor.defaults.dataset
         try:
             parser.add_argument('--' + prefix_str + 'dataset.batch_size', type=int, help='Batch size.', default = bittensor.defaults.dataset.batch_size)
             parser.add_argument('--' + prefix_str + 'dataset.block_size', type=int, help='Number of text items to pull for each example..', default = bittensor.defaults.dataset.block_size)
             parser.add_argument('--' + prefix_str + 'dataset.num_workers',  type=int, help='Number of workers for data loader.', default = bittensor.defaults.dataset.num_workers)
             parser.add_argument('--' + prefix_str + 'dataset.dataset_names', type=str, required=False, nargs='*', action='store', help='Which datasets to use (ArXiv, BookCorpus2, Books3, DMMathematics, EnronEmails, EuroParl, Gutenberg_PG, HackerNews, NIHExPorter, OpenSubtitles, PhilPapers, UbuntuIRC, YoutubeSubtitles)).',
                                                                     default = bittensor.defaults.dataset.dataset_names)
             parser.add_argument('--' + prefix_str + 'dataset.data_dir', type=str, help='Where to save and load the data.', default = bittensor.defaults.dataset.data_dir)
```

### Comparing `bittensor-5.0.0/bittensor/_dataset/dataset_impl.py` & `bittensor-5.1.0/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_dataset/dataset_mock.py` & `bittensor-5.1.0/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_dataset/thread_queue.py` & `bittensor-5.1.0/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_dendrite/dendrite.py` & `bittensor-5.1.0/bittensor/_dendrite/dendrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             dendrite: 'bittensor.Dendrite',
             timeout: float = bittensor.__blocktime__
         ):
         self.dendrite = dendrite
         self.completed = False
         self.timeout = timeout
         self.start_time = time.time()
+        self.elapsed_time = 0.0
         self.src_hotkey = self.dendrite.keypair.ss58_address
         self.src_version = bittensor.__version_as_int__
         self.dest_hotkey = self.dendrite.axon_info.hotkey
         self.dest_version = self.dendrite.axon_info.version
         self.return_code: bittensor.proto.ReturnCode = bittensor.proto.ReturnCode.Success
         self.return_message: str = 'Success'
 
@@ -204,14 +205,15 @@
             dendrite_call.return_code = bittensor.proto.ReturnCode.UnknownException
             dendrite_call.return_message = str(e)
             bittensor.logging.trace( 'Dendrite.apply() unknown error: {}'.format( dendrite_call.return_message ) )
 
         finally:
             dendrite_call.end()
             dendrite_call.log_inbound()
+            dendrite_call.elapsed_time = time.time() - dendrite_call.start_time
             return dendrite_call
 
     def __exit__ ( self ):
         self.__del__()
 
     def close ( self ):
         self.__exit__()
```

### Comparing `bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite.py` & `bittensor-5.1.0/bittensor/_dendrite/text_prompting/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_dendrite/text_prompting/dendrite_pool.py` & `bittensor-5.1.0/bittensor/_dendrite/text_prompting/dendrite_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_ipfs/ipfs_impl.py` & `bittensor-5.1.0/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_keyfile/__init__.py` & `bittensor-5.1.0/bittensor/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_keyfile/keyfile_impl.py` & `bittensor-5.1.0/bittensor/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_logging/__init__.py` & `bittensor-5.1.0/bittensor/_logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,18 @@
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments fro parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).logging = bittensor.defaults.logging
         try:
             parser.add_argument('--' + prefix_str + 'logging.debug', action='store_true', help='''Turn on bittensor debugging information''', default = bittensor.defaults.logging.debug )
             parser.add_argument('--' + prefix_str + 'logging.trace', action='store_true', help='''Turn on bittensor trace level information''', default = bittensor.defaults.logging.trace )
             parser.add_argument('--' + prefix_str + 'logging.record_log', action='store_true', help='''Turns on logging to file.''', default = bittensor.defaults.logging.record_log )
             parser.add_argument('--' + prefix_str + 'logging.logging_dir', type=str, help='Logging default root directory.', default = bittensor.defaults.logging.logging_dir )
         except argparse.ArgumentError:
             # re-parsing arguments.
```

### Comparing `bittensor-5.0.0/bittensor/_metagraph/__init__.py` & `bittensor-5.1.0/bittensor/_metagraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,25 @@
         self.weights = torch.nn.Parameter(  torch.tensor( [], dtype=torch.float32), requires_grad=False )
         self.bonds = torch.nn.Parameter(  torch.tensor( [], dtype=torch.int64), requires_grad=False )
         self.uids = torch.nn.Parameter( torch.tensor([], dtype = torch.int64),requires_grad=False )
         self.axons = []
         if sync:
             self.sync( block = None, lite = lite )
 
-    def sync ( self, block: Optional[int] = None, lite: bool = True ) -> 'metagraph':
-        subtensor = bittensor.subtensor( network = self.network )
+    def sync ( self, block: Optional[int] = None, lite: bool = True, subtensor: Optional['bittensor.Subtensor'] = None ) -> 'metagraph':
+        if not subtensor:
+            subtensor = bittensor.subtensor( network = self.network )
         if lite:
             self.neurons = subtensor.neurons_lite( block = block, netuid = self.netuid )
         else:
             self.neurons = subtensor.neurons(block = block, netuid = self.netuid )
         self.lite = lite
         self.n = torch.nn.Parameter( torch.tensor( len(self.neurons), dtype=torch.int64 ), requires_grad=False )
         self.version = torch.nn.Parameter( torch.tensor( [bittensor.__version_as_int__], dtype=torch.int64 ), requires_grad=False )
-        self.block = torch.nn.Parameter( torch.tensor( subtensor.block, dtype=torch.int64 ), requires_grad=False )
+        self.block = torch.nn.Parameter( torch.tensor( block if block else subtensor.block, dtype=torch.int64 ), requires_grad=False )
         self.uids = torch.nn.Parameter( torch.tensor( [ neuron.uid for neuron in self.neurons ], dtype=torch.int64 ), requires_grad=False )
         self.trust = torch.nn.Parameter( torch.tensor( [ neuron.trust for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.consensus = torch.nn.Parameter( torch.tensor( [ neuron.consensus for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.incentive = torch.nn.Parameter( torch.tensor( [ neuron.incentive for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.dividends = torch.nn.Parameter( torch.tensor( [ neuron.dividends for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.ranks = torch.nn.Parameter( torch.tensor( [ neuron.rank for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.emission = torch.nn.Parameter( torch.tensor( [ neuron.emission for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
```

### Comparing `bittensor-5.0.0/bittensor/_prometheus/__init__.py` & `bittensor-5.1.0/bittensor/_prometheus/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,18 @@
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).prometheus = bittensor.defaults.prometheus
         try:
             parser.add_argument('--' + prefix_str + 'prometheus.port',  type=int, required=False, default = bittensor.defaults.prometheus.port,
                 help='''Prometheus serving port.''')
             parser.add_argument(
                 '--' + prefix_str + 'prometheus.level',
                 required = False,
                 type = str,
```

### Comparing `bittensor-5.0.0/bittensor/_proto/bittensor_pb2.py` & `bittensor-5.1.0/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-5.1.0/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_serializer/__init__.py` & `bittensor-5.1.0/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_serializer/serializer_impl.py` & `bittensor-5.1.0/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/__init__.py` & `bittensor-5.1.0/bittensor/_subtensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,20 @@
         cls.add_args( parser )
         print (cls.__new__.__doc__)
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).subtensor = bittensor.defaults.subtensor
         try:
-            parser.add_argument('--' + prefix_str + 'subtensor.network', default = bittensor.defaults.subtensor.network, type=str,
+            parser.add_argument('--' + prefix_str + 'subtensor.network', default = argparse.SUPPRESS, type=str,
                                 help='''The subtensor network flag. The likely choices are:
                                         -- finney (main network)
                                         -- local (local running network)
                                         -- mock (creates a mock connection (for testing))
                                     If this option is set it overloads subtensor.chain_endpoint with
                                     an entry point node from that network.
                                     ''')
```

### Comparing `bittensor-5.0.0/bittensor/_subtensor/chain_data.py` & `bittensor-5.1.0/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/errors.py` & `bittensor-5.1.0/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-5.1.0/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_subtensor/subtensor_impl.py` & `bittensor-5.1.0/bittensor/_subtensor/subtensor_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,33 +941,31 @@
         result = json_body['result']
 
         if result in (None, []):
             return []
 
         return NeuronInfoLite.list_from_vec_u8( result )
 
-    def metagraph( self, netuid: int, lite: bool = True ) -> 'bittensor.Metagraph':
+    def metagraph( self, netuid: int, lite: bool = True, block: Optional[int] = None ) -> 'bittensor.Metagraph':
         r""" Returns the metagraph for the subnet.
         Args:
             netuid ( int ):
                 The network uid of the subnet to query.
             lite (bool, default=True):
                 If true, returns a metagraph using the lite sync (no weights, no bonds)
+            block ( Optional[int] ):
+                block to sync from, or None for latest block.
         Returns:
             metagraph ( `bittensor.Metagraph` ):
                 The metagraph for the subnet at the block.
-        """
-        return bittensor.metagraph( network = self.network, netuid = netuid, lite = lite )
-
-    ################
-    #### Transfer ##
-    ################
-
-
+        """        
+        metagraph_ = bittensor.metagraph( network = self.network, netuid = netuid, lite = lite, sync = False )
+        metagraph_.sync( block = block, lite = lite, subtensor = self)
 
+        return metagraph_
 
     ################
     #### Legacy ####
     ################
 
     def get_balance(self, address: str, block: int = None) -> Balance:
         r""" Returns the token balance for the passed ss58_address address
```

### Comparing `bittensor-5.0.0/bittensor/_subtensor/subtensor_mock.py` & `bittensor-5.1.0/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_synapse/synapse.py` & `bittensor-5.1.0/bittensor/_synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_synapse/text_prompting/miner.py` & `bittensor-5.1.0/bittensor/_neuron/base_miner_neuron.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright © 2021 Yuma Rao
+# Copyright © 2023 Yuma Rao
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of
@@ -13,223 +13,182 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import os
 import time
-import copy
 import torch
+import threading
 import argparse
 import bittensor
 
 from rich import print
-from typing import List, Dict, Union, Tuple, Optional
+from typing import Union, Tuple
 from datetime import datetime
-from abc import ABC, abstractmethod
 
-class BasePromptingMiner( ABC ):
+class BaseMinerNeuron:
 
-    @classmethod
-    @abstractmethod
-    def add_args( cls, parser: argparse.ArgumentParser ):
-        ...
-
-    def priority( self, forward_call: "bittensor.TextPromptingForwardCall" ) -> float:
-        if self.metagraph is not None:
-            uid = self.metagraph.hotkeys.index(forward_call.src_hotkey)
-            return self.metagraph.S[uid].item()
-        else:
-            return self.config.neuron.default_priority
-
-    def blacklist( self, forward_call: "bittensor.TextPromptingForwardCall" ) -> Union[ Tuple[bool, str], bool ]:
-        # Check for registration
-        def registration_check():
-            is_registered = forward_call.src_hotkey in self.metagraph.hotkeys
-            if not is_registered:
-                if self.config.neuron.blacklist.allow_non_registered: return False, 'passed blacklist'
-                else: return True, 'pubkey not registered'
-
-        # Blacklist based on stake.
-        def stake_check() -> bool:
-            default_stake = self.config.neuron.blacklist.default_stake
-            if default_stake <= 0.0:
-                return False, 'passed blacklist'
-            uid = self.metagraph.hotkeys.index(forward_call.src_hotkey)
-            if self.metagraph.S[uid].item() < default_stake:
-                bittensor.logging.debug( "Blacklisted. Stake too low.")
-                return True, 'Stake too low.'
-            else: return False, 'passed blacklist'
-
-        # Optionally blacklist based on checks.
-        try:
-            registration_check()
-            stake_check()
-            return False, 'passed blacklist'
-        except Exception as e:
-            bittensor.logging.warning( "Blacklisted. Error in `registration_check` or `stake_check()" )
-            return True, 'Error in `registration_check` or `stake_check()'
-
-    @abstractmethod
-    def forward( self, messages: List[Dict[str, str]] ) -> str:
-        ...
-
-    @classmethod
-    @abstractmethod
-    def check_config( cls, config: 'bittensor.Config' ):
-        ...
+    def priority( self, forward_call: "bittensor.SynapseCall" ) -> float:
+        return self.prioritizer.priority( forward_call, metagraph = self.metagraph )
 
+    def blacklist( self, forward_call: "bittensor.SynapseCall" ) -> Union[ Tuple[bool, str], bool ]:
+        return self.blacklister.blacklist( forward_call, metagraph = self.metagraph )
+    
     @classmethod
     def config( cls ) -> "bittensor.Config":
         parser = argparse.ArgumentParser()
-        cls.add_super_args( parser )
+        cls.add_args( parser )
         return bittensor.config( parser )
 
     @classmethod
     def help( cls ):
         parser = argparse.ArgumentParser()
-        cls.add_super_args( parser )
         cls.add_args(parser)
         print( cls.__new__.__doc__ )
         parser.print_help()
 
     @classmethod
-    def super_check_config( cls, config: "bittensor.Config" ):
-        cls.check_config( config )
+    def check_config( cls, config: "bittensor.Config" ):
         bittensor.axon.check_config( config )
         bittensor.wallet.check_config( config )
         bittensor.logging.check_config( config )
         bittensor.subtensor.check_config( config )
         full_path = os.path.expanduser(
             '{}/{}/{}/{}'.format( config.logging.logging_dir, config.wallet.get('name', bittensor.defaults.wallet.name),
                                   config.wallet.get('hotkey', bittensor.defaults.wallet.hotkey), config.neuron.name ) )
         config.neuron.full_path = os.path.expanduser( full_path )
         if not os.path.exists( config.neuron.full_path ):
             os.makedirs( config.neuron.full_path )
 
     @classmethod
-    def add_super_args( cls, parser: argparse.ArgumentParser ):
-        cls.add_args(parser)
+    def add_args( cls, parser: argparse.ArgumentParser, prefix: str = None ):
+        prefix_str = "" if prefix is None else prefix + "."
         parser.add_argument(
-            '--netuid',
-            type = int,
-            help = 'Subnet netuid',
-            default = 41
+            '--' + prefix_str + 'netuid', 
+            type = int, 
+            help = 'Subnet netuid', 
+            default = 1
         )
         parser.add_argument(
-            '--neuron.name',
+            '--' + prefix_str + 'neuron.name', 
             type = str,
             help = 'Trials for this miner go in miner.root / (wallet_cold - wallet_hot) / miner.name ',
             default = 'openai_prompting_miner'
         )
         parser.add_argument(
-            '--neuron.blocks_per_epoch',
-            type = str,
+            '--' + prefix_str + 'neuron.blocks_per_epoch', 
+            type = str, 
             help = 'Blocks until the miner sets weights on chain',
             default = 100
         )
         parser.add_argument(
-            '--neuron.no_set_weights',
-            action = 'store_true',
+            '--' + prefix_str + 'neuron.no_set_weights', 
+            action = 'store_true', 
             help = 'If True, the model does not set weights.',
             default = False
         )
-        parser.add_argument(
-            '--neuron.max_batch_size',
-            type = int,
-            help = 'The maximum batch size for forward requests.',
-            default = -1
-        )
-        parser.add_argument(
-            '--neuron.max_sequence_len',
-            type = int,
-            help = 'The maximum sequence length for forward requests.',
-            default = -1
-        )
-        parser.add_argument(
-            '--neuron.blacklist.hotkeys',
-            type = str,
-            required = False,
-            nargs = '*',
-            action = 'store',
-            help = 'To blacklist certain hotkeys', default=[]
-        )
-        parser.add_argument(
-            '--neuron.blacklist.allow_non_registered',
-            action = 'store_true',
-            help = 'If True, the miner will allow non-registered hotkeys to mine.',
-            default = True
-        )
-        parser.add_argument(
-            '--neuron.blacklist.default_stake',
-            type = float,
-            help = 'Set default stake for miners.',
-            default = 0.0
-        )
-        parser.add_argument(
-            '--neuron.default_priority',
-            type = float,
-            help = 'Set default priority for miners.',
-            default = 0.0
-        )
-        bittensor.wallet.add_args( parser )
-        bittensor.axon.add_args( parser )
-        bittensor.subtensor.add_args( parser )
-        bittensor.logging.add_args( parser )
-
-    def __init__(
-        self,
-        config: "bittensor.Config" = None
-    ):
-        config = config if config != None else self.config()
-        self.config = copy.deepcopy( config )
-        self.super_check_config( self.config )
-        self.config.to_defaults()
+        bittensor.wallet.add_args( parser, prefix = prefix )
+        bittensor.axon.add_args( parser, prefix = prefix )
+        bittensor.subtensor.add_args( parser, prefix = prefix )
+        bittensor.logging.add_args( parser, prefix = prefix )
+        bittensor.blacklist.add_args( parser, prefix = prefix_str + 'neuron' )
+        bittensor.priority.add_args( parser, prefix = prefix_str + 'neuron' )
+
+    def __init__(self, netuid: int = None, config: "bittensor.Config" = None ):
+        super_config = config if config != None else BaseMinerNeuron.config() # Grab super (BaseMinerNeuron) config
+        child_config = self.config() # grab child (<subclass>Miner) class configs.
+        self.config = child_config
+        self.config.merge( super_config ) # Merge the two configs. Child configs override super configs.
+        self.config.netuid = netuid or self.config.netuid
+        BaseMinerNeuron.check_config( self.config )
+
+        # Build objects.
         bittensor.logging( config = self.config, logging_dir = self.config.neuron.full_path )
         self.subtensor = bittensor.subtensor( self.config )
         self.wallet = bittensor.wallet( self.config )
         self.metagraph = self.subtensor.metagraph( self.config.netuid )
-        self.axon = bittensor.axon(
-            wallet = self.wallet,
-            metagraph = self.metagraph,
-            config = self.config,
-        )
-        class Synapse( bittensor.TextPromptingSynapse ):
-            def priority( _, forward_call: "bittensor.TextPromptingForwardCall" ) -> float:
-                return self.priority( forward_call )
-            def blacklist( _, forward_call: "bittensor.TextPromptingForwardCall" ) -> Union[ Tuple[bool, str], bool ]:
-                return self.blacklist( forward_call )
-            def backward( self, messages: List[Dict[str, str]], response: str, rewards: torch.FloatTensor ) -> str: pass
-            def forward( _, messages: List[Dict[str, str]] ) -> str:
-                return self.forward( messages )
-        self.synapse = Synapse( axon = self.axon )
+        self.axon = bittensor.axon( wallet = self.wallet, config = self.config )
+        self.blacklister = bittensor.blacklist( config = self.config.neuron )
+        self.prioritizer = bittensor.priority( config = self.config.neuron )
+
+        # Used for backgounr process.
+        self.is_running = False
+        self.should_exit = False 
+        self.background_thread = None
+
+    def attach( self, synapse: "bittensor.Synapse" ):
+        # pass through attach function.
+        self.axon.attach( synapse )
+
+    def __enter__(self):
+        bittensor.logging.trace( 'BaseMinerNeuron.__enter__()' )
+        self.start_in_background()
+        return self
+    
+    def __exit__(self, exc_type, exc_value, traceback):
+        bittensor.logging.trace( 'BaseMinerNeuron.__exit__()' )
+        self.stop()
+
+    def start_in_background(self):
+        if self.is_running:
+            bittensor.logging.warning( 'The base miner neuron is already running.')
+        else:
+            self.should_exit = False
+            self.background_thread = threading.Thread( target = self.run, daemon = True )
+            self.background_thread.start()
+            self.is_running = True
+            bittensor.logging.trace( 'Starting the base miner neuron in the background.')
+
+    def stop(self):
+        if self.is_running:
+            self.should_exit = True
+        else:
+            bittensor.logging.warning( 'The base miner neuron is not running.')
 
     def run( self ):
+        bittensor.logging.debug( 'BaseMinerNeuron.run()' )
 
         # --- Start the miner.
+        self.is_running = True
         self.wallet.reregister( netuid = self.config.netuid, subtensor = self.subtensor )
         self.axon.start()
-        self.axon.netuid = self.config.netuid
-        self.axon.protocol = 4
-        self.subtensor.serve_axon( netuid = self.config.netuid, axon = self.axon )
+        self.subtensor.serve_axon( netuid = self.config.netuid, axon = self.axon, wait_for_finalization = False, wait_for_inclusion = False ) #TODO: fix finalization & inclusion
 
         # --- Run Forever.
         last_update = self.subtensor.get_current_block()
-        while True:
+        retries = 0
+        while not self.should_exit:
 
             # --- Wait until next epoch.
             current_block = self.subtensor.get_current_block()
             while (current_block - last_update) < self.config.neuron.blocks_per_epoch:
+                if self.should_exit: continue
                 time.sleep( 0.1 ) #bittensor.__blocktime__
                 current_block = self.subtensor.get_current_block()
             last_update = self.subtensor.get_current_block()
 
             # --- Update the metagraph with the latest network state.
-            self.metagraph.sync( lite = True )
-            uid = self.metagraph.hotkeys.index( self.wallet.hotkey.ss58_address )
+            try:
+                self.metagraph.sync( lite = True )
+                uid = self.metagraph.hotkeys.index( self.wallet.hotkey.ss58_address )
+            except:
+                # --- If we fail to sync the metagraph, wait and try again.
+                if(retries > 8):
+                    bittensor.logging.error( f'Failed to sync metagraph, exiting.')
+                    self.stop()
+                    break 
+                seconds_to_sleep = 5 * 1.5**(retries)
+                bittensor.logging.error( f'Failed to sync metagraph, retrying in {seconds_to_sleep} seconds.')
+                time.sleep( seconds_to_sleep )
+                retries += 1
+                continue
+
+            if(retries > 0):
+                retries = 0
 
             # --- Log performance.
             print(
                 f"[white not bold]{datetime.now():%Y-%m-%d %H:%M:%S}[/white not bold]{' ' * 4} | "
                 f"{f'UID [bright_cyan]{uid}[/bright_cyan]'.center(16 + len('[bright_cyan][/bright_cyan]'))} | "
                 f'[dim white not bold] [green]{str(self.metagraph.S[uid].item()):.4}[/green] Stake [/dim white not bold]'
                 f'[dim white not bold]| [yellow]{str(self.metagraph.trust[uid].item()) :.3}[/yellow] Trust [/dim white not bold]'
@@ -238,16 +197,18 @@
             # --- Set weights.
             if not self.config.neuron.no_set_weights:
                 try:
                     # --- query the chain for the most current number of peers on the network
                     chain_weights = torch.zeros( self.subtensor.subnetwork_n( netuid = self.config.netuid ))
                     chain_weights[uid] = 1
                     did_set = self.subtensor.set_weights(
-                        uids=torch.arange(0, len(chain_weights)),
-                        netuid=self.config.netuid,
-                        weights=chain_weights,
-                        wait_for_inclusion=False,
-                        wallet=self.wallet,
-                        version_key=1
+                        uids = torch.arange(0, len(chain_weights)),
+                        netuid = self.config.netuid,
+                        weights = chain_weights,
+                        wait_for_inclusion = False,
+                        walle = self.wallet,
+                        version_key = 1
                     )
                 except:
-                    pass
+                    pass
+
+        self.axon.stop()
```

### Comparing `bittensor-5.0.0/bittensor/_synapse/text_prompting/synapse.py` & `bittensor-5.1.0/bittensor/_synapse/text_prompting/synapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class SynapseForwardMulti( bittensor.SynapseCall ):
     name: str = "text_prompting_forward_multi"
     is_forward: bool = True
     multi_completions: List[ str ] = [""]
 
     def __init__(
             self,
-            synapse: "TextPromptingSynapseMulti",
+            synapse: "bittensor.TextPromptingSynapseMulti",
             request_proto: bittensor.proto.MultiForwardTextPromptingRequest,
             multi_forward_callback: Callable,
         ):
         super().__init__( synapse = synapse, request_proto = request_proto )
         self.messages: List[ Dict[str, str] ] = request_proto.messages
         self.formatted_messages = [ json.loads(message) for message in self.messages ]
         self.multi_forward_callback = multi_forward_callback
```

### Comparing `bittensor-5.0.0/bittensor/_threadpool/__init__.py` & `bittensor-5.1.0/bittensor/_threadpool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,18 @@
         return priority_thread_pool_impl.PriorityThreadPoolExecutor(maxsize = config.priority.maxsize, max_workers = config.priority.max_workers)
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).priority = bittensor.defaults.priority
         try:
             parser.add_argument('--' + prefix_str + 'priority.max_workers', type = int, help='''maximum number of threads in thread pool''', default = bittensor.defaults.priority.max_workers)
             parser.add_argument('--' + prefix_str + 'priority.maxsize', type=int, help='''maximum size of tasks in priority queue''', default = bittensor.defaults.priority.maxsize)
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
```

### Comparing `bittensor-5.0.0/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-5.1.0/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_tokenizer/__init__.py` & `bittensor-5.1.0/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_wallet/__init__.py` & `bittensor-5.1.0/bittensor/_wallet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,17 +103,21 @@
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: str = None ):
         """ Accept specific arguments from parser
         """
         prefix_str = '' if prefix == None else prefix + '.'
+        if prefix is not None:
+            if not hasattr(bittensor.defaults, prefix):
+                setattr(bittensor.defaults, prefix, bittensor.Config())
+            getattr(bittensor.defaults, prefix).wallet = bittensor.defaults.wallet
         try:
-            parser.add_argument('--' + prefix_str + 'wallet.name', required=False, default=bittensor.defaults.wallet.name, help='''The name of the wallet to unlock for running bittensor (name mock is reserved for mocking this wallet)''')
-            parser.add_argument('--' + prefix_str + 'wallet.hotkey', required=False, default=bittensor.defaults.wallet.hotkey, help='''The name of wallet's hotkey.''')
+            parser.add_argument('--' + prefix_str + 'wallet.name', required=False, default=argparse.SUPPRESS, help='''The name of the wallet to unlock for running bittensor (name mock is reserved for mocking this wallet)''')
+            parser.add_argument('--' + prefix_str + 'wallet.hotkey', required=False, default=argparse.SUPPRESS, help='''The name of wallet's hotkey.''')
             parser.add_argument('--' + prefix_str + 'wallet.path', required=False, default=bittensor.defaults.wallet.path, help='''The path to your bittensor wallets''')
             parser.add_argument('--' + prefix_str + 'wallet._mock', action='store_true', default=bittensor.defaults.wallet._mock, help='To turn on wallet mocking for testing purposes.')
 
             parser.add_argument('--' + prefix_str + 'wallet.reregister', required=False, action='store', default=bittensor.defaults.wallet.reregister, type=strtobool, help='''Whether to reregister the wallet if it is not already registered.''')
 
         except argparse.ArgumentError as e:
             pass
```

### Comparing `bittensor-5.0.0/bittensor/_wallet/wallet_impl.py` & `bittensor-5.1.0/bittensor/_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/_wallet/wallet_mock.py` & `bittensor-5.1.0/bittensor/_wallet/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/__init__.py` & `bittensor-5.1.0/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/_register_cuda.py` & `bittensor-5.1.0/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/balance.py` & `bittensor-5.1.0/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/codes.py` & `bittensor-5.1.0/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/formatting.py` & `bittensor-5.1.0/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/networking.py` & `bittensor-5.1.0/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/registration.py` & `bittensor-5.1.0/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/registratrion_old.py` & `bittensor-5.1.0/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/stats.py` & `bittensor-5.1.0/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/test_utils.py` & `bittensor-5.1.0/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/tokenizer_utils.py` & `bittensor-5.1.0/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor/utils/weight_utils.py` & `bittensor-5.1.0/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/bittensor.egg-info/SOURCES.txt` & `bittensor-5.1.0/bittensor.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 bittensor/__init__.py
 bittensor.egg-info/PKG-INFO
 bittensor.egg-info/SOURCES.txt
 bittensor.egg-info/dependency_links.txt
 bittensor.egg-info/requires.txt
 bittensor.egg-info/top_level.txt
 bittensor/_axon/__init__.py
+bittensor/_blacklist/__init__.py
 bittensor/_cli/__init__.py
 bittensor/_cli/cli_impl.py
 bittensor/_cli/commands/__init__.py
 bittensor/_cli/commands/delegates.py
 bittensor/_cli/commands/inspect.py
 bittensor/_cli/commands/list.py
 bittensor/_cli/commands/metagraph.py
@@ -37,14 +38,20 @@
 bittensor/_dendrite/text_prompting/dendrite_pool.py
 bittensor/_ipfs/__init__.py
 bittensor/_ipfs/ipfs_impl.py
 bittensor/_keyfile/__init__.py
 bittensor/_keyfile/keyfile_impl.py
 bittensor/_logging/__init__.py
 bittensor/_metagraph/__init__.py
+bittensor/_neuron/__init__.py
+bittensor/_neuron/base_huggingface_miner.py
+bittensor/_neuron/base_miner_neuron.py
+bittensor/_neuron/base_prompting_miner.py
+bittensor/_neuron/base_validator.py
+bittensor/_priority/__init__.py
 bittensor/_prometheus/__init__.py
 bittensor/_proto/__init__.py
 bittensor/_proto/bittensor_pb2.py
 bittensor/_proto/bittensor_pb2_grpc.py
 bittensor/_serializer/__init__.py
 bittensor/_serializer/serializer_impl.py
 bittensor/_subtensor/__init__.py
@@ -61,15 +68,14 @@
 bittensor/_subtensor/extrinsics/set_weights.py
 bittensor/_subtensor/extrinsics/staking.py
 bittensor/_subtensor/extrinsics/transfer.py
 bittensor/_subtensor/extrinsics/unstaking.py
 bittensor/_synapse/__init__.py
 bittensor/_synapse/synapse.py
 bittensor/_synapse/text_prompting/__init__.py
-bittensor/_synapse/text_prompting/miner.py
 bittensor/_synapse/text_prompting/synapse.py
 bittensor/_threadpool/__init__.py
 bittensor/_threadpool/priority_thread_pool_impl.py
 bittensor/_tokenizer/__init__.py
 bittensor/_wallet/__init__.py
 bittensor/_wallet/wallet_impl.py
 bittensor/_wallet/wallet_mock.py
```

### Comparing `bittensor-5.0.0/bittensor.egg-info/requires.txt` & `bittensor-5.1.0/bittensor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bittensor-5.0.0/setup.py` & `bittensor-5.1.0/setup.py`

 * *Files identical despite different names*


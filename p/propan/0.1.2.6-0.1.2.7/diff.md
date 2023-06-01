# Comparing `tmp/propan-0.1.2.6.tar.gz` & `tmp/propan-0.1.2.7.tar.gz`

## Comparing `propan-0.1.2.6.tar` & `propan-0.1.2.7.tar`

### file list

```diff
@@ -1,142 +1,143 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.6/SECURITY.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__about__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__main__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/py.typed
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/sqs.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/test.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.6/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.6/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.6/README.md
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.6/pyproject.toml
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.7/SECURITY.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__about__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__main__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/test.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.7/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.7/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.7/README.md
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.7/pyproject.toml
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.7/PKG-INFO
```

### Comparing `propan-0.1.2.6/CONTRIBUTING.md` & `propan-0.1.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/SECURITY.md` & `propan-0.1.2.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/.github/workflows/documentation.yml` & `propan-0.1.2.7/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/.github/workflows/publish_coverage.yml` & `propan-0.1.2.7/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/.github/workflows/publish_pypi.yml` & `propan-0.1.2.7/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/.github/workflows/tests.yml` & `propan-0.1.2.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/3_lifespan_events.py` & `propan-0.1.2.7/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.7/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/5_publishing.py` & `propan-0.1.2.7/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/6_arguments_casting.py` & `propan-0.1.2.7/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/7_handler_errors_processing.py` & `propan-0.1.2.7/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.7/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.7/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.7/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.7/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.7/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/dependencies/7_annotated.py` & `propan-0.1.2.7/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.7/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/rabbit/direct.py` & `propan-0.1.2.7/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/rabbit/fanout.py` & `propan-0.1.2.7/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/rabbit/header.py` & `propan-0.1.2.7/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/rabbit/topic.py` & `propan-0.1.2.7/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/redis/direct.py` & `propan-0.1.2.7/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/examples/redis/pattern.py` & `propan-0.1.2.7/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/__about__.py` & `propan-0.1.2.7/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.2.6"
+__version__ = "0.1.2.7"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.2.6/propan/__init__.py` & `propan-0.1.2.7/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/annotations.py` & `propan-0.1.2.7/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/types.py` & `propan-0.1.2.7/propan/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 SendableMessage: TypeAlias = Union[
     DecodedMessage,
     BaseModel,
     None,
 ]
 
-HandlerCallable: TypeAlias = Callable[
-    ...,
-    Union[Awaitable[SendableMessage], SendableMessage],
+HandlerCallable: TypeAlias = Union[
+    Callable[..., Awaitable[SendableMessage]],
+    Callable[..., SendableMessage],
 ]
 HandlerWrapper: TypeAlias = Callable[
     [HandlerCallable],
     HandlerCallable,
 ]
```

### Comparing `propan-0.1.2.6/propan/brokers/push_back_watcher.py` & `propan-0.1.2.7/propan/brokers/push_back_watcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import Counter
 from logging import Logger
 from types import TracebackType
 from typing import Callable, Optional, Type
 
 from typing_extensions import Counter as CounterType
 
+from propan.brokers.exceptions import SkipMessage
 from propan.utils.functions import call_or_await
 
 
 class BaseWatcher(ABC):
     max_tries: int
 
     def __init__(
@@ -40,14 +41,25 @@
     def is_max(self, message_id: str) -> bool:
         return False
 
     def remove(self, message_id: str) -> None:
         pass
 
 
+class NotPushBackWatcher(BaseWatcher):
+    def add(self, message_id: str) -> None:
+        pass
+
+    def is_max(self, message_id: str) -> bool:
+        return True
+
+    def remove(self, message_id: str) -> None:
+        pass
+
+
 class PushBackWatcher(BaseWatcher):
     memory: CounterType[str]
 
     def __init__(
         self,
         max_tries: int = 3,
         logger: Optional[Logger] = None,
@@ -96,13 +108,16 @@
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         if not exc_type:
             await call_or_await(self.on_success)
             self.watcher.remove(self._message_id)
 
+        elif isinstance(exc_val, SkipMessage) is True:
+            self.watcher.remove(self._message_id)
+
         elif self.watcher.is_max(self._message_id):
             await call_or_await(self.on_max)
             self.watcher.remove(self._message_id)
 
         else:
             await call_or_await(self.on_error)
```

### Comparing `propan-0.1.2.6/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.7/propan/brokers/_model/broker_usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from propan.brokers._model.utils import (
     change_logger_handlers,
     get_watcher,
     set_message_context,
     suppress_decor,
 )
+from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import (
     AnyCallable,
     AnyDict,
     DecodedMessage,
     DecoratedAsync,
@@ -202,43 +203,46 @@
 
         return wrapper
 
     def _wrap_parse_message(
         self, func: Callable[[PropanMessage], Awaitable[T]]
     ) -> Callable[[Any], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: Any) -> T:
+        async def parse_wrapper(message: Any) -> T:
             return await func(await self._parse_message(message))
 
-        return wrapper
+        return parse_wrapper
 
     def _log_execution(
         self,
         **broker_args: Any,
     ) -> Wrapper:
         def decor(
             func: Callable[[PropanMessage], Awaitable[T]]
         ) -> Callable[[PropanMessage], Awaitable[T]]:
             @wraps(func)
-            async def wrapper(message: PropanMessage) -> T:
+            async def log_wrapper(message: PropanMessage) -> T:
                 log_context = self._get_log_context(message=message, **broker_args)
 
                 with context.scope("log_context", log_context):
                     self._log("Received", extra=log_context)
 
                     try:
                         r = await func(message)
+                    except SkipMessage as e:
+                        self._log("Skipped", extra=log_context)
+                        raise e
                     except Exception as e:
                         self._log(repr(e), logging.ERROR)
                         raise e
                     else:
                         self._log("Processed", extra=log_context)
                         return r
 
-            return wrapper
+            return log_wrapper
 
         return decor
 
     def _log(
         self,
         message: str,
         log_level: Optional[int] = None,
```

### Comparing `propan-0.1.2.6/propan/brokers/_model/schemas.py` & `propan-0.1.2.7/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/_model/utils.py` & `propan-0.1.2.7/propan/brokers/_model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.utils import context
 
 T = TypeVar("T")
+P = TypeVar("P")
 
 
 def change_logger_handlers(logger: logging.Logger, fmt: str) -> None:
     for handler in logger.handlers:
         formatter = handler.formatter
         if formatter is not None:
             use_colors = getattr(formatter, "use_colors", None)
@@ -36,21 +37,20 @@
     else:
         watcher = PushBackWatcher(logger=logger, max_tries=try_number)
     return watcher
 
 
 def suppress_decor(
     func: Callable[[Any], Awaitable[T]]
-) -> Callable[[Any], Awaitable[Optional[T]]]:
+) -> Callable[[Any, bool], Awaitable[Optional[T]]]:
     @wraps(func)
     async def wrapper(message: Any, reraise_exc: bool = False) -> Optional[T]:
         try:
             return await func(message)
         except Exception as e:
-            print(e)
             if reraise_exc is True:
                 raise e
             return None
 
     return wrapper
```

### Comparing `propan-0.1.2.6/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.7/propan/brokers/kafka/kafka_broker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 import asyncio
 import logging
 from functools import partial, wraps
 from typing import Any, Callable, Dict, List, NoReturn, Optional, Sequence, Tuple, Union
+from uuid import uuid4
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord
-from typing_extensions import TypeVar
+from typing_extensions import TypeAlias, TypeVar
 
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.exceptions import SkipMessage
 from propan.brokers.kafka.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.types import (
     AnyCallable,
     AnyDict,
+    DecodedMessage,
     DecoratedCallable,
     SendableMessage,
     Wrapper,
 )
 from propan.utils.context import context
 
 T = TypeVar("T")
+CorrelationId: TypeAlias = str
 
 
 class KafkaBroker(BrokerUsecase):
     _publisher: Optional[AIOKafkaProducer]
     _connection: Callable[[Tuple[str, ...]], AIOKafkaConsumer]
     __max_topic_len: int
+    response_topic: str
+    response_callbacks: Dict[CorrelationId, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
+        response_topic: str = "",
         log_fmt: Optional[str] = None,
         **kwargs: AnyDict,
     ) -> None:
         super().__init__(bootstrap_servers, log_fmt=log_fmt, **kwargs)
         self.__max_topic_len = 4
         self._publisher = None
+        self.response_topic = response_topic
+        self.response_callbacks = {}
 
     async def _connect(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         **kwargs: Any,
     ) -> AIOKafkaConsumer:
         kwargs["client_id"] = kwargs.get("client_id", "propan-" + __version__)
@@ -75,14 +84,18 @@
                 "sasl_oauth_token_provider",
             }
             and v
         }
         return partial(AIOKafkaConsumer, **consumer_kwargs)
 
     async def close(self) -> None:
+        for f in self.response_callbacks.values():
+            f.cancel()
+        self.response_callbacks = {}
+
         for handler in self.handlers:
             if handler.task is not None:
                 handler.task.cancel()
                 handler.task = None
 
             if handler.consumer is not None:
                 await handler.consumer.stop()
@@ -111,14 +124,21 @@
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        if self.response_topic:
+            self.handle(
+                self.response_topic,
+                _raw=True,
+                enable_auto_commit=False,
+            )(self._consume_response)
+
         context.set_local(
             "log_context",
             self._get_log_context(None, ""),
         )
 
         await super().start()
 
@@ -144,15 +164,24 @@
         )
 
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
     ) -> Callable[[PropanMessage], T]:
         @wraps(func)
         async def wrapper(message: PropanMessage) -> T:
-            return await func(message)
+            r = await func(message)
+
+            if message.reply_to:
+                await self.publish(
+                    message=r or "",
+                    headers={"correlation_id": message.headers.get("correlation_id")},
+                    topic=message.reply_to,
+                )
+
+            return r
 
         return wrapper
 
     async def publish(
         self,
         message: SendableMessage,
         topic: str,
@@ -161,32 +190,66 @@
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         *,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> Any:
+    ) -> Optional[DecodedMessage]:
         message, content_type = super()._encode_message(message)
 
-        headers = {
+        headers_to_send = {
             "content-type": content_type or "",
-            "reply_to": reply_to,
             **(headers or {}),
         }
 
-        return await self._publisher.send(
+        if callback is True:
+            reply_to = reply_to or self.response_topic
+            if not reply_to:
+                raise ValueError(
+                    "You should specify `response_topic` at init or use `reply_to` argument"
+                )
+
+        if reply_to:
+            correlation_id = str(uuid4())
+            headers_to_send.update(
+                {
+                    "reply_to": reply_to,
+                    "correlation_id": correlation_id,
+                }
+            )
+        else:
+            correlation_id = ""
+
+        response_future: Optional["asyncio.Future[DecodedMessage]"]
+        if callback is True:
+            response_future = asyncio.Future()
+            self.response_callbacks[correlation_id] = response_future
+        else:
+            response_future = None
+
+        await self._publisher.send(
             topic=topic,
             value=message,
             key=key,
             partition=partition,
             timestamp_ms=timestamp_ms,
-            headers=[(i, j.encode()) for i, j in headers.items()],
+            headers=[(i, j.encode()) for i, j in headers_to_send.items()],
         )
 
+        if response_future is not None:
+            try:
+                response = await asyncio.wait_for(response_future, callback_timeout)
+            except asyncio.TimeoutError as e:
+                if raise_timeout is True:
+                    raise e
+                return None
+            else:
+                return response
+
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(topic)-{self.__max_topic_len}s | "
             "%(message_id)-10s "
             "- %(message)s"
@@ -215,7 +278,16 @@
         while True:
             try:
                 msg = await handler.consumer.getone()
             except Exception as e:
                 self._log(e, logging.WATNING, c)
             else:
                 await handler.callback(msg)
+
+    async def _consume_response(self, message: PropanMessage):
+        correlation_id = message.headers.get("correlation_id")
+        if correlation_id is not None:
+            callback = self.response_callbacks.pop(correlation_id, None)
+            if callback is not None:
+                callback.set_result(await self._decode_message(message))
+
+        raise SkipMessage()
```

### Comparing `propan-0.1.2.6/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.7/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import logging
-from asyncio import AbstractEventLoop
+from asyncio import AbstractEventLoop, Future
 from ssl import SSLContext
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
 from aiokafka.structs import ConsumerRecord
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
-from typing_extensions import Literal, TypeVar
+from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.kafka.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
-from propan.types import SendableMessage, Wrapper
+from propan.types import DecodedMessage, SendableMessage, Wrapper
 
 T = TypeVar("T")
 Partition = TypeVar("Partition")
+CorrelationId: TypeAlias = str
 
 class KafkaBroker(BrokerUsecase):
     _publisher: Optional[AIOKafkaProducer]
     _connection: Callable[[Tuple[str, ...]], AIOKafkaConsumer]
     __max_topic_len: int
+    response_topic: str
+    response_callbacks: Dict[CorrelationId, "Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
+        response_topic: str = "",
         # both
         client_id: str = "propan-" + __version__,
         request_timeout_ms: int = 40 * 1000,
         retry_backoff_ms: int = 100,
         metadata_max_age_ms: int = 5 * 60 * 1000,
         security_protocol: Literal[
             "SSL",
@@ -177,15 +181,15 @@
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         *,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> Any: ...
+    ) -> Optional[DecodedMessage]: ...
     @property
     def fmt(self) -> str: ...
     def _get_log_context(  # type: ignore[override]
         self,
         message: Optional[PropanMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]: ...
```

### Comparing `propan-0.1.2.6/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.7/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.7/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.7/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/nats/schemas.py` & `propan-0.1.2.7/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.7/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.7/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.7/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/redis/schemas.py` & `propan-0.1.2.7/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.7/propan/brokers/sqs/sqs_broker.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,116 +8,134 @@
     List,
     NoReturn,
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
+from uuid import uuid4
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.session import get_session
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
+from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
-    FakePushBackWatcher,
+    NotPushBackWatcher,
     WatcherContext,
 )
-from propan.brokers.sqs.schema import Handler, SQSQueue
-from propan.types import AnyCallable, DecoratedCallable, HandlerWrapper, SendableMessage
+from propan.brokers.sqs.schema import Handler, SQSMessage, SQSQueue
+from propan.types import (
+    AnyCallable,
+    DecodedMessage,
+    DecoratedCallable,
+    HandlerWrapper,
+    SendableMessage,
+)
 from propan.utils import context
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
+CorrelationId: TypeAlias = str
 
 
 class SQSBroker(BrokerUsecase):
     _connection: AioBaseClient
     _queues: Dict[str, QueueUrl]
-    handlers: List[Handler]
     __max_queue_len: int
+    response_queue: str
+    response_callbacks: Dict[CorrelationId, "asyncio.Future[DecodedMessage]"]
+    handlers: List[Handler]
 
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         log_fmt: Optional[str] = None,
+        response_queue: str = "",
         **kwargs: Any,
     ) -> None:
         super().__init__(url, log_fmt=log_fmt, **kwargs)
         self._queues = {}
         self.__max_queue_len = 4
+        self.response_queue = response_queue
+        self.response_callbacks = {}
 
     async def _connect(self, url: Optional[str] = None, **kwargs: Any) -> AioBaseClient:
         session = get_session()
         client: AioBaseClient = await session._create_client(
             service_name="sqs", endpoint_url=url, **kwargs
         )
         context.set_global("client", client)
         await client.__aenter__()
         return client
 
     async def close(self) -> None:
+        for f in self.response_callbacks.values():
+            f.cancel()
+        self.response_callbacks = {}
+
         for h in self.handlers:
             if h.task is not None:
                 h.task.cancel()
                 h.task = None
 
         if self._connection is not None:
             await self._connection.__aexit__(None, None, None)
             self._connection = None
 
     async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage:
         attributes = message.get("MessageAttributes", {})
 
-        headers = {}
-        for i, j in attributes.items():
-            v = j.get("StringValue", "0")
-            if v != "0":
-                headers[i] = v
-            else:
-                headers[i] = None
+        headers = {i: j.get("StringValue") for i, j in attributes.items()}
 
         return PropanMessage(
             body=message.get("Body", "").encode(),
             message_id=message.get("MessageId"),
             content_type=headers.pop("content-type", None),
-            reply_to=headers.pop("reply", None) or "",
+            reply_to=headers.pop("reply_to", None) or "",
             headers=headers,
             raw_message=message,
         )
 
     def _process_message(
         self,
         func: Callable[[PropanMessage], T],
         watcher: Optional[BaseWatcher],
     ) -> Callable[[PropanMessage], T]:
         if watcher is None:
-            watcher = FakePushBackWatcher()
+            watcher = NotPushBackWatcher()
 
         @wraps(func)
-        async def wrapper(message: PropanMessage) -> T:
+        async def process_wrapper(message: PropanMessage) -> T:
             context = WatcherContext(
                 watcher,
                 message.message_id,
                 on_success=self.delete_message,
                 on_max=self.delete_message,
             )
 
             async with context:
                 r = await func(message)
 
                 if message.reply_to:
-                    await self.publish(r or "", message.reply_to)
+                    await self.publish(
+                        message=r or "",
+                        queue=message.reply_to,
+                        headers={
+                            "correlation_id": message.headers.get("correlation_id")
+                        },
+                    )
 
                 return r
 
-        return wrapper
+        return process_wrapper
 
     def handle(
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
@@ -136,15 +154,16 @@
         params = {
             "WaitTimeSeconds": wait_interval,
             "MaxNumberOfMessages": max_messages_number,
             "AttributeNames": [*attributes],
             "VisibilityTimeout": visibility_timeout,
             "MessageAttributeNames": (
                 "content-type",
-                "reply",
+                "reply_to",
+                "correlation_id",
                 *message_attributes,
             ),
         }
         if request_attempt_id is not None:
             params["ReceiveRequestAttemptId"] = request_attempt_id
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
@@ -157,14 +176,20 @@
             handler = Handler(callback=func, queue=queue, consumer_params=params)
             self.handlers.append(handler)
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        if self.response_queue:
+            self.handle(
+                self.response_queue,
+                _raw=True,
+            )(self._consume_response)
+
         context.set_local(
             "log_context",
             self._get_log_context(None, ""),
         )
 
         await super().start()
 
@@ -191,74 +216,57 @@
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
     ) -> None:
         queue_url = await self.get_queue(queue)
 
-        params = self._build_message(
+        if callback is True:
+            reply_to = reply_to or self.response_queue
+            if not reply_to:
+                raise ValueError(
+                    "You should specify `response_queue` at init or use `reply_to` argument"
+                )
+
+        if reply_to:
+            correlation_id = str(uuid4())
+        else:
+            correlation_id = ""
+
+        response_future: Optional["asyncio.Future[DecodedMessage]"]
+        if callback is True:
+            response_future = asyncio.Future()
+            self.response_callbacks[correlation_id] = response_future
+        else:
+            response_future = None
+
+        params = SQSMessage(
             message=message,
-            queue_url=queue_url,
-            headers=headers,
+            headers=headers or {},
             delay_seconds=delay_seconds,
-            message_attributes=message_attributes,
-            message_system_attributes=message_system_attributes,
+            message_attributes=message_attributes or {},
+            message_system_attributes=message_system_attributes or {},
             deduplication_id=deduplication_id,
             group_id=group_id,
+        ).to_params(
             reply_to=reply_to,
+            correlation_id=correlation_id,
         )
 
-        await self._connection.send_message(**params)
-
-    @classmethod
-    def _build_message(
-        cls,
-        message: SendableMessage,
-        queue_url: str,
-        *,
-        headers: Optional[Dict[str, str]] = None,
-        delay_seconds: int = 0,  # 0...900
-        message_attributes: Optional[Dict[str, Any]] = None,
-        message_system_attributes: Optional[Dict[str, Any]] = None,
-        # FIFO only
-        deduplication_id: Optional[str] = None,
-        group_id: Optional[str] = None,
-        # broker
-        reply_to: str = "",
-    ) -> Dict[str, Any]:
-        msg, content_type = cls._encode_message(message)
-
-        headers = headers or {}
-        headers["content-type"] = headers.get("content-type", content_type)
-        headers["reply"] = reply_to
-
-        params = {
-            "QueueUrl": queue_url,
-            "MessageBody": msg.decode(),
-            "DelaySeconds": delay_seconds,
-            "MessageSystemAttributes": message_system_attributes or {},
-            "MessageAttributes": {
-                **(message_attributes or {}),
-                **{
-                    i: {
-                        "StringValue": j or "0",
-                        "DataType": "String",
-                    }
-                    for i, j in headers.items()
-                },
-            },
-        }
-
-        if deduplication_id is not None:
-            params["MessageDeduplicationId"] = deduplication_id
-
-        if group_id is not None:
-            params["MessageGroupId"] = group_id
+        await self._connection.send_message(QueueUrl=queue_url, **params)
 
-        return params
+        if response_future is not None:
+            try:
+                response = await asyncio.wait_for(response_future, callback_timeout)
+            except asyncio.TimeoutError as e:
+                if raise_timeout is True:
+                    raise e
+                return None
+            else:
+                return response
 
     async def create_queue(self, queue: SQSQueue) -> QueueUrl:
         url = self._queues.get(queue.name)
         if url is None:  # pragma: no branch
             url = (
                 await self._connection.create_queue(
                     QueueName=queue.name,
@@ -321,16 +329,37 @@
                     await asyncio.sleep(5)
 
                 else:
                     if connected is False:
                         self._log("Connection established", logging.INFO, c)
                         connected = True
 
-                    for msg in r.get("Messages", []):
-                        await handler.callback(msg)
+                    messages = r.get("Messages", [])
+                    for msg in messages:
+                        try:
+                            await handler.callback(msg, True)
+                        except Exception:
+                            has_trash_messages = True
+                        else:
+                            has_trash_messages = False
+
+                    if has_trash_messages is True:
+                        await asyncio.sleep(
+                            handler.consumer_params.get("WaitTimeSeconds", 1.0)
+                        )
+
+    async def _consume_response(self, message: PropanMessage):
+        correlation_id = message.headers.get("correlation_id")
+        if correlation_id is not None:
+            callback = self.response_callbacks.pop(correlation_id, None)
+            if callback is not None:
+                callback.set_result(await self._decode_message(message))
+                return
+
+        raise SkipMessage()
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(queue)-{self.__max_queue_len}s | "
             "%(message_id)-10s "
```

### Comparing `propan-0.1.2.6/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.7/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NoReturn,
@@ -16,28 +17,31 @@
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.sqs.schema import Handler, SQSQueue
 from propan.log import access_logger
-from propan.types import HandlerWrapper, SendableMessage
+from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
 
 class SQSBroker(BrokerUsecase):
     _connection: AioBaseClient
     _queues: Dict[str, QueueUrl]
+    response_queue: str
+    response_callbacks: Dict[str, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
+        response_queue: str = "",
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
         verify: Optional[bool] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
@@ -59,22 +63,16 @@
         verify: Optional[bool] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         config: Optional[AioConfig] = None,
     ) -> AioBaseClient:
         """"""
-    async def _connect(self, *args: Any, **kwargs: Any) -> AioBaseClient: ...
-    async def close(self) -> None: ...
-    async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage: ...
-    def _process_message(
-        self,
-        func: Callable[[PropanMessage], T],
-        watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]: ...
+    async def close(self) -> None:
+        """"""
     async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
         queue: str,
         *,
         headers: Optional[Dict[str, str]] = None,
         delay_seconds: int = 0,
@@ -82,47 +80,61 @@
         message_system_attributes: Optional[Dict[str, Any]] = None,
         deduplication_id: Optional[str] = None,
         group_id: Optional[str] = None,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> None: ...
-    @classmethod
-    def _build_message(
-        cls,
-        message: SendableMessage,
-        queue_url: str,
-        *,
-        headers: Optional[Dict[str, str]] = None,
-        delay_seconds: int = 0,  # 0...900
-        message_attributes: Optional[Dict[str, Any]] = None,
-        message_system_attributes: Optional[Dict[str, Any]] = None,
-        # FIFO only
-        deduplication_id: Optional[str] = None,
-        group_id: Optional[str] = None,
-        # broker
-        reply_to: str = "",
-    ) -> Dict[str, Any]: ...
+    ) -> None:
+        """"""
     def handle(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
-    ) -> HandlerWrapper: ...
-    async def start(self) -> None: ...
-    async def create_queue(self, queue: str) -> QueueUrl: ...
-    async def delete_queue(self, queue: str) -> None: ...
-    async def get_queue(self, queue: str) -> QueueUrl: ...
-    async def delete_message(self) -> None: ...
+    ) -> HandlerWrapper:
+        """"""
+    async def start(self) -> None:
+        """"""
+    async def create_queue(self, queue: str) -> QueueUrl:
+        """"""
+    async def delete_queue(self, queue: str) -> None:
+        """"""
+    async def get_queue(self, queue: str) -> QueueUrl:
+        """"""
+    async def delete_message(self) -> None:
+        """"""
     async def _consume(self, queue_url: str, handler: Handler) -> NoReturn: ...
     @property
     def fmt(self) -> str: ...
     def _get_log_context(  # type: ignore[override]
         self, message: Optional[PropanMessage], queue: str
     ) -> Dict[str, Any]: ...
+    @classmethod
+    def _build_message(
+        cls,
+        message: SendableMessage,
+        queue_url: str,
+        *,
+        headers: Optional[Dict[str, str]] = None,
+        delay_seconds: int = 0,  # 0...900
+        message_attributes: Optional[Dict[str, Any]] = None,
+        message_system_attributes: Optional[Dict[str, Any]] = None,
+        # FIFO only
+        deduplication_id: Optional[str] = None,
+        group_id: Optional[str] = None,
+        # broker
+        reply_to: str = "",
+    ) -> Dict[str, Any]: ...
+    async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage: ...
+    def _process_message(
+        self,
+        func: Callable[[PropanMessage], T],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[PropanMessage], T]: ...
+    async def _connect(self, *args: Any, **kwargs: Any) -> AioBaseClient: ...
```

### Comparing `propan-0.1.2.6/propan/cli/app.py` & `propan-0.1.2.7/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/main.py` & `propan-0.1.2.7/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/core.py` & `propan-0.1.2.7/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.7/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/supervisors/basereload.py` & `propan-0.1.2.7/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.7/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/supervisors/utils.py` & `propan-0.1.2.7/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.7/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/utils/imports.py` & `propan-0.1.2.7/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/utils/logs.py` & `propan-0.1.2.7/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/cli/utils/parser.py` & `propan-0.1.2.7/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/__init__.py` & `propan-0.1.2.7/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/core/route.py` & `propan-0.1.2.7/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/core/router.py` & `propan-0.1.2.7/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.7/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/nats/router.pyi` & `propan-0.1.2.7/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.7/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/redis/router.pyi` & `propan-0.1.2.7/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.7/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/log/formatter.py` & `propan-0.1.2.7/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/log/logging.py` & `propan-0.1.2.7/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/__init__.py` & `propan-0.1.2.7/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/kafka.py` & `propan-0.1.2.7/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/nats.py` & `propan-0.1.2.7/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/rabbit.py` & `propan-0.1.2.7/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/redis.py` & `propan-0.1.2.7/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/test/sqs.py` & `propan-0.1.2.7/propan/test/sqs.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,47 +7,45 @@
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
 from propan import SQSBroker
+from propan.brokers.sqs import SQSMessage
 from propan.test.utils import call_handler
 from propan.types import SendableMessage
 
 __all__ = (
     "build_message",
     "TestSQSBroker",
 )
 
 
 def build_message(
     message: SendableMessage,
-    queue: str,
+    queue: str = "",
     headers: Optional[Dict[str, str]] = None,
     delay_seconds: int = 0,  # 0...900
     message_attributes: Optional[Dict[str, Any]] = None,
     message_system_attributes: Optional[Dict[str, Any]] = None,
     # FIFO only
     deduplication_id: Optional[str] = None,
     group_id: Optional[str] = None,
-    *,
     reply_to: str = "",
 ) -> Dict[str, Any]:
-    params = SQSBroker._build_message(
+    params = SQSMessage(
         message=message,
-        queue_url=queue,
-        headers=headers,
         delay_seconds=delay_seconds,
-        message_attributes=message_attributes,
-        message_system_attributes=message_system_attributes,
+        headers=headers or {},
+        message_attributes=message_attributes or {},
+        message_system_attributes=message_system_attributes or {},
         deduplication_id=deduplication_id,
         group_id=group_id,
-        reply_to=reply_to,
-    )
+    ).to_params(reply_to=reply_to)
 
     body = params.get("MessageBody", "0")
     attributes = params.get("MessageAttributes", {})
 
     return {
         "Body": body,
         "MD5OfBody": md5(body.encode()).hexdigest(),
@@ -74,15 +72,14 @@
     reply_to: str = "",
     callback: bool = False,
     callback_timeout: Optional[float] = None,
     raise_timeout: bool = False,
 ) -> Any:
     incoming = build_message(
         message=message,
-        queue=queue,
         headers=headers,
         delay_seconds=delay_seconds,
         message_attributes=message_attributes,
         message_system_attributes=message_system_attributes,
         deduplication_id=deduplication_id,
         group_id=group_id,
         reply_to=reply_to,
```

### Comparing `propan-0.1.2.6/propan/test/utils.py` & `propan-0.1.2.7/propan/test/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 async def call_handler(
     handler: BaseHandler,
     message: Any,
     callback: bool = False,
     callback_timeout: Optional[float] = 30.0,
     raise_timeout: bool = False,
 ) -> Any:
-    r = handler.callback(message)
     try:
-        result = await asyncio.wait_for(r, timeout=callback_timeout)
+        result = await asyncio.wait_for(
+            handler.callback(message), timeout=callback_timeout
+        )
     except asyncio.TimeoutError as e:
         if raise_timeout is True:  # pragma: no branch
             raise e
         result = None
 
     if callback is True:  # pragma: no branch
         return result
```

### Comparing `propan-0.1.2.6/propan/utils/functions.py` & `propan-0.1.2.7/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/utils/context/main.py` & `propan-0.1.2.7/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/propan/utils/context/types.py` & `propan-0.1.2.7/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/LICENSE` & `propan-0.1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/README.md` & `propan-0.1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/pyproject.toml` & `propan-0.1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.6/PKG-INFO` & `propan-0.1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.6
+Version: 0.1.2.7
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.6 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.7 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```


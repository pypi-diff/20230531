# Comparing `tmp/propan-0.1.2.5.tar.gz` & `tmp/propan-0.1.2.6.tar.gz`

## Comparing `propan-0.1.2.5.tar` & `propan-0.1.2.6.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.5/SECURITY.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/sqs/1_basic.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__about__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__main__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/logging.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/nats.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/sqs.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/test.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.5/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.5/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.5/README.md
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.5/pyproject.toml
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.6/SECURITY.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.6/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__about__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/__main__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/py.typed
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/sqs.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.6/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.6/scripts/test.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.6/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.6/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.6/README.md
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.6/PKG-INFO
```

### Comparing `propan-0.1.2.5/CONTRIBUTING.md` & `propan-0.1.2.6/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 ### pip
 
 After activating the environment as described above:
 
 ```bash
-$ pip install -e ."[dev]"
+$ pip install -e ".[dev]"
 ```
 
 It will install all the dependencies and your local Propan in your local environment.
 
 #### Using your local Propan
 
 If you create a Python file that imports and uses Propan, and run it with the Python from your local environment, it will use your local Propan source code.
```

### Comparing `propan-0.1.2.5/SECURITY.md` & `propan-0.1.2.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/.github/workflows/documentation.yml` & `propan-0.1.2.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/.github/workflows/publish_coverage.yml` & `propan-0.1.2.6/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/.github/workflows/publish_pypi.yml` & `propan-0.1.2.6/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/.github/workflows/tests.yml` & `propan-0.1.2.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/3_lifespan_events.py` & `propan-0.1.2.6/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.6/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/5_publishing.py` & `propan-0.1.2.6/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/6_arguments_casting.py` & `propan-0.1.2.6/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/7_handler_errors_processing.py` & `propan-0.1.2.6/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.6/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.6/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.6/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.6/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.6/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/dependencies/7_annotated.py` & `propan-0.1.2.6/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.6/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/rabbit/direct.py` & `propan-0.1.2.6/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/rabbit/fanout.py` & `propan-0.1.2.6/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/rabbit/header.py` & `propan-0.1.2.6/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/rabbit/topic.py` & `propan-0.1.2.6/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/redis/direct.py` & `propan-0.1.2.6/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/examples/redis/pattern.py` & `propan-0.1.2.6/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/__init__.py` & `propan-0.1.2.6/propan/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Imports to use at __all__
-from propan.__about__ import INSTALL_MESSAGE
+from propan import __about__ as about
 from propan.cli.app import *  # noqa: F403
 from propan.log import *  # noqa: F403
 from propan.utils import *  # noqa: F403
 
 try:
     from propan.brokers.rabbit import RabbitBroker
 except Exception:
-    RabbitBroker = None  # type: ignore
+    RabbitBroker = about.INSTALL_RABBIT  # type: ignore
 
 try:
     from propan.brokers.nats import NatsBroker
 except Exception:
-    NatsBroker = None  # type: ignore
+    NatsBroker = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.brokers.redis import RedisBroker
 except Exception:
-    RedisBroker = None  # type: ignore
+    RedisBroker = about.INSTALL_REDIS  # type: ignore
 
 try:
     from propan.brokers.kafka import KafkaBroker
 except Exception:
-    KafkaBroker = None  # type: ignore
+    KafkaBroker = about.INSTALL_KAFKA  # type: ignore
 
 try:
     from propan.brokers.sqs import SQSBroker
 except Exception:
-    SQSBroker = None  # type: ignore
+    SQSBroker = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitBroker, NatsBroker, RedisBroker, SQSBroker, KafkaBroker)
-), INSTALL_MESSAGE
+), about.INSTALL_MESSAGE
 
 __all__ = (  # noqa: F405
     # app
     "PropanApp",
     # log
     "logger",
     "access_logger",
```

### Comparing `propan-0.1.2.5/propan/annotations.py` & `propan-0.1.2.6/propan/annotations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from typing_extensions import Annotated
 
-from propan.__about__ import INSTALL_MESSAGE
+from propan import __about__ as about
 from propan.cli.app import PropanApp
 from propan.utils.context import Context as ContextField
 from propan.utils.context import ContextRepo as CR
 
 Logger = Annotated[logging.Logger, ContextField("logger")]
 App = Annotated[PropanApp, ContextField("app")]
 ContextRepo = Annotated[CR, ContextField("context")]
@@ -19,66 +19,66 @@
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
     RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
     Channel = Annotated[
         aio_pika.robust_channel.RobustChannel, ContextField("broker._channel")
     ]
 except Exception:
-    RabbitBroker = RabbitMessage = Channel = None  # type: ignore
+    RabbitBroker = RabbitMessage = Channel = about.INSTALL_RABBIT
 
 
 try:
     from nats.aio.msg import Msg
 
     from propan.brokers.nats import NatsBroker as NB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
 except Exception:
-    NatsBroker = NatsMessage = None  # type: ignore
+    NatsBroker = NatsMessage = about.INSTALL_NATS
 
 
 try:
     from redis.asyncio.client import Redis as R
 
     from propan.brokers.redis import RedisBroker as RedB
 
     RedisBroker = Annotated[RedB, ContextField("broker")]
     Redis = Annotated[R, ContextField("broker._connection")]
 except Exception:
-    RedisBroker = Redis = None  # type: ignore
+    RedisBroker = Redis = about.INSTALL_REDIS
 
 
 try:
     from aiokafka import AIOKafkaProducer
     from aiokafka.structs import ConsumerRecord
 
     from propan.brokers.kafka import KafkaBroker as KB
 
     KafkaBroker = Annotated[KB, ContextField("broker")]
     KafkaMessage = Annotated[ConsumerRecord, ContextField("message")]
     Producer = Annotated[AIOKafkaProducer, ContextField("producer")]
 except Exception:
-    KafkaBroker = KafkaMessage = None  # type: ignore
+    KafkaBroker = KafkaMessage = about.INSTALL_KAFKA
 
 
 try:
     from aiobotocore.client import AioBaseClient
 
     from propan.brokers.sqs import SQSBroker as SB
 
     SQSBroker = Annotated[SB, ContextField("broker")]
     client = Annotated[AioBaseClient, ContextField("client")]
     queue_url = Annotated[str, ContextField("queue_url")]
 except Exception:
-    SQSBroker = client = queue_url = None  # type: ignore
+    SQSBroker = client = queue_url = about.INSTALL_SQS
 
 
 assert any(
     (
         all((RabbitBroker, RabbitMessage, Channel)),
         all((NatsBroker, NatsMessage)),
         all((RedisBroker, Redis)),
         all((KafkaBroker, KafkaMessage, Producer)),
         all((SQSBroker, client, queue_url)),
     )
-), INSTALL_MESSAGE
+), about.INSTALL_MESSAGE
```

### Comparing `propan-0.1.2.5/propan/types.py` & `propan-0.1.2.6/propan/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,33 @@
 AnyCallable: TypeAlias = Callable[..., Any]
 NoneCallable: TypeAlias = Callable[..., None]
 
 DecoratedCallable: TypeAlias = AnyCallable
 DecoratedCallableNone: TypeAlias = NoneCallable
 DecoratedAsync: TypeAlias = AsyncFunc
 
-Wrapper: TypeAlias = Callable[[AnyCallable], DecoratedCallable]
-AsyncWrapper: TypeAlias = Callable[[AnyCallable], DecoratedAsync]
-DecodedMessage: TypeAlias = Union[AnyDict, Sequence[Any], str, bytes]
-SendableMessage: TypeAlias = Union[DecodedMessage, BaseModel, None]
+Wrapper: TypeAlias = Callable[
+    [AnyCallable],
+    DecoratedCallable,
+]
+AsyncWrapper: TypeAlias = Callable[
+    [AnyCallable],
+    DecoratedAsync,
+]
+DecodedMessage: TypeAlias = Union[
+    AnyDict,
+    Sequence[Any],
+    str,
+    bytes,
+]
+SendableMessage: TypeAlias = Union[
+    DecodedMessage,
+    BaseModel,
+    None,
+]
 
 HandlerCallable: TypeAlias = Callable[
     ...,
     Union[Awaitable[SendableMessage], SendableMessage],
 ]
 HandlerWrapper: TypeAlias = Callable[
     [HandlerCallable],
```

### Comparing `propan-0.1.2.5/propan/brokers/push_back_watcher.py` & `propan-0.1.2.6/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.6/propan/brokers/_model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
+from typing_extensions import Self
+
 from propan.brokers._model.schemas import (
     ContentType,
     ContentTypes,
     PropanMessage,
     SendableModel,
 )
 from propan.brokers._model.utils import (
@@ -27,15 +29,14 @@
     SendableMessage,
     Wrapper,
 )
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
 T = TypeVar("T")
-Cls = TypeVar("Cls", bound="BrokerUsecase")
 
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: List[Any]
     _connection: Any
@@ -81,43 +82,48 @@
         message: SendableMessage,
         *args: Any,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
         **kwargs: Any,
-    ) -> Any:
+    ) -> Optional[DecodedMessage]:
         raise NotImplementedError()
 
     @abstractmethod
     async def close(self) -> None:
         raise NotImplementedError()
 
     @abstractmethod
     async def _parse_message(self, message: Any) -> PropanMessage:
         raise NotImplementedError()
 
     @abstractmethod
     def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
+        self,
+        func: Callable[[PropanMessage], T],
+        watcher: Optional[BaseWatcher],
     ) -> Callable[[PropanMessage], T]:
         raise NotImplementedError()
 
     def _get_log_context(
-        self, message: Optional[PropanMessage], **kwargs: Dict[str, str]
+        self,
+        message: Optional[PropanMessage],
+        **kwargs: Dict[str, str],
     ) -> Dict[str, Any]:
         return {
             "message_id": message.message_id[:10] if message else "",
         }
 
     @abstractmethod
     def handle(
         self,
         *broker_args: Any,
         retry: Union[bool, int] = False,
+        _raw: bool = False,
         **broker_kwargs: Any,
     ) -> HandlerWrapper:
         raise NotImplementedError()
 
     @staticmethod
     async def _decode_message(message: PropanMessage) -> DecodedMessage:
         body = message.body
@@ -139,33 +145,34 @@
 
     async def start(self) -> None:
         if self.logger is not None:
             change_logger_handlers(self.logger, self.fmt)
 
         await self.connect()
 
-    async def __aenter__(self: Cls) -> Cls:
+    async def __aenter__(self) -> Self:
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.close()
 
     def _wrap_handler(
         self,
         func: AnyCallable,
         retry: Union[bool, int] = False,
+        _raw: bool = False,
         **broker_args: Any,
     ) -> DecoratedAsync:
         f = to_async(func)
 
         if self._is_apply_types is True:
             f = apply_types(f)
 
-        f = self._wrap_decode_message(f)
+        f = self._wrap_decode_message(f, _raw=_raw)
 
         if self.logger is not None:
             f = self._log_execution(**broker_args)(f)
 
         f = self._process_message(f, get_watcher(self.logger, retry))
 
         f = self._wrap_parse_message(f)
@@ -173,19 +180,29 @@
         f = set_message_context(f)
 
         f = suppress_decor(f)
 
         return f
 
     def _wrap_decode_message(
-        self, func: Callable[..., Awaitable[T]]
+        self,
+        func: Callable[..., Awaitable[T]],
+        _raw: bool = False,
     ) -> Callable[[PropanMessage], Awaitable[T]]:
+        decode: Callable[
+            [PropanMessage], Awaitable[Union[PropanMessage, DecodedMessage]]
+        ]
+        if _raw is True:
+            decode = _fake_decode
+        else:
+            decode = self._decode_message
+
         @wraps(func)
         async def wrapper(message: PropanMessage) -> T:
-            return await func(await self._decode_message(message))
+            return await func(await decode(message))
 
         return wrapper
 
     def _wrap_parse_message(
         self, func: Callable[[PropanMessage], Awaitable[T]]
     ) -> Callable[[Any], Awaitable[T]]:
         @wraps(func)
@@ -227,7 +244,11 @@
         log_level: Optional[int] = None,
         extra: Optional[AnyDict] = None,
     ) -> None:
         if self.logger is not None:
             self.logger.log(
                 level=(log_level or self.log_level), msg=message, extra=extra
             )
+
+
+async def _fake_decode(message: PropanMessage) -> PropanMessage:
+    return message
```

### Comparing `propan-0.1.2.5/propan/brokers/_model/schemas.py` & `propan-0.1.2.6/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/_model/utils.py` & `propan-0.1.2.6/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.6/propan/brokers/kafka/kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,22 @@
         if self._publisher is not None:
             await self._publisher.stop()
             self._publisher = None
 
     def handle(
         self,
         *topics: str,
+        _raw: bool = False,
         **kwargs: AnyDict,
     ) -> Wrapper:
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             for t in topics:
                 self.__max_topic_len = max((self.__max_topic_len, len(t)))
 
-            func = self._wrap_handler(func)
+            func = self._wrap_handler(func, _raw=_raw)
             handler = Handler(
                 callback=func,
                 topics=topics,
                 consumer_kwargs=kwargs,
             )
             self.handlers.append(handler)
```

### Comparing `propan-0.1.2.5/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.6/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.6/propan/brokers/nats/nats_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 import logging
 from functools import wraps
 from secrets import token_hex
-from typing import Any, Callable, Dict, List, Optional, TypeVar
+from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
 
 import nats
 from nats.aio.client import Callback, Client, ErrorCallback
 from nats.aio.msg import Msg
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.types import AnyDict, DecoratedCallable, SendableMessage
+from propan.types import AnyDict, DecodedMessage, DecoratedCallable, SendableMessage
 from propan.utils import context
 
 T = TypeVar("T")
 
 
 class NatsBroker(BrokerUsecase):
     handlers: List[Handler]
@@ -52,22 +52,28 @@
             **kwargs,
         )
 
     def handle(
         self,
         subject: str,
         queue: str = "",
-        **original_kwargs,
+        *,
+        retry: Union[bool, int] = False,
+        _raw: bool = False,
     ) -> Callable[[DecoratedCallable], None]:
         self.__max_subject_len = max((self.__max_subject_len, len(subject)))
         self.__max_queue_len = max((self.__max_queue_len, len(queue)))
 
         def wrapper(func: DecoratedCallable) -> None:
             func = self._wrap_handler(
-                func, queue=queue, subject=subject, **original_kwargs
+                func,
+                queue=queue,
+                subject=subject,
+                retry=retry,
+                _raw=_raw,
             )
             handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
@@ -95,15 +101,15 @@
         subject: str,
         *,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-    ) -> None:
+    ) -> Optional[DecodedMessage]:
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
         msg, content_type = self._encode_message(message)
 
         client = self._connection
```

### Comparing `propan-0.1.2.5/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.6/propan/brokers/nats/nats_broker.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from nats.aio.msg import Msg
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
-from propan.types import HandlerWrapper, SendableMessage
+from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 
 class NatsBroker(BrokerUsecase):
     logger: logging.Logger
     handlers: List[Handler]
     _connection: Optional[Client]
@@ -114,23 +114,22 @@
         subject: str,
         *,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-    ) -> None: ...
+    ) -> Optional[DecodedMessage]: ...
     def handle(  # type: ignore[override]
         self,
         subject: str,
         queue: str = "",
         *,
         retry: Union[bool, int] = False,
     ) -> HandlerWrapper: ...
-    async def __aenter__(self) -> "NatsBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
     async def close(self) -> None: ...
     def _get_log_context(  # type: ignore[override]
         self,
         message: Optional[PropanMessage],
         subject: str,
         queue: str = "",
```

### Comparing `propan-0.1.2.5/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.6/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/nats/schemas.py` & `propan-0.1.2.6/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.6/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,25 +73,27 @@
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         retry: Union[bool, int] = False,
+        _raw: bool = False,
     ) -> HandlerWrapper:
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
             func = self._wrap_handler(
                 func,
                 queue=queue,
                 exchange=exchange,
                 retry=retry,
+                _raw=_raw,
             )
             handler = Handler(callback=func, queue=queue, exchange=exchange)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
```

### Comparing `propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.6/propan/brokers/redis/redis_broker.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,175 @@
 import logging
-from ssl import SSLContext
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Callable, Dict, List, Mapping, Optional, Type, TypeVar, Union
 
-import aio_pika
-import aiormq
-from pamqp.common import FieldTable
-from typing_extensions import ParamSpec
-from yarl import URL
+from redis.asyncio.client import Redis
+from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
+from propan.brokers.redis.schemas import Handler
 from propan.log import access_logger
-from propan.types import SendableMessage
+from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
-P = ParamSpec("P")
 T = TypeVar("T")
-PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 
-class RabbitBroker(BrokerUsecase):
+class RedisBroker(BrokerUsecase):
     handlers: List[Handler]
-    _connection: Optional[aio_pika.RobustConnection]
-    _channel: Optional[aio_pika.RobustChannel]
-
-    __max_queue_len: int
-    __max_exchange_len: int
+    _connection: Redis[bytes]
+    __max_channel_len: int
 
     def __init__(
         self,
-        url: Union[str, URL, None] = None,
-        host: str = "localhost",
-        port: int = 5672,
-        login: str = "guest",
-        password: str = "guest",
-        virtualhost: str = "/",
-        ssl: bool = False,
-        ssl_options: Optional[aio_pika.abc.SSLOptions] = None,
-        ssl_context: Optional[SSLContext] = None,
-        timeout: aio_pika.abc.TimeoutType = None,
-        client_properties: Optional[FieldTable] = None,
+        url: str = "redis://localhost:6379",
+        polling_interval: float = 1.0,
         *,
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        db: Union[str, int] = 0,
+        client_name: Optional[str] = None,
+        health_check_interval: float = 0,
+        max_connections: Optional[int] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_read_size: int = 65536,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        connection_class: Type[Connection] = Connection,
+        encoder_class: Type[Encoder] = Encoder,
+        # broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        consumers: Optional[int] = None,
     ) -> None:
-        """
-        URL string might be contain ssl parameters e.g.
-        `amqps://user:pass@host//?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
+        """Redis Pub/sub Propan broker
 
-        :param client_properties: add custom client capability.
-        :param url:
-            RFC3986_ formatted broker address. When :class:`None`
-            will be used keyword arguments.
-        :param host: hostname of the broker
-        :param port: broker port 5672 by default
-        :param login: username string. `'guest'` by default.
-        :param password: password string. `'guest'` by default.
-        :param virtualhost: virtualhost parameter. `'/'` by default
-        :param ssl: use SSL for connection. Should be used with addition kwargs.
-        :param ssl_options: A dict of values for the SSL connection.
-        :param timeout: connection timeout in seconds
-        :param ssl_context: ssl.SSLContext instance
+        URL examples:
 
-        .. _RFC3986: https://goo.gl/MzgYAs
-        .. _official Python documentation: https://goo.gl/pty9xA
+        - redis://[[username]:[password]]@localhost:6379/0
+        - rediss://[[username]:[password]]@localhost:6379/0
+        - unix://[username@]/path/to/socket.sock?db=0[&password=password]
+
+        Three URL schemes are supported:
+
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - `unix://`: creates a Unix Domain Socket connection.
+
+        Url will be parsed to kwargs and partially replaced by keywords arguments if they specified.
         """
-        ...
     async def connect(
         self,
-        url: Union[str, URL, None] = None,
+        url: str = "redis://localhost:6379",
         host: str = "localhost",
-        port: int = 5672,
-        login: str = "guest",
-        password: str = "guest",
-        virtualhost: str = "/",
-        ssl: bool = False,
-        ssl_options: Optional[aio_pika.abc.SSLOptions] = None,
-        ssl_context: Optional[SSLContext] = None,
-        timeout: aio_pika.abc.TimeoutType = None,
-        client_properties: Optional[FieldTable] = None,
-    ) -> aio_pika.Connection:
-        """
-        URL string might be contain ssl parameters e.g.
-        `amqps://user:pass@host//?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
-
-        :param client_properties: add custom client capability.
-        :param url:
-            RFC3986_ formatted broker address. When :class:`None`
-            will be used keyword arguments.
-        :param host: hostname of the broker
-        :param port: broker port 5672 by default
-        :param login: username string. `'guest'` by default.
-        :param password: password string. `'guest'` by default.
-        :param virtualhost: virtualhost parameter. `'/'` by default
-        :param ssl: use SSL for connection. Should be used with addition kwargs.
-        :param ssl_options: A dict of values for the SSL connection.
-        :param timeout: connection timeout in seconds
-        :param ssl_context: ssl.SSLContext instance
+        port: Union[str, int] = 6379,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        db: Union[str, int] = 0,
+        client_name: Optional[str] = None,
+        health_check_interval: float = 0,
+        max_connections: Optional[int] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_read_size: int = 65536,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type[BaseParser] = DefaultParser,
+        connection_class: Type[Connection] = Connection,
+        encoder_class: Type[Encoder] = Encoder,
+    ) -> Redis[bytes]:
+        """Connect to Redis
+
+        URL examples:
+
+        - redis://[[username]:[password]]@localhost:6379/0
+        - rediss://[[username]:[password]]@localhost:6379/0
+        - unix://[username@]/path/to/socket.sock?db=0[&password=password]
+
+        Three URL schemes are supported:
+
+        - `redis://` creates a TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/redis>
+        - `rediss://` creates a SSL wrapped TCP socket connection. See more at:
+          <https://www.iana.org/assignments/uri-schemes/prov/rediss>
+        - `unix://`: creates a Unix Domain Socket connection.
+
+        Url will be parsed to kwargs and partially replaced by keywords arguments if they specified.
+        """
+    async def _connect(self, *args: Any, **kwargs: Any) -> Redis[bytes]: ...
+    async def start(self) -> None:
+        """Initialize Redis connection and startup all consumers"""
+    async def close(self) -> None:
+        """Cancel all consumers tasks and subscribtions, close Redis connection"""
+    def handle(  # type: ignore[override]
+        self,
+        channel: str,
+        *,
+        pattern: bool = False,
+    ) -> HandlerWrapper:
+        """Register channel consumer method
+
+        Args:
+            channel: channel to consume messages
+            pattern: use psubscribe or subscribe method
 
-        .. _RFC3986: https://goo.gl/MzgYAs
-        .. _official Python documentation: https://goo.gl/pty9xA
+        Returns:
+            Async or sync function decorator
         """
-        ...
     async def publish(  # type: ignore[override]
         self,
-        message: PikaSendableMessage = "",
-        queue: Union[RabbitQueue, str] = "",
-        exchange: Union[RabbitExchange, str, None] = None,
+        message: SendableMessage = "",
+        channel: str = "",
         *,
-        # publish kwargs
-        routing_key: str = "",
-        mandatory: bool = True,
-        immediate: bool = False,
-        timeout: aio_pika.abc.TimeoutType = None,
-        # callback kwargs
+        reply_to: str = "",
+        headers: Optional[Dict[str, Any]] = None,
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-        # message kwargs
-        headers: Optional[aio_pika.abc.HeadersType] = None,
-        content_type: Optional[str] = None,
-        content_encoding: Optional[str] = None,
-        persist: bool = False,
-        priority: Optional[int] = None,
-        correlation_id: Optional[str] = None,
-        reply_to: Optional[str] = None,
-        expiration: Optional[aio_pika.abc.DateType] = None,
-        message_id: Optional[str] = None,
-        timestamp: Optional[aio_pika.abc.DateType] = None,
-        type: Optional[str] = None,
-        user_id: Optional[str] = None,
-        app_id: Optional[str] = None,
-    ) -> Optional[aiormq.abc.ConfirmationFrameType]: ...
-    def handle(  # type: ignore[override]
-        self,
-        queue: Union[str, RabbitQueue],
-        exchange: Union[str, RabbitExchange, None] = None,
-        *,
-        retry: Union[bool, int] = False,
-    ) -> Callable[
-        [
-            Callable[
-                P, Union[PikaSendableMessage, Coroutine[Any, Any, PikaSendableMessage]]
-            ]
-        ],
-        Callable[P, PikaSendableMessage],
-    ]:
-        """
-        retry: Union[bool, int] - at exeption message will returns to queue `int` times or endless if `True`
+    ) -> Optional[DecodedMessage]:
+        """Publish the message to the channel.
+
+        Args:
+            message: encodable message to send
+            channel: channel to publish message
+            reply_to: queue to send response
+            headers: message headers (for consumers)
+            callback: wait for response
+            callback_timeout: response waiting time
+            raise_timeout: if False timeout returns None instead asyncio.TimeoutError
+
+        Returns:
+            `None` if you are not waiting for response
+            (reply_to and callback are not specified)
+
+            `DecodedMessage` | `None` if response is expected
         """
-        ...
-    async def __aenter__(self) -> "RabbitBroker": ...
-    async def _connect(
-        self,
-        *args: Any,
-        **kwargs: Any,
-    ) -> aio_pika.RobustConnection: ...
-    async def close(self) -> None: ...
-    def _process_message(
-        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
-    ) -> Callable[[PropanMessage], T]: ...
     def _get_log_context(  # type: ignore[override]
-        self,
-        message: Optional[PropanMessage],
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange] = None,
+        self, message: Optional[PropanMessage], channel: str
     ) -> Dict[str, Any]: ...
-    async def _init_handler(
-        self,
-        handler: Handler,
-    ) -> aio_pika.abc.AbstractRobustQueue: ...
-    async def _init_queue(
-        self,
-        queue: RabbitQueue,
-    ) -> aio_pika.abc.AbstractRobustQueue: ...
-    async def _init_exchange(
-        self,
-        exchange: RabbitExchange,
-    ) -> aio_pika.abc.AbstractRobustExchange: ...
-    async def start(self) -> None: ...
-    @classmethod
-    def _validate_message(
-        cls: Type["RabbitBroker"],
-        message: PikaSendableMessage,
-        callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
-        **message_kwargs: Dict[str, Any],
-    ) -> aio_pika.Message: ...
     @staticmethod
-    async def _parse_message(
-        message: aio_pika.message.IncomingMessage,
-    ) -> PropanMessage: ...
+    async def _decode_message(message: PropanMessage) -> DecodedMessage: ...
+    @staticmethod
+    async def _parse_message(message: Any) -> PropanMessage: ...
+    def _process_message(
+        self,
+        func: Callable[[PropanMessage], T],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[PropanMessage], T]: ...
+    @property
+    def fmt(self) -> str: ...
```

### Comparing `propan-0.1.2.5/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.6/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.6/propan/brokers/redis/redis_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,21 +94,23 @@
         return wrapper
 
     def handle(
         self,
         channel: str = "",
         *,
         pattern: bool = False,
+        _raw: bool = False,
     ) -> HandlerWrapper:
         self.__max_channel_len = max(self.__max_channel_len, len(channel))
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             func = self._wrap_handler(
                 func,
                 channel=channel,
+                _raw=_raw,
             )
             handler = Handler(callback=func, channel=channel, pattern=pattern)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
@@ -140,15 +142,15 @@
         channel: str = "",
         *,
         reply_to: str = "",
         headers: Optional[Dict[str, Any]] = None,
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
-    ) -> None:
+    ) -> Optional[DecodedMessage]:
         if self._connection is None:
             raise ValueError("Redis connection not established yet")
 
         msg, content_type = self._encode_message(message)
 
         if callback is True:
             callback_channel = str(uuid4())
```

### Comparing `propan-0.1.2.5/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.6/propan/fastapi/core/router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,141 @@
-import logging
-from typing import Any, Callable, Dict, List, Mapping, Optional, Type, TypeVar, Union
+from contextlib import asynccontextmanager
+from enum import Enum
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
-from redis.asyncio.client import Redis
-from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
+from fastapi import APIRouter, FastAPI, params
+from fastapi.datastructures import Default
+from fastapi.routing import APIRoute
+from fastapi.types import DecoratedCallable
+from fastapi.utils import generate_unique_id
+from starlette import routing
+from starlette.responses import JSONResponse, Response
+from starlette.routing import _DefaultLifespan
+from starlette.types import ASGIApp, Lifespan
+from typing_extensions import AsyncIterator, TypeVar
 
 from propan.brokers._model import BrokerUsecase
-from propan.brokers._model.schemas import PropanMessage
-from propan.brokers.push_back_watcher import BaseWatcher
-from propan.brokers.redis.schemas import Handler
-from propan.log import access_logger
-from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
-
-T = TypeVar("T")
-
-class RedisBroker(BrokerUsecase):
-    handlers: List[Handler]
-    _connection: Redis[bytes]
-    __max_channel_len: int
+from propan.fastapi.core.route import PropanRoute
+from propan.types import AnyDict
+
+Broker = TypeVar("Broker", bound=BrokerUsecase)
+
+
+class PropanRouter(APIRouter, Generic[Broker]):
+    broker_class: Type[Broker]
+    broker: Broker
 
     def __init__(
         self,
-        url: str = "redis://localhost:6379",
-        polling_interval: float = 1.0,
-        *,
-        connection_class: Type[Connection] = Connection,
-        max_connections: Optional[int] = None,
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
-        db: Union[str, int] = 0,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        socket_keepalive: bool = False,
-        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
-        socket_type: int = 0,
-        retry_on_timeout: bool = False,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        parser_class: Type[BaseParser] = DefaultParser,
-        socket_read_size: int = 65536,
-        health_check_interval: float = 0,
-        client_name: Optional[str] = None,
-        username: Optional[str] = None,
-        encoder_class: Type[Encoder] = Encoder,
-        # broker kwargs
-        logger: Optional[logging.Logger] = access_logger,
-        log_level: int = logging.INFO,
-        log_fmt: Optional[str] = None,
-        apply_types: bool = True,
-    ) -> None: ...
-    async def connect(
-        self,
-        url: str = "redis://localhost:6379",
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
-        db: Union[str, int] = 0,
-        password: Optional[str] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
-        socket_keepalive: bool = False,
-        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
-        socket_type: int = 0,
-        retry_on_timeout: bool = False,
-        encoding: str = "utf-8",
-        encoding_errors: str = "strict",
-        decode_responses: bool = False,
-        parser_class: Type[BaseParser] = DefaultParser,
-        socket_read_size: int = 65536,
-        health_check_interval: float = 0,
-        client_name: Optional[str] = None,
-        username: Optional[str] = None,
-        encoder_class: Type[Encoder] = Encoder,
-    ) -> Redis[bytes]: ...
-    async def _connect(self, *args: Any, **kwargs: Any) -> Redis[bytes]: ...
-    async def close(self) -> None: ...
-    @staticmethod
-    async def _parse_message(message: Any) -> PropanMessage: ...
-    def _process_message(
-        self,
-        func: Callable[[PropanMessage], T],
-        watcher: Optional[BaseWatcher],
-    ) -> Callable[[PropanMessage], T]: ...
-    def handle(  # type: ignore[override]
+        *connection_args: Tuple[Any, ...],
+        prefix: str = "",
+        tags: Optional[List[Union[str, Enum]]] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
+        default_response_class: Type[Response] = Default(JSONResponse),
+        responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
+        callbacks: Optional[List[routing.BaseRoute]] = None,
+        routes: Optional[List[routing.BaseRoute]] = None,
+        redirect_slashes: bool = True,
+        default: Optional[ASGIApp] = None,
+        dependency_overrides_provider: Optional[Any] = None,
+        route_class: Type[APIRoute] = APIRoute,
+        on_startup: Optional[Sequence[Callable[[], Any]]] = None,
+        on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
+        deprecated: Optional[bool] = None,
+        include_in_schema: bool = True,
+        lifespan: Optional[Lifespan[Any]] = None,
+        generate_unique_id_function: Callable[[APIRoute], str] = Default(
+            generate_unique_id
+        ),
+        **connection_kwars: AnyDict,
+    ) -> None:
+        assert (
+            self.broker_class
+        ), "You should specify `broker_class` at your implementation"
+
+        self.broker = self.broker_class(
+            *connection_args,
+            apply_types=False,
+            **connection_kwars,  # type: ignore
+        )
+
+        super().__init__(
+            prefix=prefix,
+            tags=tags,
+            dependencies=dependencies,
+            default_response_class=default_response_class,
+            responses=responses,
+            callbacks=callbacks,
+            routes=routes,
+            redirect_slashes=redirect_slashes,
+            default=default,
+            dependency_overrides_provider=dependency_overrides_provider,
+            route_class=route_class,
+            deprecated=deprecated,
+            include_in_schema=include_in_schema,
+            generate_unique_id_function=generate_unique_id_function,
+            lifespan=self._wrap_lifespan(lifespan),
+            on_startup=on_startup,
+            on_shutdown=on_shutdown,
+        )
+
+    def add_api_mq_route(
         self,
-        channel: str,
+        path: str,
         *,
-        pattern: bool = False,
-    ) -> HandlerWrapper: ...
-    def _get_log_context(  # type: ignore[override]
-        self, message: Optional[PropanMessage], channel: str
-    ) -> Dict[str, Any]: ...
-    @staticmethod
-    async def _decode_message(message: PropanMessage) -> DecodedMessage: ...
-    @property
-    def fmt(self) -> str: ...
-    async def start(self) -> None: ...
-    async def publish(  # type: ignore[override]
+        endpoint: Callable[..., Any],
+        **broker_kwargs: AnyDict,
+    ) -> None:
+        route = PropanRoute(
+            path,
+            endpoint=endpoint,
+            dependency_overrides_provider=self.dependency_overrides_provider,
+            broker=self.broker,
+            **broker_kwargs,
+        )
+        self.routes.append(route)
+
+    def event(
         self,
-        message: SendableMessage = "",
-        channel: str = "",
-        *,
-        reply_to: str = "",
-        headers: Optional[Dict[str, Any]] = None,
-        callback: bool = False,
-        callback_timeout: Optional[float] = 30.0,
-        raise_timeout: bool = False,
-    ) -> None: ...
+        path: str,
+        **broker_kwargs: Dict[str, Any],
+    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        def decorator(func: DecoratedCallable) -> DecoratedCallable:
+            self.add_api_mq_route(
+                path,
+                endpoint=func,
+                **broker_kwargs,
+            )
+            return func
+
+        return decorator
+
+    def _wrap_lifespan(self, lifespan: Optional[Lifespan[Any]] = None) -> Lifespan[Any]:
+        if lifespan is not None:
+            lifespan_context = lifespan
+        else:
+            lifespan_context = _DefaultLifespan(self)
+
+        @asynccontextmanager
+        async def start_broker_lifespan(
+            app: FastAPI,
+        ) -> AsyncIterator[Dict[str, Broker]]:
+            async with lifespan_context(app) as maybe_context:
+                await self.broker.start()
+                context = {"broker": self.broker}
+                if maybe_context:
+                    context.update(maybe_context)
+                yield context
+                await self.broker.close()
+
+        return start_broker_lifespan
```

### Comparing `propan-0.1.2.5/propan/brokers/redis/schemas.py` & `propan-0.1.2.6/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.6/propan/brokers/sqs/sqs_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
+        _raw: bool = False,
     ) -> HandlerWrapper:
         if isinstance(queue, str):
             queue = SQSQueue(queue)
 
         self.__max_queue_len = max((self.__max_queue_len, len(queue.name)))
 
         params = {
@@ -143,15 +144,20 @@
                 *message_attributes,
             ),
         }
         if request_attempt_id is not None:
             params["ReceiveRequestAttemptId"] = request_attempt_id
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
-            func = self._wrap_handler(func, queue=queue.name, retry=retry)
+            func = self._wrap_handler(
+                func,
+                queue=queue.name,
+                retry=retry,
+                _raw=_raw,
+            )
             handler = Handler(callback=func, queue=queue, consumer_params=params)
             self.handlers.append(handler)
             return func
 
         return wrapper
 
     async def start(self) -> None:
@@ -182,15 +188,15 @@
         deduplication_id: Optional[str] = None,
         group_id: Optional[str] = None,
         # broker
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> Any:
+    ) -> None:
         queue_url = await self.get_queue(queue)
 
         params = self._build_message(
             message=message,
             queue_url=queue_url,
             headers=headers,
             delay_seconds=delay_seconds,
@@ -255,17 +261,21 @@
         if url is None:  # pragma: no branch
             url = (
                 await self._connection.create_queue(
                     QueueName=queue.name,
                     Attributes={
                         i: str(j)
                         for i, j in queue.dict(
-                            exclude={"name"}, by_alias=True, exclude_defaults=True
+                            exclude={"name"},
+                            by_alias=True,
+                            exclude_defaults=True,
+                            exclude_unset=True,
                         ).items()
                     },
+                    tags=queue.tags,
                 )
             ).get("QueueUrl", "")
             self._queues[queue.name] = url
         return url
 
     async def delete_queue(self, queue: str) -> None:
         await self._connection.delete_queue(QueueUrl=self.get_queue(queue))
```

### Comparing `propan-0.1.2.5/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.6/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,30 @@
         aws_session_token: Optional[str] = None,
         config: Optional[AioConfig] = None,
         # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-    ) -> None: ...
+    ) -> None:
+        """"""
     async def connect(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
         verify: Optional[bool] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         config: Optional[AioConfig] = None,
-    ) -> AioBaseClient: ...
+    ) -> AioBaseClient:
+        """"""
     async def _connect(self, *args: Any, **kwargs: Any) -> AioBaseClient: ...
     async def close(self) -> None: ...
     async def _parse_message(self, message: Dict[str, Any]) -> PropanMessage: ...
     def _process_message(
         self,
         func: Callable[[PropanMessage], T],
         watcher: Optional[BaseWatcher],
@@ -80,15 +82,15 @@
         message_system_attributes: Optional[Dict[str, Any]] = None,
         deduplication_id: Optional[str] = None,
         group_id: Optional[str] = None,
         reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
-    ) -> Any: ...
+    ) -> None: ...
     @classmethod
     def _build_message(
         cls,
         message: SendableMessage,
         queue_url: str,
         *,
         headers: Optional[Dict[str, str]] = None,
```

### Comparing `propan-0.1.2.5/propan/cli/app.py` & `propan-0.1.2.6/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/main.py` & `propan-0.1.2.6/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/core.py` & `propan-0.1.2.6/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.6/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/supervisors/basereload.py` & `propan-0.1.2.6/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.6/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/supervisors/utils.py` & `propan-0.1.2.6/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.6/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/utils/imports.py` & `propan-0.1.2.6/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/utils/logs.py` & `propan-0.1.2.6/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/cli/utils/parser.py` & `propan-0.1.2.6/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/fastapi/__init__.py` & `propan-0.1.2.6/propan/fastapi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from propan.__about__ import INSTALL_MESSAGE
+from propan import __about__ as about
 
 try:
     from propan.fastapi.rabbit import RabbitRouter
 except Exception:
-    RabbitRouter = None  # type: ignore
+    RabbitRouter = about.INSTALL_RABBIT  # type: ignore
 
 try:
     from propan.fastapi.redis import RedisRouter
 except Exception:
-    RedisRouter = None  # type: ignore
+    RedisRouter = about.INSTALL_REDIS  # type: ignore
 
 try:
     from propan.fastapi.kafka import KafkaRouter
 except Exception:
-    KafkaRouter = None  # type: ignore
+    KafkaRouter = about.INSTALL_KAFKA  # type: ignore
 
 try:
     from propan.fastapi.nats import NatsRouter
 except Exception:
-    NatsRouter = None  # type: ignore
+    NatsRouter = about.INSTALL_NATS  # type: ignore
 
 try:
     from propan.fastapi.sqs import SQSRouter
 except Exception:
-    SQSRouter = None  # type: ignore
+    SQSRouter = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitRouter, RedisRouter, KafkaRouter, NatsRouter, SQSRouter)
-), INSTALL_MESSAGE
+), about.INSTALL_MESSAGE
 
 __all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter", "SQSRouter")
```

### Comparing `propan-0.1.2.5/propan/fastapi/core/route.py` & `propan-0.1.2.6/propan/fastapi/core/route.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from fastapi.dependencies.utils import get_dependant, solve_dependencies
 from fastapi.routing import run_endpoint_function
 from pydantic import ValidationError, create_model
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
 from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage as NativeMessage
 from propan.types import AnyDict
 
-NativeMessage = Union[str, AnyDict, bytes]
-
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
         broker: BrokerUsecase,
@@ -29,15 +28,15 @@
         self.path = path
         self.broker = broker
         self.dependant = get_dependant(path=path, call=endpoint)
 
         handler = PropanMessage.get_session(
             self.dependant, dependency_overrides_provider
         )
-        broker.handle(path, **handle_kwargs)(handler)  # type: ignore
+        broker.handle(path, _raw=True, **handle_kwargs)(handler)  # type: ignore
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
     _headers: AnyDict  # type: ignore
     _body: AnyDict  # type: ignore
@@ -70,19 +69,20 @@
                 lambda i: i in dependencies_names,
                 inspect.signature(dependant.call).parameters,
             ),
             None,
         )
 
         async def app(message: NativeMessage) -> Any:
+            body: Union[AnyDict, bytes] = message.body
             if first_arg is not None:
-                if not isinstance(message, dict):  # pragma: no branch
-                    message = {first_arg: message}
+                if not isinstance(body, dict):  # pragma: no branch
+                    body = {first_arg: body}
 
-                session = cls(message)
+                session = cls(body, message.headers)
             else:
                 session = cls()
             return await func(session)
 
         return app
```

### Comparing `propan-0.1.2.5/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.6/propan/fastapi/kafka/router.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 from propan.__about__ import __version__
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 Partition = TypeVar("Partition")
 
-class KafkaRouter(PropanRouter):
-    broker: KafkaBroker
-
+class KafkaRouter(PropanRouter[KafkaBroker]):
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
         # both
         client_id: str = "propan-" + __version__,
         request_timeout_ms: int = 40 * 1000,
```

### Comparing `propan-0.1.2.5/propan/fastapi/nats/router.pyi` & `propan-0.1.2.6/propan/fastapi/nats/router.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 from starlette.types import ASGIApp
 
 from propan import NatsBroker
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
-class NatsRouter(PropanRouter):
-    broker: NatsBroker
-
+class NatsRouter(PropanRouter[NatsBroker]):
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
         discovered_server_cb: Optional[Callback] = None,
```

### Comparing `propan-0.1.2.5/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.6/propan/fastapi/rabbit/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
 from propan import RabbitBroker
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
-class RabbitRouter(PropanRouter):
-    broker: RabbitBroker
-
+class RabbitRouter(PropanRouter[RabbitBroker]):
     def __init__(
         self,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
         virtualhost: str = "/",
```

### Comparing `propan-0.1.2.5/propan/fastapi/redis/router.pyi` & `propan-0.1.2.6/propan/fastapi/redis/router.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 from starlette.types import ASGIApp
 
 from propan import RedisBroker
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
-class RedisRouter(PropanRouter):
-    broker: RedisBroker
-
+class RedisRouter(PropanRouter[RedisBroker]):
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: float = 1.0,
         host: str = "localhost",
         port: Union[str, int] = 6379,
         db: Union[str, int] = 0,
```

### Comparing `propan-0.1.2.5/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.6/propan/fastapi/sqs/router.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 from propan import SQSBroker
 from propan.brokers.sqs.schema import SQSQueue
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
-class SQSRouter(PropanRouter):
-    broker: SQSBroker
-
+class SQSRouter(PropanRouter[SQSBroker]):
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
```

### Comparing `propan-0.1.2.5/propan/log/formatter.py` & `propan-0.1.2.6/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/log/logging.py` & `propan-0.1.2.6/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/test/__init__.py` & `propan-0.1.2.6/propan/test/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from propan.__about__ import INSTALL_MESSAGE
+from propan import __about__ as about
 
 try:
     from propan.test.rabbit import TestRabbitBroker
 except Exception:
-    TestRabbitBroker = None  # type: ignore
+    TestRabbitBroker = about.INSTALL_RABBIT
 
 try:
     from propan.test.redis import TestRedisBroker
 except Exception:
-    TestRedisBroker = None  # type: ignore
+    TestRedisBroker = about.INSTALL_REDIS
 
 try:
     from propan.test.kafka import TestKafkaBroker
 except Exception:
-    TestKafkaBroker = None  # type: ignore
+    TestKafkaBroker = about.INSTALL_KAFKA
 
 try:
     from propan.test.nats import TestNatsBroker
 except Exception:
-    TestNatsBroker = None  # type: ignore
+    TestNatsBroker = about.INSTALL_NATS
 
 try:
     from propan.test.sqs import TestSQSBroker
 except Exception:
-    TestSQSBroker = None  # type: ignore
+    TestSQSBroker = about.INSTALL_SQS
 
 assert any(
     (TestRabbitBroker, TestRedisBroker, TestKafkaBroker, TestNatsBroker, TestSQSBroker)
-), INSTALL_MESSAGE
+), about.INSTALL_MESSAGE
 
 __all__ = (
     "TestRabbitBroker",
     "TestRedisBroker",
     "TestKafkaBroker",
     "TestNatsBroker",
     "TestSQSBroker",
```

### Comparing `propan-0.1.2.5/propan/test/kafka.py` & `propan-0.1.2.6/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/test/nats.py` & `propan-0.1.2.6/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/test/rabbit.py` & `propan-0.1.2.6/propan/test/rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from propan.types import AnyDict
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
+
 from uuid import uuid4
 
 import aiormq
 from aio_pika.message import IncomingMessage
 from pamqp import commands as spec
 from pamqp.header import ContentHeader
```

### Comparing `propan-0.1.2.5/propan/test/redis.py` & `propan-0.1.2.6/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/test/sqs.py` & `propan-0.1.2.6/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/test/utils.py` & `propan-0.1.2.6/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/utils/functions.py` & `propan-0.1.2.6/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/utils/context/main.py` & `propan-0.1.2.6/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/propan/utils/context/types.py` & `propan-0.1.2.6/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/LICENSE` & `propan-0.1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/README.md` & `propan-0.1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/pyproject.toml` & `propan-0.1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.5/PKG-INFO` & `propan-0.1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.5
+Version: 0.1.2.6
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
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.5 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.6 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```


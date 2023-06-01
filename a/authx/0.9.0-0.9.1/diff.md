# Comparing `tmp/authx-0.9.0.tar.gz` & `tmp/authx-0.9.1.tar.gz`

## Comparing `authx-0.9.0.tar` & `authx-0.9.1.tar`

### file list

```diff
@@ -1,165 +1,161 @@
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 authx-0.9.0/.all-contributorsrc
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 authx-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 authx-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 authx-0.9.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 authx-0.9.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 authx-0.9.0/.github/dependabot.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 authx-0.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 authx-0.9.0/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 authx-0.9.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 authx-0.9.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 authx-0.9.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 authx-0.9.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 authx-0.9.0/authx/__init__.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 authx-0.9.0/authx/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/authx/py.typed
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/base.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/confirm.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/crud.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/manage.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/password.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/protection.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 authx-0.9.0/authx/backend/api/users.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 authx-0.9.0/authx/cache/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 authx-0.9.0/authx/cache/backend.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 authx-0.9.0/authx/cache/config.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 authx-0.9.0/authx/cache/redis.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/config.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/email.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/expiry.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/jwt.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/logger.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/password.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/session.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/socket.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/time.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 authx-0.9.0/authx/core/user.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 authx-0.9.0/authx/database/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 authx-0.9.0/authx/database/base.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 authx-0.9.0/authx/database/encodedb.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 authx-0.9.0/authx/database/mongodb.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 authx-0.9.0/authx/errors/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 authx-0.9.0/authx/errors/social.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/authx/handler/__init__.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 authx-0.9.0/authx/handler/errors.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 authx-0.9.0/authx/middleware/Oauth2.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 authx-0.9.0/authx/middleware/__init__.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx-0.9.0/authx/middleware/metrics.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx-0.9.0/authx/middleware/profiler.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 authx-0.9.0/authx/middleware/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/authx/models/__init__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 authx-0.9.0/authx/models/cache.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 authx-0.9.0/authx/models/common.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 authx-0.9.0/authx/models/social.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 authx-0.9.0/authx/models/user.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/admin.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/auth.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/password.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/search.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 authx-0.9.0/authx/routers/social.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/__init__.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/admin.py
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/auth.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/password.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/search.py
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 authx-0.9.0/authx/services/social.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/authx/utils/__init__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 authx-0.9.0/authx/utils/captcha.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 authx-0.9.0/authx/utils/keys.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 authx-0.9.0/authx/utils/logger.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 authx-0.9.0/authx/utils/strings.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 authx-0.9.0/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 authx-0.9.0/docs/contributing.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 authx-0.9.0/docs/faq.md
--rw-r--r--   0        0        0    86820 2020-02-02 00:00:00.000000 authx-0.9.0/docs/favicon.png
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-0.9.0/docs/header.svg
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 authx-0.9.0/docs/help.md
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 authx-0.9.0/docs/index.md
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 authx-0.9.0/docs/installation.md
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 authx-0.9.0/docs/license.md
--rw-r--r--   0        0        0    38188 2020-02-02 00:00:00.000000 authx-0.9.0/docs/release.md
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/Get-Started.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/cache/Example.md
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/cache/HTTPCache.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/cache/index.md
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/cache/redis.md
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/crud/index.md
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/database/encodedb.md
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/database/index.md
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/database/mongodb.md
--rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/middleware/example.md
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/middleware/index.md
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/middleware/metrics.md
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/middleware/profiling.md
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/middleware/service-performance.md
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/models/base.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/models/index.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/models/properties.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/models/social.md
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/admin.md
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/authentication.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/index.md
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/password.md
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/search.md
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/routers/social.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/captcha.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/email.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/hashing.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/index.md
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/jwt.md
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/security/session.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/admin.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/authentication.md
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/index.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/password.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/search.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/services/social-authentication.md
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 authx-0.9.0/docs/configuration/socket/index.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/clean.sh
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/docker.sh
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/docs_build.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/docs_serve.sh
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/format.sh
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/test.sh
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 authx-0.9.0/scripts/test_html.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 authx-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 authx-0.9.0/tests/test_version.py
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 authx-0.9.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/tests/cache/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 authx-0.9.0/tests/cache/test_cache_config.py
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 authx-0.9.0/tests/cache/test_http_cache.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 authx-0.9.0/tests/cache/test_keys.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 authx-0.9.0/tests/cache/test_method_cache.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx-0.9.0/tests/core/test_core_deps_session.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 authx-0.9.0/tests/core/test_core_email.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 authx-0.9.0/tests/core/test_core_jwt.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 authx-0.9.0/tests/core/test_core_session.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 authx-0.9.0/tests/core/test_core_user.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 authx-0.9.0/tests/key/private_key
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 authx-0.9.0/tests/key/public_key
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/__init__.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/test_metrics.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/test_middleware.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/test_middleware_Oauth2.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/example/.env.sample
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/example/__init__.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/example/app.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/example/db.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 authx-0.9.0/tests/middleware/example/requirements.txt
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 authx-0.9.0/tests/routers/test_routers_admin.py
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 authx-0.9.0/tests/routers/test_routers_auth.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 authx-0.9.0/tests/routers/test_routers_password.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 authx-0.9.0/tests/routers/test_routers_search.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 authx-0.9.0/tests/routers/test_routers_social.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 authx-0.9.0/tests/services/test_services_auth.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 authx-0.9.0/tests/services/test_services_password.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 authx-0.9.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 authx-0.9.0/LICENSE
--rw-r--r--   0        0        0     9856 2020-02-02 00:00:00.000000 authx-0.9.0/README.md
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 authx-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 authx-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 authx-0.9.1/.all-contributorsrc
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 authx-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 authx-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 authx-0.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 authx-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 authx-0.9.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 authx-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 authx-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 authx-0.9.1/authx/__init__.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 authx-0.9.1/authx/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/authx/py.typed
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/base.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/confirm.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/crud.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/manage.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/password.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/protection.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 authx-0.9.1/authx/backend/api/users.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 authx-0.9.1/authx/cache/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 authx-0.9.1/authx/cache/backend.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 authx-0.9.1/authx/cache/config.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 authx-0.9.1/authx/cache/redis.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/config.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/email.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/expiry.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/jwt.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/logger.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/password.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/session.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/socket.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/time.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 authx-0.9.1/authx/core/user.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 authx-0.9.1/authx/database/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 authx-0.9.1/authx/database/base.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 authx-0.9.1/authx/database/encodedb.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 authx-0.9.1/authx/database/mongodb.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 authx-0.9.1/authx/errors/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 authx-0.9.1/authx/errors/social.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/authx/handler/__init__.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 authx-0.9.1/authx/handler/errors.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 authx-0.9.1/authx/middleware/Oauth2.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 authx-0.9.1/authx/middleware/__init__.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx-0.9.1/authx/middleware/metrics.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx-0.9.1/authx/middleware/profiler.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 authx-0.9.1/authx/middleware/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/authx/models/__init__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 authx-0.9.1/authx/models/cache.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 authx-0.9.1/authx/models/common.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 authx-0.9.1/authx/models/social.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 authx-0.9.1/authx/models/user.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/admin.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/auth.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/password.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/search.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 authx-0.9.1/authx/routers/social.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/__init__.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/admin.py
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/auth.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/password.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/search.py
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 authx-0.9.1/authx/services/social.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/authx/utils/__init__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 authx-0.9.1/authx/utils/captcha.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 authx-0.9.1/authx/utils/keys.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 authx-0.9.1/authx/utils/logger.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 authx-0.9.1/authx/utils/strings.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 authx-0.9.1/docs/code_of_conduct.md
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 authx-0.9.1/docs/contributing.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 authx-0.9.1/docs/faq.md
+-rw-r--r--   0        0        0    86820 2020-02-02 00:00:00.000000 authx-0.9.1/docs/favicon.png
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-0.9.1/docs/header.svg
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 authx-0.9.1/docs/help.md
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 authx-0.9.1/docs/index.md
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 authx-0.9.1/docs/installation.md
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 authx-0.9.1/docs/license.md
+-rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 authx-0.9.1/docs/release.md
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/Get-Started.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/cache/Example.md
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/cache/HTTPCache.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/cache/index.md
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/cache/redis.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/crud/index.md
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/database/encodedb.md
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/database/index.md
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/database/mongodb.md
+-rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/middleware/example.md
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/middleware/index.md
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/middleware/metrics.md
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/middleware/profiling.md
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/middleware/service-performance.md
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/models/base.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/models/index.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/models/properties.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/models/social.md
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/admin.md
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/authentication.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/index.md
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/password.md
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/search.md
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/routers/social.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/captcha.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/email.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/hashing.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/index.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/jwt.md
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/security/session.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/admin.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/authentication.md
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/index.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/password.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/search.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/services/social-authentication.md
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 authx-0.9.1/docs/configuration/socket/index.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/clean.sh
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/docker.sh
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/docs_build.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/format.sh
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/test.sh
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 authx-0.9.1/scripts/test_html.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 authx-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 authx-0.9.1/tests/test_version.py
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 authx-0.9.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/tests/cache/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 authx-0.9.1/tests/cache/test_cache_config.py
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 authx-0.9.1/tests/cache/test_http_cache.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 authx-0.9.1/tests/cache/test_keys.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 authx-0.9.1/tests/cache/test_method_cache.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx-0.9.1/tests/core/test_core_deps_session.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 authx-0.9.1/tests/core/test_core_email.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 authx-0.9.1/tests/core/test_core_jwt.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 authx-0.9.1/tests/core/test_core_session.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 authx-0.9.1/tests/core/test_core_user.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 authx-0.9.1/tests/key/private_key
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 authx-0.9.1/tests/key/public_key
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/test_metrics.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/test_middleware.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/test_middleware_Oauth2.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/example/.env.sample
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/example/__init__.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/example/app.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/example/db.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 authx-0.9.1/tests/middleware/example/requirements.txt
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 authx-0.9.1/tests/routers/test_routers_admin.py
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 authx-0.9.1/tests/routers/test_routers_auth.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 authx-0.9.1/tests/routers/test_routers_password.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 authx-0.9.1/tests/routers/test_routers_search.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 authx-0.9.1/tests/routers/test_routers_social.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 authx-0.9.1/tests/services/test_services_auth.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 authx-0.9.1/tests/services/test_services_password.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 authx-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 authx-0.9.1/LICENSE
+-rw-r--r--   0        0        0     9806 2020-02-02 00:00:00.000000 authx-0.9.1/README.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 authx-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 authx-0.9.1/PKG-INFO
```

### Comparing `authx-0.9.0/.all-contributorsrc` & `authx-0.9.1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/.pre-commit-config.yaml` & `authx-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/mkdocs.yml` & `authx-0.9.1/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 site_name: AuthenticationX
 site_description: Ready to use and customizable Authentications and Oauth2 management for FastAPI ⚡
-site_url: https://authx.yezz.me/
+site_url: https://authx-v0.yezz.me/
 
 theme:
   features:
     - header.autohide
   name: 'material'
   palette:
     - scheme: default
```

### Comparing `authx-0.9.0/.github/workflows/documentation.yml` & `authx-0.9.1/.github/workflows/release.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-name: Build Docs
+name: Publish
+
 on:
-  push:
-    branches:
-      - main
+  release:
+    types:
+      - created
 
 jobs:
-  build-docs:
-    runs-on: ubuntu-18.04
+  publish:
+    runs-on: ubuntu-latest
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-docs
-      - name: Install docs extras
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
+      - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install -e .[docs]
-      - name: Build docs
-        run: bash scripts/docs_build.sh
-
-      - name: Deploy docs
-        uses: jsmrcaga/action-netlify-deploy@v1.1.0
+        run: pip install build
+      - name: Build distribution
+        run: python -m build
+      - name: Publish
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
-          NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_TOKEN }}
-          NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
-          NETLIFY_DEPLOY_TO_PROD: true
-          NETLIFY_DEPLOY_MESSAGE: "Prod deploy v${{ github.ref }}"
+          password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Dump GitHub context
+        env:
+          GITHUB_CONTEXT: ${{ toJson(github) }}
+        run: echo "$GITHUB_CONTEXT"
```

### Comparing `authx-0.9.0/.github/workflows/lint.yml` & `authx-0.9.1/.github/workflows/lint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Lint and Format
 
 on:
   push:
     branches:
-      - main
+      - 0.X.X-fix
   pull_request:
     types: [opened, synchronize]
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `authx-0.9.0/.github/workflows/test.yml` & `authx-0.9.1/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Test Suite
 
 on:
   push:
     branches:
-      - main
+      - 0.X.X-fix
   pull_request:
     types: [opened, synchronize]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     services:
```

### Comparing `authx-0.9.0/authx/__init__.py` & `authx-0.9.1/authx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Ready to use and customizable Authentications and Oauth2 management for FastAPI"""
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 from authx.backend import UsersRepo as UsersRepo
 from authx.cache import RedisBackend as RedisBackend
 from authx.core import AuthXSocket as AuthXSocket
 from authx.core import EmailClient as EmailClient
 from authx.core import JWTBackend as JWTBackend
 from authx.core import User as User
```

### Comparing `authx-0.9.0/authx/main.py` & `authx-0.9.1/authx/main.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/base.py` & `authx-0.9.1/authx/backend/base.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/__init__.py` & `authx-0.9.1/authx/backend/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/confirm.py` & `authx-0.9.1/authx/backend/api/confirm.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/crud.py` & `authx-0.9.1/authx/backend/api/crud.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/manage.py` & `authx-0.9.1/authx/backend/api/manage.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/password.py` & `authx-0.9.1/authx/backend/api/password.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/protection.py` & `authx-0.9.1/authx/backend/api/protection.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/backend/api/users.py` & `authx-0.9.1/authx/backend/api/users.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/cache/backend.py` & `authx-0.9.1/authx/cache/backend.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/cache/config.py` & `authx-0.9.1/authx/cache/config.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/cache/redis.py` & `authx-0.9.1/authx/cache/redis.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/__init__.py` & `authx-0.9.1/authx/core/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/config.py` & `authx-0.9.1/authx/core/config.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/email.py` & `authx-0.9.1/authx/core/email.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/expiry.py` & `authx-0.9.1/authx/core/expiry.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/jwt.py` & `authx-0.9.1/authx/core/jwt.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/logger.py` & `authx-0.9.1/authx/core/logger.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/session.py` & `authx-0.9.1/authx/core/session.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/socket.py` & `authx-0.9.1/authx/core/socket.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/time.py` & `authx-0.9.1/authx/core/time.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/core/user.py` & `authx-0.9.1/authx/core/user.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/database/base.py` & `authx-0.9.1/authx/database/base.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/database/encodedb.py` & `authx-0.9.1/authx/database/encodedb.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/database/mongodb.py` & `authx-0.9.1/authx/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/handler/errors.py` & `authx-0.9.1/authx/handler/errors.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/middleware/Oauth2.py` & `authx-0.9.1/authx/middleware/Oauth2.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/middleware/metrics.py` & `authx-0.9.1/authx/middleware/metrics.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/middleware/profiler.py` & `authx-0.9.1/authx/middleware/profiler.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/middleware/service.py` & `authx-0.9.1/authx/middleware/service.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/models/cache.py` & `authx-0.9.1/authx/models/cache.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/models/common.py` & `authx-0.9.1/authx/models/common.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/models/social.py` & `authx-0.9.1/authx/models/social.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/models/user.py` & `authx-0.9.1/authx/models/user.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/routers/admin.py` & `authx-0.9.1/authx/routers/admin.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/routers/auth.py` & `authx-0.9.1/authx/routers/auth.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/routers/password.py` & `authx-0.9.1/authx/routers/password.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/routers/search.py` & `authx-0.9.1/authx/routers/search.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/routers/social.py` & `authx-0.9.1/authx/routers/social.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/services/admin.py` & `authx-0.9.1/authx/services/admin.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/services/auth.py` & `authx-0.9.1/authx/services/auth.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/services/password.py` & `authx-0.9.1/authx/services/password.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/services/search.py` & `authx-0.9.1/authx/services/search.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/services/social.py` & `authx-0.9.1/authx/services/social.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/utils/captcha.py` & `authx-0.9.1/authx/utils/captcha.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/utils/keys.py` & `authx-0.9.1/authx/utils/keys.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/authx/utils/logger.py` & `authx-0.9.1/authx/utils/logger.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/code_of_conduct.md` & `authx-0.9.1/docs/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/contributing.md` & `authx-0.9.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/faq.md` & `authx-0.9.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/favicon.png` & `authx-0.9.1/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/header.svg` & `authx-0.9.1/docs/header.svg`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/help.md` & `authx-0.9.1/docs/help.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/index.md` & `authx-0.9.1/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
 </p>
 
 [![Test](https://github.com/yezz123/authx/actions/workflows/test.yml/badge.svg)](https://github.com/yezz123/authx/actions/workflows/test.yml)
 [![Publish](https://github.com/yezz123/authx/actions/workflows/release.yml/badge.svg)](https://github.com/yezz123/authx/actions/workflows/release.yml)
 [![Pypi](https://img.shields.io/pypi/pyversions/AuthX.svg?color=%2334D058)](https://pypi.org/project/AuthX)
-[![codecov](https://codecov.io/gh/yezz123/AuthX/branch/main/graph/badge.svg?token=3j5znCNzDp)](https://codecov.io/gh/yezz123/AuthX)
+[![codecov](https://codecov.io/gh/yezz123/AuthX/branch/0.X.X-fix/graph/badge.svg)](https://codecov.io/gh/yezz123/AuthX)
 [![PyPI](https://badge.fury.io/py/authx.svg)](https://badge.fury.io/py/authx)
 [![Downloads](https://pepy.tech/badge/authx)](https://pepy.tech/project/authx)
 [![framework](https://img.shields.io/badge/Framework-FastAPI-blue?style)](https://fastapi.tiangolo.com/)
 
 <!--  -->
 
 ---
 
 **Source Code**: <https://github.com/yezz123/authx>
 
-**Get Started**: <https://authx.yezz.me/>
+**Get Started**: <https://authx-v0.yezz.me/>
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **Authx** is designed to be as
 customizable and adaptable as possible.
```

### Comparing `authx-0.9.0/docs/license.md` & `authx-0.9.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/release.md` & `authx-0.9.1/docs/release.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,41 @@
 # Release Notes 🎞
 
+## 0.9.0
+
+### Fixes 🐛
+
+* ➕ Support Python 3.11 by @yezz123 in <https://github.com/yezz123/authx/pull/355>
+* 🐛  Support `aioredis` from redis package by @yezz123 in <https://github.com/yezz123/authx/pull/369>
+
+### Dependencies 🔨
+
+* ⬆ Update email-validator requirement from <1.3.1,>=1.1.0 to >=1.1.0,<1.3.2 by @dependabot in <https://github.com/yezz123/authx/pull/347>
+* ⬆ Bump pymdown-extensions from 9.9.1 to 9.9.2 by @dependabot in <https://github.com/yezz123/authx/pull/346>
+* ⬆ Bump pre-commit from 2.21.0 to 3.0.0 by @dependabot in <https://github.com/yezz123/authx/pull/348>
+* ⬆ Update sqlalchemy requirement from <1.4.47,>=1.4.37 to >=1.4.37,<2.0.1 by @dependabot in <https://github.com/yezz123/authx/pull/350>
+* ⬆ Bump pre-commit from 3.0.0 to 3.0.1 by @dependabot in <https://github.com/yezz123/authx/pull/349>
+* ⬆ Bump pre-commit from 3.0.1 to 3.0.4 by @dependabot in <https://github.com/yezz123/authx/pull/354>
+* ⬆ Update sqlalchemy requirement from <2.0.1,>=1.4.37 to >=1.4.37,<2.0.2 by @dependabot in <https://github.com/yezz123/authx/pull/353>
+* ⬆ Update starlette requirement from <0.23.2,>=0.14.02 to >=0.14.02,<0.24.1 by @dependabot in <https://github.com/yezz123/authx/pull/356>
+* ⬆ Update sqlalchemy requirement from <2.0.2,>=1.4.37 to >=1.4.37,<2.0.3 by @dependabot in <https://github.com/yezz123/authx/pull/357>
+* ⬆ Bump cryptography from 39.0.0 to 39.0.1 by @dependabot in <https://github.com/yezz123/authx/pull/358>
+* ⬆ Update redis requirement from <4.4.3,>=4.3.3 to >=4.3.3,<4.5.1 by @dependabot in <https://github.com/yezz123/authx/pull/359>
+* ⬆ Bump markdown-include from 0.8.0 to 0.8.1 by @dependabot in <https://github.com/yezz123/authx/pull/360>
+* ⬆ Update fastapi requirement from <0.90.0,>=0.65.2 to >=0.65.2,<0.91.0 by @dependabot in <https://github.com/yezz123/authx/pull/361>
+* ⬆ Update redis requirement from <4.5.1,>=4.3.3 to >=4.3.3,<4.5.2 by @dependabot in <https://github.com/yezz123/authx/pull/362>
+* ⬆ Update sqlalchemy requirement from <2.0.3,>=1.4.37 to >=1.4.37,<2.0.4 by @dependabot in <https://github.com/yezz123/authx/pull/363>
+* ⬆ Update fastapi requirement from <0.91.0,>=0.65.2 to >=0.65.2,<0.92.0 by @dependabot in <https://github.com/yezz123/authx/pull/364>
+* ⬆ Update starlette requirement from <0.24.1,>=0.14.02 to >=0.14.02,<0.25.1 by @dependabot in <https://github.com/yezz123/authx/pull/366>
+* ⬆ Update fastapi requirement from <0.92.0,>=0.65.2 to >=0.65.2,<0.93.0 by @dependabot in <https://github.com/yezz123/authx/pull/367>
+* ⬆ Bump pydantic from 1.10.4 to 1.10.5 by @dependabot in <https://github.com/yezz123/authx/pull/368>
+* ⬆ Bump starlette from 0.17.1 to 0.25.0 in /tests/middleware/example by @dependabot in <https://github.com/yezz123/authx/pull/365>
+
+**Full Changelog**: <https://github.com/yezz123/authx/compare/0.8.3...0.9.0>
+
 ## 0.8.3
 
 ### Fixes 🐛
 
 * Fixes a few imports in the documentation by @alobbs in <https://github.com/yezz123/authx/pull/343>
 * ✨ Use Ruff for linting by @yezz123 in <https://github.com/yezz123/authx/pull/344>
 
@@ -392,15 +424,15 @@
 from pytz import timezone
 
 africa_Casablanca = timezone('Africa/Casablanca')
 HTTPCache.init(redis_url=REDIS_URL, namespace='test_namespace', tz=africa_Casablanca)
 ```
 
 * Read More in the New Documentation:
-  <https://authx.yezz.me/configuration/cache/httpcache/>
+  <https://authx-v0.yezz.me/configuration/cache/httpcache/>
 
 ### What's Changed
 
 * chore(docs): Improve Documentation by @yezz123 in
   <https://github.com/yezz123/authx/pull/209>
 * chore(dev): refactor code & improve some exceptions ✨ by @yezz123 in
   <https://github.com/yezz123/authx/pull/212>
@@ -477,15 +509,15 @@
     redisURL="redis://localhost:6379/1",
     sessionIdName="sessionId",
     sessionIdGenerator=lambda: str(random.randint(1000, 9999)),
     expireTime=timedelta(days=1),
 )
 ```
 
-* Read the Changelog <https://authx.yezz.me/release/>
+* Read the Changelog <https://authx-v0.yezz.me/release/>
 
 ## What's Changed
 
 * chore(dev): Add Sessions Requirements by @yezz123 in
   <https://github.com/yezz123/authx/pull/207>
 
 * chore(docs): Documented the Functionality of Session Storing by @yezz123 in
```

### Comparing `authx-0.9.0/docs/configuration/Get-Started.md` & `authx-0.9.1/docs/configuration/Get-Started.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/cache/Example.md` & `authx-0.9.1/docs/configuration/cache/Example.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/cache/HTTPCache.md` & `authx-0.9.1/docs/configuration/cache/HTTPCache.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/cache/index.md` & `authx-0.9.1/docs/configuration/cache/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/cache/redis.md` & `authx-0.9.1/docs/configuration/cache/redis.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/crud/index.md` & `authx-0.9.1/docs/configuration/crud/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/database/encodedb.md` & `authx-0.9.1/docs/configuration/database/encodedb.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/database/index.md` & `authx-0.9.1/docs/configuration/database/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/database/mongodb.md` & `authx-0.9.1/docs/configuration/database/mongodb.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/middleware/example.md` & `authx-0.9.1/docs/configuration/middleware/example.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/middleware/index.md` & `authx-0.9.1/docs/configuration/middleware/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/middleware/metrics.md` & `authx-0.9.1/docs/configuration/middleware/metrics.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/middleware/profiling.md` & `authx-0.9.1/docs/configuration/middleware/profiling.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/middleware/service-performance.md` & `authx-0.9.1/docs/configuration/middleware/service-performance.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/models/base.md` & `authx-0.9.1/docs/configuration/models/base.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/models/index.md` & `authx-0.9.1/docs/configuration/models/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/models/properties.md` & `authx-0.9.1/docs/configuration/models/properties.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/models/social.md` & `authx-0.9.1/docs/configuration/models/social.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/admin.md` & `authx-0.9.1/docs/configuration/routers/admin.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/authentication.md` & `authx-0.9.1/docs/configuration/routers/authentication.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/index.md` & `authx-0.9.1/docs/configuration/routers/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/password.md` & `authx-0.9.1/docs/configuration/routers/password.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/search.md` & `authx-0.9.1/docs/configuration/routers/search.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/routers/social.md` & `authx-0.9.1/docs/configuration/routers/social.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/captcha.md` & `authx-0.9.1/docs/configuration/security/captcha.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/email.md` & `authx-0.9.1/docs/configuration/security/email.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/hashing.md` & `authx-0.9.1/docs/configuration/security/hashing.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/index.md` & `authx-0.9.1/docs/configuration/security/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/jwt.md` & `authx-0.9.1/docs/configuration/security/jwt.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/security/session.md` & `authx-0.9.1/docs/configuration/security/session.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/services/admin.md` & `authx-0.9.1/docs/configuration/services/admin.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/services/authentication.md` & `authx-0.9.1/docs/configuration/services/authentication.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/services/password.md` & `authx-0.9.1/docs/configuration/services/password.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/services/search.md` & `authx-0.9.1/docs/configuration/services/search.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/docs/configuration/socket/index.md` & `authx-0.9.1/docs/configuration/socket/index.md`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/scripts/clean.sh` & `authx-0.9.1/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/utils.py` & `authx-0.9.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/cache/test_cache_config.py` & `authx-0.9.1/tests/cache/test_cache_config.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/cache/test_http_cache.py` & `authx-0.9.1/tests/cache/test_http_cache.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/cache/test_keys.py` & `authx-0.9.1/tests/cache/test_keys.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/cache/test_method_cache.py` & `authx-0.9.1/tests/cache/test_method_cache.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/core/test_core_deps_session.py` & `authx-0.9.1/tests/core/test_core_deps_session.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/core/test_core_jwt.py` & `authx-0.9.1/tests/core/test_core_jwt.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/core/test_core_session.py` & `authx-0.9.1/tests/core/test_core_session.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/core/test_core_user.py` & `authx-0.9.1/tests/core/test_core_user.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/key/private_key` & `authx-0.9.1/tests/key/private_key`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/middleware/test_metrics.py` & `authx-0.9.1/tests/middleware/test_metrics.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/middleware/test_middleware.py` & `authx-0.9.1/tests/middleware/test_middleware.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/middleware/test_middleware_Oauth2.py` & `authx-0.9.1/tests/middleware/test_middleware_Oauth2.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/middleware/example/app.py` & `authx-0.9.1/tests/middleware/example/app.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/middleware/example/db.py` & `authx-0.9.1/tests/middleware/example/db.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/routers/test_routers_admin.py` & `authx-0.9.1/tests/routers/test_routers_admin.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/routers/test_routers_auth.py` & `authx-0.9.1/tests/routers/test_routers_auth.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/routers/test_routers_password.py` & `authx-0.9.1/tests/routers/test_routers_password.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/routers/test_routers_search.py` & `authx-0.9.1/tests/routers/test_routers_search.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/routers/test_routers_social.py` & `authx-0.9.1/tests/routers/test_routers_social.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/services/test_services_auth.py` & `authx-0.9.1/tests/services/test_services_auth.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/tests/services/test_services_password.py` & `authx-0.9.1/tests/services/test_services_password.py`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/.gitignore` & `authx-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/LICENSE` & `authx-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `authx-0.9.0/README.md` & `authx-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 <a href="https://github.com/yezz123/authx/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/yezz123/authx/actions/workflows/test.yml/badge.svg" alt="lint">
 </a>
 <a href="https://pypi.org/project/authx" target="_blank">
     <img src="https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
-    <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
+    <img src="https://codecov.io/gh/yezz123/authx/branch/0.X.X-fix/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://pepy.tech/badge/authx" alt="Test">
 </a>
 </p>
 
-
 ---
 
 **Source Code**: <https://github.com/yezz123/AuthX>
 
-**Documentation**: <https://authx.yezz.me/>
+**Documentation**: <https://authx-v0.yezz.me/>
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **AuthX** is designed to be as
 customizable and adaptable as possible.
 
@@ -65,17 +64,15 @@
 - [x] Support Sessions and Pre-built CRUD functions and Instance to launch
       Redis.
 - [x] Support SocketIO.
 - [x] Support Middleware of [pyinstrument](https://pyinstrument.readthedocs.io/)
       to check your service performance.
 - [x] Support Middleware for collecting and exposing [Prometheus](https://prometheus.io/) metrics.
 
-**Note:** Check [Release Notes](https://authx.yezz.me/release/).
-
-**Note:** Check [Examples](https://github.com/yezz123/authx/tree/main/example).
+**Note:** Check [Release Notes](https://authx-v0.yezz.me/release/).
 
 ## Project using 🚀
 
 ```python
 from fastapi import Depends, FastAPI
 from authx import Authentication, User, RedisBackend
 
@@ -159,18 +156,18 @@
 
 This project follows the
 [all-contributors](https://github.com/all-contributors/all-contributors)
 specification. Contributions of any kind welcome!
 
 ## Links 🚧
 
-- [Homepage](https://authx.yezz.me/)
-- [FAQ](https://authx.yezz.me/faq/)
-- [Release - AuthX](https://authx.yezz.me/release/)
-- [MIT License](https://authx.yezz.me/license/)
-- [Code of Conduct](https://authx.yezz.me/code_of_conduct/)
-- [Contributing](https://authx.yezz.me/contributing/)
-- [Help - Sponsors](https://authx.yezz.me/help/)
+- [Homepage](https://authx-v0.yezz.me/)
+- [FAQ](https://authx-v0.yezz.me/faq/)
+- [Release - AuthX](https://authx-v0.yezz.me/release/)
+- [MIT License](https://authx-v0.yezz.me/license/)
+- [Code of Conduct](https://authx-v0.yezz.me/code_of_conduct/)
+- [Contributing](https://authx-v0.yezz.me/contributing/)
+- [Help - Sponsors](https://authx-v0.yezz.me/help/)
 
 ## License 📝
 
 This project is licensed under the terms of the MIT License.
```

### Comparing `authx-0.9.0/pyproject.toml` & `authx-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,67 +26,66 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "fastapi >=0.65.2,<0.93.0",
+    "fastapi >=0.65.2,<0.96.0",
     "passlib ==1.7.4",
     "bcrypt ==4.0.1",
-    "email-validator >=1.1.0,<1.3.2",
-    "pyjwt ==2.6.0",
-    "cryptography==39.0.1",
-    "httpx==0.23.3",
+    "email-validator >=1.1.0,<2.0.1",
+    "pyjwt ==2.7.0",
+    "cryptography==41.0.0",
+    "httpx==0.24.1",
     "itsdangerous == 2.1.2",
     "aiosmtplib == 2.0.1",
-    "pydantic==1.10.5",
+    "pydantic==1.10.7",
     "databases == 0.7.0",
-    "motor == 3.1.1",
+    "motor == 3.1.2",
     "Authlib==0.15.5",
-    "starlette >=0.14.02,<0.25.1",
-    "redis >=4.3.3,<4.5.2",
-    "pytz==2022.7.1",
+    "starlette >=0.14.02,<0.27.1",
+    "redis >=4.3.3,<4.5.6",
+    "pytz==2023.3",
     "python-dateutil==2.8.2",
-    "python-socketio >=4.6.0,<5.7.3",
+    "python-socketio >=4.6.0,<5.8.1",
     "pyinstrument >=4.1.1,<4.5.0",
-    "SQLAlchemy >=1.4.37,<2.0.4",
+    "SQLAlchemy >=1.4.37,<2.0.16",
     "prometheus-client",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/yezz123/authx"
-Documentation = "https://authx.yezz.me/"
+Documentation = "https://authx-v0.yezz.me/"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 lint = [
-    "pre-commit==3.0.4",
+    "pre-commit==3.3.2",
 ]
 test = [
-    "pytest==7.2.1",
-    "pytest-asyncio == 0.20.3",
-    "requests==2.28.2",
-    "uvicorn==0.20.0",
+    "pytest==7.3.1",
+    "pytest-asyncio == 0.21.0",
+    "requests==2.31.0",
+    "uvicorn==0.22.0",
     "asynctest==0.13.0",
-    "codecov==2.1.12",
-    "pytest-cov==4.0.0",
-    "websockets==10.4",
+    "pytest-cov==4.1.0",
+    "websockets==11.0.3",
     "uvloop==0.17.0"
 ]
 docs = [
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<10.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "mkdocs-mermaid2-plugin==0.6.0",
     "markdown-include==0.8.1",
-    "pymdown-extensions==9.9.2",
+    "pymdown-extensions==10.0.1",
     "jinja2==3.1.2"
 ]
 
 [tool.hatch.version]
 path = "authx/__init__.py"
 
 
@@ -115,28 +114,17 @@
 
 [tool.ruff.isort]
 known-third-party = ["pydantic", "sqlalchemy", "typing_extensions"]
 
 [tool.coverage.run]
 parallel = true
 source = [
-    "tests",
     "authx"
 ]
 context = '${CONTEXT}'
-omit = [
-    "authx/core/config.py",
-    "authx/main.py",
-    "authx/utils/**",
-    "authx/errors/**",
-    "authx/database/**",
-    "authx/cache/**",
-    "authx/services/**",
-    "tests/middleware/example/**"
-]
 
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
```

### Comparing `authx-0.9.0/PKG-INFO` & `authx-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: authx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Ready to use and customizable Authentications and Oauth2 management for FastAPI
 Project-URL: Homepage, https://github.com/yezz123/authx
-Project-URL: Documentation, https://authx.yezz.me/
+Project-URL: Documentation, https://authx-v0.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
@@ -22,53 +22,52 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: aiosmtplib==2.0.1
 Requires-Dist: authlib==0.15.5
 Requires-Dist: bcrypt==4.0.1
-Requires-Dist: cryptography==39.0.1
+Requires-Dist: cryptography==41.0.0
 Requires-Dist: databases==0.7.0
-Requires-Dist: email-validator<1.3.2,>=1.1.0
-Requires-Dist: fastapi<0.93.0,>=0.65.2
-Requires-Dist: httpx==0.23.3
+Requires-Dist: email-validator<2.0.1,>=1.1.0
+Requires-Dist: fastapi<0.96.0,>=0.65.2
+Requires-Dist: httpx==0.24.1
 Requires-Dist: itsdangerous==2.1.2
-Requires-Dist: motor==3.1.1
+Requires-Dist: motor==3.1.2
 Requires-Dist: passlib==1.7.4
 Requires-Dist: prometheus-client
-Requires-Dist: pydantic==1.10.5
+Requires-Dist: pydantic==1.10.7
 Requires-Dist: pyinstrument<4.5.0,>=4.1.1
-Requires-Dist: pyjwt==2.6.0
+Requires-Dist: pyjwt==2.7.0
 Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: python-socketio<5.7.3,>=4.6.0
-Requires-Dist: pytz==2022.7.1
-Requires-Dist: redis<4.5.2,>=4.3.3
-Requires-Dist: sqlalchemy<2.0.4,>=1.4.37
-Requires-Dist: starlette<0.25.1,>=0.14.02
+Requires-Dist: python-socketio<5.8.1,>=4.6.0
+Requires-Dist: pytz==2023.3
+Requires-Dist: redis<4.5.6,>=4.3.3
+Requires-Dist: sqlalchemy<2.0.16,>=1.4.37
+Requires-Dist: starlette<0.27.1,>=0.14.02
 Provides-Extra: docs
 Requires-Dist: jinja2==3.1.2; extra == 'docs'
 Requires-Dist: markdown-include==0.8.1; extra == 'docs'
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'docs'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'docs'
 Requires-Dist: mkdocs-material<10.0.0,>=8.1.4; extra == 'docs'
 Requires-Dist: mkdocs-mermaid2-plugin==0.6.0; extra == 'docs'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'docs'
-Requires-Dist: pymdown-extensions==9.9.2; extra == 'docs'
+Requires-Dist: pymdown-extensions==10.0.1; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: pre-commit==3.0.4; extra == 'lint'
+Requires-Dist: pre-commit==3.3.2; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: asynctest==0.13.0; extra == 'test'
-Requires-Dist: codecov==2.1.12; extra == 'test'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'test'
-Requires-Dist: pytest-cov==4.0.0; extra == 'test'
-Requires-Dist: pytest==7.2.1; extra == 'test'
-Requires-Dist: requests==2.28.2; extra == 'test'
-Requires-Dist: uvicorn==0.20.0; extra == 'test'
+Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
+Requires-Dist: pytest-cov==4.1.0; extra == 'test'
+Requires-Dist: pytest==7.3.1; extra == 'test'
+Requires-Dist: requests==2.31.0; extra == 'test'
+Requires-Dist: uvicorn==0.22.0; extra == 'test'
 Requires-Dist: uvloop==0.17.0; extra == 'test'
-Requires-Dist: websockets==10.4; extra == 'test'
+Requires-Dist: websockets==11.0.3; extra == 'test'
 Description-Content-Type: text/markdown
 
 # AuthenticationX 💫
 
 ![authx](https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png)
 
 <p align="center">
@@ -79,27 +78,26 @@
 <a href="https://github.com/yezz123/authx/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/yezz123/authx/actions/workflows/test.yml/badge.svg" alt="lint">
 </a>
 <a href="https://pypi.org/project/authx" target="_blank">
     <img src="https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
-    <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
+    <img src="https://codecov.io/gh/yezz123/authx/branch/0.X.X-fix/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://pepy.tech/badge/authx" alt="Test">
 </a>
 </p>
 
-
 ---
 
 **Source Code**: <https://github.com/yezz123/AuthX>
 
-**Documentation**: <https://authx.yezz.me/>
+**Documentation**: <https://authx-v0.yezz.me/>
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **AuthX** is designed to be as
 customizable and adaptable as possible.
 
@@ -134,17 +132,15 @@
 - [x] Support Sessions and Pre-built CRUD functions and Instance to launch
       Redis.
 - [x] Support SocketIO.
 - [x] Support Middleware of [pyinstrument](https://pyinstrument.readthedocs.io/)
       to check your service performance.
 - [x] Support Middleware for collecting and exposing [Prometheus](https://prometheus.io/) metrics.
 
-**Note:** Check [Release Notes](https://authx.yezz.me/release/).
-
-**Note:** Check [Examples](https://github.com/yezz123/authx/tree/main/example).
+**Note:** Check [Release Notes](https://authx-v0.yezz.me/release/).
 
 ## Project using 🚀
 
 ```python
 from fastapi import Depends, FastAPI
 from authx import Authentication, User, RedisBackend
 
@@ -228,18 +224,18 @@
 
 This project follows the
 [all-contributors](https://github.com/all-contributors/all-contributors)
 specification. Contributions of any kind welcome!
 
 ## Links 🚧
 
-- [Homepage](https://authx.yezz.me/)
-- [FAQ](https://authx.yezz.me/faq/)
-- [Release - AuthX](https://authx.yezz.me/release/)
-- [MIT License](https://authx.yezz.me/license/)
-- [Code of Conduct](https://authx.yezz.me/code_of_conduct/)
-- [Contributing](https://authx.yezz.me/contributing/)
-- [Help - Sponsors](https://authx.yezz.me/help/)
+- [Homepage](https://authx-v0.yezz.me/)
+- [FAQ](https://authx-v0.yezz.me/faq/)
+- [Release - AuthX](https://authx-v0.yezz.me/release/)
+- [MIT License](https://authx-v0.yezz.me/license/)
+- [Code of Conduct](https://authx-v0.yezz.me/code_of_conduct/)
+- [Contributing](https://authx-v0.yezz.me/contributing/)
+- [Help - Sponsors](https://authx-v0.yezz.me/help/)
 
 ## License 📝
 
 This project is licensed under the terms of the MIT License.
```


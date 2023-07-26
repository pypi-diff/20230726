# Comparing `tmp/fabric-credmgr-client-1.6.0b8.tar.gz` & `tmp/fabric-credmgr-client-1.6.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.6.0b8.tar", last modified: Wed Jul 26 18:49:34 2023, max compression
+gzip compressed data, was "fabric-credmgr-client-1.6.0b9.tar", last modified: Wed Jul 26 20:19:14 2023, max compression
```

## Comparing `fabric-credmgr-client-1.6.0b8.tar` & `fabric-credmgr-client-1.6.0b9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b8/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b8/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b8/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b8/.travis.yml
--rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b8/LICENSE
--rw-r--r--   0        0        0     4941 2023-07-25 19:41:10.336694 fabric-credmgr-client-1.6.0b8/README.md
--rw-r--r--   0        0        0      329 2023-07-17 13:35:48.694756 fabric-credmgr-client-1.6.0b8/docs/DecodedToken.md
--rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b8/docs/DefaultApi.md
--rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b8/docs/Jwks.md
--rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b8/docs/JwksKeys.md
--rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b8/docs/Request.md
--rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b8/docs/RevokeList.md
--rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b8/docs/Status200OkNoContent.md
--rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b8/docs/Status200OkNoContentData.md
--rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b8/docs/Status200OkPaginated.md
--rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b8/docs/Status200OkSingle.md
--rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b8/docs/Status400BadRequest.md
--rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b8/docs/Status400BadRequestErrors.md
--rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b8/docs/Status401Unauthorized.md
--rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b8/docs/Status401UnauthorizedErrors.md
--rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b8/docs/Status403Forbidden.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b8/docs/Status403ForbiddenErrors.md
--rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b8/docs/Status404NotFound.md
--rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b8/docs/Status404NotFoundErrors.md
--rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b8/docs/Status500InternalServerError.md
--rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b8/docs/Status500InternalServerErrorErrors.md
--rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b8/docs/Success.md
--rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b8/docs/Token.md
--rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b8/docs/TokenPost.md
--rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b8/docs/Tokens.md
--rw-r--r--   0        0        0    12847 2023-07-26 16:08:53.625902 fabric-credmgr-client-1.6.0b8/docs/TokensApi.md
--rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b8/docs/Version.md
--rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b8/docs/VersionApi.md
--rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b8/docs/VersionData.md
--rw-r--r--   0        0        0       50 2023-07-26 18:49:08.571799 fabric-credmgr-client-1.6.0b8/fabric_cm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/__init__.py
--rw-r--r--   0        0        0    13111 2023-07-26 18:40:00.606510 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/credmgr_proxy.py
--rw-r--r--   0        0        0     2060 2023-07-26 15:37:13.962587 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/session_helper.py
--rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/__init__.py
--rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0        0        0    30241 2023-07-26 18:46:26.266396 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25120 2023-07-25 23:33:20.373712 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/configuration.py
--rw-r--r--   0        0        0     2466 2023-07-17 13:34:51.161528 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3472 2023-07-17 13:38:26.234277 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/decoded_token.py
--rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/revoke_list.py
--rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/token_post.py
--rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b8/git_push.sh
--rw-r--r--   0        0        0     1129 2023-07-25 18:45:35.707490 fabric-credmgr-client-1.6.0b8/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b8/test/__init__.py
--rw-r--r--   0        0        0      738 2023-07-26 14:17:26.395428 fabric-credmgr-client-1.6.0b8/test/test_credmgr_proxy.py
--rw-r--r--   0        0        0      949 2023-07-17 14:21:20.038470 fabric-credmgr-client-1.6.0b8/test/test_decoded_token.py
--rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b8/test/test_default_api.py
--rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b8/test/test_jwks.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b8/test/test_jwks_keys.py
--rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b8/test/test_request.py
--rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b8/test/test_revoke_list.py
--rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b8/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b8/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b8/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b8/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b8/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b8/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b8/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b8/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b8/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b8/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b8/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b8/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b8/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b8/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b8/test/test_token.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b8/test/test_tokens.py
--rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b8/test/test_tokens_api.py
--rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b8/test/test_version.py
--rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b8/test/test_version_api.py
--rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b8/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b8/tox.ini
--rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b8/PKG-INFO
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b9/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b9/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b9/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b9/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b9/LICENSE
+-rw-r--r--   0        0        0     4941 2023-07-25 19:41:10.336694 fabric-credmgr-client-1.6.0b9/README.md
+-rw-r--r--   0        0        0      329 2023-07-17 13:35:48.694756 fabric-credmgr-client-1.6.0b9/docs/DecodedToken.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b9/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b9/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b9/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b9/docs/Request.md
+-rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b9/docs/RevokeList.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b9/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b9/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b9/docs/Status200OkPaginated.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b9/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b9/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b9/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b9/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b9/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b9/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b9/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b9/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b9/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b9/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b9/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b9/docs/Success.md
+-rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b9/docs/Token.md
+-rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b9/docs/TokenPost.md
+-rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b9/docs/Tokens.md
+-rw-r--r--   0        0        0    12847 2023-07-26 16:08:53.625902 fabric-credmgr-client-1.6.0b9/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b9/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b9/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b9/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-07-26 20:18:28.906933 fabric-credmgr-client-1.6.0b9/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0    13111 2023-07-26 18:40:00.606510 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2060 2023-07-26 15:37:13.962587 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/session_helper.py
+-rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    30241 2023-07-26 18:46:26.266396 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25264 2023-07-26 20:17:22.851777 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2466 2023-07-17 13:34:51.161528 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3472 2023-07-17 13:38:26.234277 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/decoded_token.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/revoke_list.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/token_post.py
+-rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b9/git_push.sh
+-rw-r--r--   0        0        0     1129 2023-07-25 18:45:35.707490 fabric-credmgr-client-1.6.0b9/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b9/test/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-26 14:17:26.395428 fabric-credmgr-client-1.6.0b9/test/test_credmgr_proxy.py
+-rw-r--r--   0        0        0      949 2023-07-17 14:21:20.038470 fabric-credmgr-client-1.6.0b9/test/test_decoded_token.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b9/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b9/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b9/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b9/test/test_request.py
+-rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b9/test/test_revoke_list.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b9/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b9/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b9/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b9/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b9/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b9/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b9/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b9/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b9/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b9/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b9/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b9/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b9/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b9/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b9/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b9/test/test_tokens.py
+-rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b9/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b9/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b9/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b9/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b9/tox.ini
+-rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b9/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.6.0b8/.gitignore` & `fabric-credmgr-client-1.6.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/.swagger-codegen-ignore` & `fabric-credmgr-client-1.6.0b9/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/LICENSE` & `fabric-credmgr-client-1.6.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/README.md` & `fabric-credmgr-client-1.6.0b9/README.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/DefaultApi.md` & `fabric-credmgr-client-1.6.0b9/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/JwksKeys.md` & `fabric-credmgr-client-1.6.0b9/docs/JwksKeys.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status200OkNoContent.md` & `fabric-credmgr-client-1.6.0b9/docs/Status200OkNoContent.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status400BadRequestErrors.md` & `fabric-credmgr-client-1.6.0b9/docs/Status400BadRequestErrors.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status401Unauthorized.md` & `fabric-credmgr-client-1.6.0b9/docs/Status401Unauthorized.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status403Forbidden.md` & `fabric-credmgr-client-1.6.0b9/docs/Status403Forbidden.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status404NotFound.md` & `fabric-credmgr-client-1.6.0b9/docs/Status404NotFound.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Status500InternalServerError.md` & `fabric-credmgr-client-1.6.0b9/docs/Status500InternalServerError.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/Token.md` & `fabric-credmgr-client-1.6.0b9/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/TokensApi.md` & `fabric-credmgr-client-1.6.0b9/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/docs/VersionApi.md` & `fabric-credmgr-client-1.6.0b9/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/session_helper.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/session_helper.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/tokens_api.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Contact: kthare10@unc.edu
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
+import logging
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
@@ -71,16 +72,19 @@
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'Swagger-Codegen/1.0.0/python'
 
     def __del__(self):
-        self.pool.close()
-        self.pool.join()
+        try:
+            self.pool.close()
+            self.pool.join()
+        except Exception as e:
+            logging.getLogger().error(f"Ignoring connexion pool error: {e}")
 
     @property
     def user_agent(self):
         """User agent for this API client"""
         return self.default_headers['User-Agent']
 
     @user_agent.setter
```

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/decoded_token.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/decoded_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/revoke_list.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/token.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/token_post.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/token_post.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.6.0b9/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/git_push.sh` & `fabric-credmgr-client-1.6.0b9/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/pyproject.toml` & `fabric-credmgr-client-1.6.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_credmgr_proxy.py` & `fabric-credmgr-client-1.6.0b9/test/test_credmgr_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_decoded_token.py` & `fabric-credmgr-client-1.6.0b9/test/test_decoded_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_default_api.py` & `fabric-credmgr-client-1.6.0b9/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_jwks.py` & `fabric-credmgr-client-1.6.0b9/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_jwks_keys.py` & `fabric-credmgr-client-1.6.0b9/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_request.py` & `fabric-credmgr-client-1.6.0b9/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_revoke_list.py` & `fabric-credmgr-client-1.6.0b9/test/test_revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b9/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b9/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b9/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.6.0b9/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.6.0b9/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b9/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b9/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b9/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.6.0b9/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b9/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status404_not_found.py` & `fabric-credmgr-client-1.6.0b9/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b9/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b9/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b9/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_token.py` & `fabric-credmgr-client-1.6.0b9/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_tokens.py` & `fabric-credmgr-client-1.6.0b9/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_tokens_api.py` & `fabric-credmgr-client-1.6.0b9/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_version.py` & `fabric-credmgr-client-1.6.0b9/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_version_api.py` & `fabric-credmgr-client-1.6.0b9/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/test/test_version_data.py` & `fabric-credmgr-client-1.6.0b9/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b8/PKG-INFO` & `fabric-credmgr-client-1.6.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.6.0b8
+Version: 1.6.0b9
 Summary: Fabric Control Framework
 Keywords: Fabric Credential Manager API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/fabric-credmgr-client-1.6.0b4.tar.gz` & `tmp/fabric-credmgr-client-1.6.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.6.0b4.tar", last modified: Mon Jul 17 15:15:18 2023, max compression
+gzip compressed data, was "fabric-credmgr-client-1.6.0b5.tar", last modified: Wed Jul 26 14:20:26 2023, max compression
```

## Comparing `fabric-credmgr-client-1.6.0b4.tar` & `fabric-credmgr-client-1.6.0b5.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b4/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b4/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b4/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b4/.travis.yml
--rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b4/LICENSE
--rw-r--r--   0        0        0     4901 2023-07-03 21:15:47.092949 fabric-credmgr-client-1.6.0b4/README.md
--rw-r--r--   0        0        0      329 2023-07-17 13:35:48.694756 fabric-credmgr-client-1.6.0b4/docs/DecodedToken.md
--rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b4/docs/DefaultApi.md
--rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b4/docs/Jwks.md
--rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b4/docs/JwksKeys.md
--rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b4/docs/Request.md
--rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b4/docs/RevokeList.md
--rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b4/docs/Status200OkNoContent.md
--rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b4/docs/Status200OkNoContentData.md
--rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b4/docs/Status200OkPaginated.md
--rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b4/docs/Status200OkSingle.md
--rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b4/docs/Status400BadRequest.md
--rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b4/docs/Status400BadRequestErrors.md
--rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b4/docs/Status401Unauthorized.md
--rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b4/docs/Status401UnauthorizedErrors.md
--rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b4/docs/Status403Forbidden.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b4/docs/Status403ForbiddenErrors.md
--rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b4/docs/Status404NotFound.md
--rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b4/docs/Status404NotFoundErrors.md
--rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b4/docs/Status500InternalServerError.md
--rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b4/docs/Status500InternalServerErrorErrors.md
--rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b4/docs/Success.md
--rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b4/docs/Token.md
--rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b4/docs/TokenPost.md
--rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b4/docs/Tokens.md
--rw-r--r--   0        0        0    12431 2023-07-17 13:37:07.207677 fabric-credmgr-client-1.6.0b4/docs/TokensApi.md
--rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b4/docs/Version.md
--rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b4/docs/VersionApi.md
--rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b4/docs/VersionData.md
--rw-r--r--   0        0        0       50 2023-07-17 15:04:17.490159 fabric-credmgr-client-1.6.0b4/fabric_cm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/__init__.py
--rw-r--r--   0        0        0    10628 2023-07-17 15:10:09.527618 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/credmgr_proxy.py
--rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/__init__.py
--rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0        0        0    29435 2023-07-17 13:34:13.902087 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25120 2023-07-05 15:48:03.304939 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/configuration.py
--rw-r--r--   0        0        0     2466 2023-07-17 13:34:51.161528 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3472 2023-07-17 13:38:26.234277 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/decoded_token.py
--rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/revoke_list.py
--rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/token_post.py
--rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b4/git_push.sh
--rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.6.0b4/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b4/test/__init__.py
--rw-r--r--   0        0        0      949 2023-07-17 14:21:20.038470 fabric-credmgr-client-1.6.0b4/test/test_decoded_token.py
--rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b4/test/test_default_api.py
--rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b4/test/test_jwks.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b4/test/test_jwks_keys.py
--rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b4/test/test_request.py
--rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b4/test/test_revoke_list.py
--rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b4/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b4/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b4/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b4/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b4/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b4/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b4/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b4/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b4/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b4/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b4/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b4/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b4/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b4/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b4/test/test_token.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b4/test/test_tokens.py
--rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b4/test/test_tokens_api.py
--rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b4/test/test_version.py
--rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b4/test/test_version_api.py
--rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b4/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b4/tox.ini
--rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b4/PKG-INFO
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b5/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b5/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b5/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b5/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b5/LICENSE
+-rw-r--r--   0        0        0     4941 2023-07-25 19:41:10.336694 fabric-credmgr-client-1.6.0b5/README.md
+-rw-r--r--   0        0        0      329 2023-07-17 13:35:48.694756 fabric-credmgr-client-1.6.0b5/docs/DecodedToken.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b5/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b5/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b5/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b5/docs/Request.md
+-rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b5/docs/RevokeList.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b5/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b5/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b5/docs/Status200OkPaginated.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b5/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b5/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b5/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b5/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b5/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b5/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b5/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b5/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b5/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b5/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b5/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b5/docs/Success.md
+-rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b5/docs/Token.md
+-rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b5/docs/TokenPost.md
+-rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b5/docs/Tokens.md
+-rw-r--r--   0        0        0    12639 2023-07-25 19:40:33.987285 fabric-credmgr-client-1.6.0b5/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b5/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b5/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b5/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-07-26 14:20:03.152764 fabric-credmgr-client-1.6.0b5/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0    12721 2023-07-26 14:11:37.443677 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2060 2023-07-26 14:11:37.449425 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/session_helper.py
+-rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    29780 2023-07-25 23:42:29.251196 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25120 2023-07-25 23:33:20.373712 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2466 2023-07-17 13:34:51.161528 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3472 2023-07-17 13:38:26.234277 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/decoded_token.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/revoke_list.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/token_post.py
+-rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b5/git_push.sh
+-rw-r--r--   0        0        0     1129 2023-07-25 18:45:35.707490 fabric-credmgr-client-1.6.0b5/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b5/test/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-26 14:17:26.395428 fabric-credmgr-client-1.6.0b5/test/test_credmgr_proxy.py
+-rw-r--r--   0        0        0      949 2023-07-17 14:21:20.038470 fabric-credmgr-client-1.6.0b5/test/test_decoded_token.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b5/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b5/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b5/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b5/test/test_request.py
+-rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b5/test/test_revoke_list.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b5/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b5/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b5/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b5/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b5/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b5/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b5/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b5/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b5/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b5/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b5/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b5/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b5/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b5/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b5/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b5/test/test_tokens.py
+-rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b5/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b5/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b5/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b5/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b5/tox.ini
+-rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b5/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.6.0b4/.gitignore` & `fabric-credmgr-client-1.6.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/.swagger-codegen-ignore` & `fabric-credmgr-client-1.6.0b5/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/LICENSE` & `fabric-credmgr-client-1.6.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/README.md` & `fabric-credmgr-client-1.6.0b5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 *TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a token for an user
 *TokensApi* | [**tokens_revokes_post**](docs/TokensApi.md#tokens_revokes_post) | **POST** /tokens/revokes | Revoke a token
 *TokensApi* | [**tokens_validate_post**](docs/TokensApi.md#tokens_validate_post) | **POST** /tokens/validate | Validate an identity token issued by Credential Manager
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
+ - [DecodedToken](docs/DecodedToken.md)
  - [Jwks](docs/Jwks.md)
  - [JwksKeys](docs/JwksKeys.md)
  - [Request](docs/Request.md)
  - [RevokeList](docs/RevokeList.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
  - [Status200OkPaginated](docs/Status200OkPaginated.md)
```

### Comparing `fabric-credmgr-client-1.6.0b4/docs/DefaultApi.md` & `fabric-credmgr-client-1.6.0b5/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/JwksKeys.md` & `fabric-credmgr-client-1.6.0b5/docs/JwksKeys.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status200OkNoContent.md` & `fabric-credmgr-client-1.6.0b5/docs/Status200OkNoContent.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status400BadRequestErrors.md` & `fabric-credmgr-client-1.6.0b5/docs/Status400BadRequestErrors.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status401Unauthorized.md` & `fabric-credmgr-client-1.6.0b5/docs/Status401Unauthorized.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status403Forbidden.md` & `fabric-credmgr-client-1.6.0b5/docs/Status403Forbidden.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status404NotFound.md` & `fabric-credmgr-client-1.6.0b5/docs/Status404NotFound.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Status500InternalServerError.md` & `fabric-credmgr-client-1.6.0b5/docs/Status500InternalServerError.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/Token.md` & `fabric-credmgr-client-1.6.0b5/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/docs/TokensApi.md` & `fabric-credmgr-client-1.6.0b5/docs/TokensApi.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [**tokens_refresh_post**](TokensApi.md#tokens_refresh_post) | **POST** /tokens/refresh | Refresh tokens for an user
 [**tokens_revoke_list_get**](TokensApi.md#tokens_revoke_list_get) | **GET** /tokens/revoke_list | Get token revoke list i.e. list of revoked identity token hashes
 [**tokens_revoke_post**](TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a token for an user
 [**tokens_revokes_post**](TokensApi.md#tokens_revokes_post) | **POST** /tokens/revokes | Revoke a token
 [**tokens_validate_post**](TokensApi.md#tokens_validate_post) | **POST** /tokens/validate | Validate an identity token issued by Credential Manager
 
 # **tokens_create_post**
-> Tokens tokens_create_post(project_id=project_id, scope=scope, lifetime=lifetime, comment=comment)
+> Tokens tokens_create_post(project_id=project_id, project_name=project_name, scope=scope, lifetime=lifetime, comment=comment)
 
 Generate tokens for an user
 
 Request to generate tokens for an user 
 
 ### Example
 ```python
@@ -26,31 +26,33 @@
 from fabric_cm.credmgr.swagger_client import TokensApi
 from fabric_cm.credmgr.swagger_client.rest import ApiException
 from pprint import pprint
 
 # create an instance of the API class
 api_instance = TokensApi()
 project_id = 'project_id_example' # str | Project identified by universally unique identifier (optional)
+project_name = 'project_name_example' # str | Project identified by name (optional)
 scope = 'all' # str | Scope for which token is requested (optional) (default to all)
 lifetime = 4 # int | Lifetime of the token requested in hours (optional) (default to 4)
 comment = 'Create Token via GUI' # str | Comment (optional) (default to Create Token via GUI)
 
 try:
     # Generate tokens for an user
-    api_response = api_instance.tokens_create_post(project_id=project_id, scope=scope, lifetime=lifetime, comment=comment)
+    api_response = api_instance.tokens_create_post(project_id=project_id, project_name=project_name, scope=scope, lifetime=lifetime, comment=comment)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling TokensApi->tokens_create_post: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **project_id** | **str**| Project identified by universally unique identifier | [optional] 
+ **project_name** | **str**| Project identified by name | [optional] 
  **scope** | **str**| Scope for which token is requested | [optional] [default to all]
  **lifetime** | **int**| Lifetime of the token requested in hours | [optional] [default to 4]
  **comment** | **str**| Comment | [optional] [default to Create Token via GUI]
 
 ### Return type
 
 [**Tokens**](Tokens.md)
```

### Comparing `fabric-credmgr-client-1.6.0b4/docs/VersionApi.md` & `fabric-credmgr-client-1.6.0b5/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import json
 from datetime import datetime
 from typing import Tuple, Any, List, Union
 
 from atomicwrites import atomic_write
 
 from fabric_cm.credmgr import swagger_client
+from fabric_cm.credmgr.session_helper import SessionHelper
 from fabric_cm.credmgr.swagger_client import Token, TokenPost
 from fabric_cm.credmgr.swagger_client.models import DecodedToken
 from fabric_cm.credmgr.swagger_client.rest import ApiException as CredMgrException
 
 
 @enum.unique
 class Status(enum.Enum):
@@ -113,16 +114,20 @@
     REFRESH_TOKEN = "refresh_token"
     TIME_FORMAT = "%Y-%m-%d %H:%M:%S %z"
     CREATED_AT = "created_at"
     ERROR = "error"
     PROP_AUTHORIZATION = 'Authorization'
     PROP_BEARER = 'Bearer'
 
-    def __init__(self, credmgr_host: str):
+    def __init__(self, credmgr_host: str, cookie_name: str = "fabric-service",
+                 wait_timeout: int = 500, wait_interval: int = 5):
         self.host = credmgr_host
+        self.cookie_name = cookie_name
+        self.wait_timeout = wait_timeout
+        self.wait_interval = wait_interval
         self.tokens_api = None
         if credmgr_host is not None:
             # create an instance of the API class
             configuration = swagger_client.configuration.Configuration()
             configuration.host = f"https://{credmgr_host}/credmgr/"
             api_instance = swagger_client.ApiClient(configuration)
             self.tokens_api = swagger_client.TokensApi(api_client=api_instance)
@@ -134,14 +139,46 @@
         Set tokens
         @param token token
         """
         # Set the tokens
         self.tokens_api.api_client.configuration.api_key[self.PROP_AUTHORIZATION] = token
         self.tokens_api.api_client.configuration.api_key_prefix[self.PROP_AUTHORIZATION] = self.PROP_BEARER
 
+    def create(self, scope: str = "all", project_id: str = None, project_name: str = None, file_name: str = None,
+               life_time_in_hours: int = 4, comment: str = "Created via API",
+               browser_name: str = "chrome") -> Tuple[Status, Union[dict, Exception]]:
+        """
+        Create token
+        @param project_id Project Id
+        @param project_name Project Name
+        @param scope scope
+        @param file_name File name
+        @param life_time_in_hours Token lifetime in hours
+        @param comment comment associated with the token
+        @param browser_name Browser name; allowed values: chrome, firefox, safari, edge
+        @returns Tuple of Status, token json or Exception
+        @raises Exception in case of failure
+        """
+        try:
+            if project_id is None and project_name is None:
+                raise CredMgrException("Project ID or Project Name must be specified")
+            session = SessionHelper(url=f"https://{self.host}/", cookie_name=self.cookie_name,
+                                    wait_timeout=self.wait_timeout, wait_interval=self.wait_interval)
+            cookie = session.login(browser_name=browser_name)
+            self.tokens_api.api_client.cookie = cookie
+            tokens = self.tokens_api.tokens_create_post(project_id=project_id, project_name=project_name, scope=scope,
+                                                        lifetime=life_time_in_hours, comment=comment)
+            tokens_json = tokens.data[0].to_dict()
+            if file_name is not None:
+                with atomic_write(file_name, overwrite=True) as f:
+                    json.dump(tokens_json, f)
+            return Status.OK, tokens_json
+        except Exception as e:
+            return Status.FAILURE, e
+
     def refresh(self, project_id: str, scope: str, refresh_token: str,
                 file_name: str = None) -> Tuple[Status, dict]:
         """
         Refresh token
         @param project_id Project Id
         @param scope scope
         @param refresh_token refresh token
@@ -166,15 +203,16 @@
                 refresh_token = message.split(f"{self.REFRESH_TOKEN}:")[1]
                 refresh_token = refresh_token.strip()
                 refresh_token = refresh_token.strip("\"")
                 refresh_token = refresh_token.strip("\n")
                 tokens_json[self.REFRESH_TOKEN] = refresh_token
             return Status.FAILURE, tokens_json
 
-    def revoke(self, refresh_token: str, identity_token: str, token_type: TokenType = TokenType.Refresh) -> Tuple[Status, Any]:
+    def revoke(self, refresh_token: str, identity_token: str,
+               token_type: TokenType = TokenType.Refresh) -> Tuple[Status, Any]:
         """
         Revoke token
         @param refresh_token refresh token
         @param identity_token identity token
         @param token_type token type
         @returns response
         @raises Exception in case of failure
@@ -235,15 +273,16 @@
         try:
             version = self.version_api.version_get()
             return Status.OK, version
         except CredMgrException as e:
             return Status.FAILURE, e.body
 
     def tokens(self, *, token: str, project_id: str = None, expires: str = None, states: List[TokenState] = None,
-               limit: int = 200, offset: int = 0, token_hash: str = None,) -> Tuple[Status, Union[Exception, List[Token]]]:
+               limit: int = 200, offset: int = 0,
+               token_hash: str = None,) -> Tuple[Status, Union[Exception, List[Token]]]:
         """
         Return list of tokens issued to a user
         @return list of tokens
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, CredMgrException(f"Token {token} must be specified")
```

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/tokens_api.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/tokens_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.tokens_create_post(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id: Project identified by universally unique identifier
+        :param str project_name: Project identified by name
         :param str scope: Scope for which token is requested
         :param int lifetime: Lifetime of the token requested in hours
         :param str comment: Comment
         :return: Tokens
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -64,23 +65,25 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.tokens_create_post_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id: Project identified by universally unique identifier
+        :param str project_name: Project identified by name
         :param str scope: Scope for which token is requested
         :param int lifetime: Lifetime of the token requested in hours
         :param str comment: Comment
         :return: Tokens
                  If the method is called asynchronously,
                  returns the request thread.
         """
+        kwargs = {key: value for key, value in kwargs.items() if value is not None}
 
-        all_params = ['project_id', 'scope', 'lifetime', 'comment']  # noqa: E501
+        all_params = ['project_id', 'project_name', 'scope', 'lifetime', 'comment']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -95,14 +98,16 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'project_id' in params:
             query_params.append(('project_id', params['project_id']))  # noqa: E501
+        if 'project_name' in params:
+            query_params.append(('project_name', params['project_name']))  # noqa: E501
         if 'scope' in params:
             query_params.append(('scope', params['scope']))  # noqa: E501
         if 'lifetime' in params:
             query_params.append(('lifetime', params['lifetime']))  # noqa: E501
         if 'comment' in params:
             query_params.append(('comment', params['comment']))  # noqa: E501
```

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/decoded_token.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/decoded_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/revoke_list.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/token.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/token_post.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/token_post.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.6.0b5/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/git_push.sh` & `fabric-credmgr-client-1.6.0b5/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/pyproject.toml` & `fabric-credmgr-client-1.6.0b5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 requires-python = '>=3.9'
 dependencies = [
                 "certifi >= 14.05.14",
                 "six >= 1.10",
                 "python_dateutil >= 2.5.3",
                 "urllib3 >= 1.15.1",
-                "atomicwrites"
+                "atomicwrites",
+                "selenium"
                 ]
 
 [project.optional-dependencies]
 test = ["pytest",
         "coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
```

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_decoded_token.py` & `fabric-credmgr-client-1.6.0b5/test/test_decoded_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_default_api.py` & `fabric-credmgr-client-1.6.0b5/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_jwks.py` & `fabric-credmgr-client-1.6.0b5/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_jwks_keys.py` & `fabric-credmgr-client-1.6.0b5/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_request.py` & `fabric-credmgr-client-1.6.0b5/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_revoke_list.py` & `fabric-credmgr-client-1.6.0b5/test/test_revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b5/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b5/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b5/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.6.0b5/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.6.0b5/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b5/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b5/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b5/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.6.0b5/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b5/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status404_not_found.py` & `fabric-credmgr-client-1.6.0b5/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b5/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b5/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b5/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_token.py` & `fabric-credmgr-client-1.6.0b5/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_tokens.py` & `fabric-credmgr-client-1.6.0b5/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_tokens_api.py` & `fabric-credmgr-client-1.6.0b5/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_version.py` & `fabric-credmgr-client-1.6.0b5/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_version_api.py` & `fabric-credmgr-client-1.6.0b5/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/test/test_version_data.py` & `fabric-credmgr-client-1.6.0b5/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b4/PKG-INFO` & `fabric-credmgr-client-1.6.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: Fabric Control Framework
 Keywords: Fabric Credential Manager API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: certifi >= 14.05.14
 Requires-Dist: six >= 1.10
 Requires-Dist: python_dateutil >= 2.5.3
 Requires-Dist: urllib3 >= 1.15.1
 Requires-Dist: atomicwrites
+Requires-Dist: selenium
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
@@ -118,14 +119,15 @@
 *TokensApi* | [**tokens_revoke_post**](docs/TokensApi.md#tokens_revoke_post) | **POST** /tokens/revoke | Revoke a token for an user
 *TokensApi* | [**tokens_revokes_post**](docs/TokensApi.md#tokens_revokes_post) | **POST** /tokens/revokes | Revoke a token
 *TokensApi* | [**tokens_validate_post**](docs/TokensApi.md#tokens_validate_post) | **POST** /tokens/validate | Validate an identity token issued by Credential Manager
 *VersionApi* | [**version_get**](docs/VersionApi.md#version_get) | **GET** /version | Version
 
 ## Documentation For Models
 
+ - [DecodedToken](docs/DecodedToken.md)
  - [Jwks](docs/Jwks.md)
  - [JwksKeys](docs/JwksKeys.md)
  - [Request](docs/Request.md)
  - [RevokeList](docs/RevokeList.md)
  - [Status200OkNoContent](docs/Status200OkNoContent.md)
  - [Status200OkNoContentData](docs/Status200OkNoContentData.md)
  - [Status200OkPaginated](docs/Status200OkPaginated.md)
```


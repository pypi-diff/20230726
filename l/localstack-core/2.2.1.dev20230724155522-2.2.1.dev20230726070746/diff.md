# Comparing `tmp/localstack-core-2.2.1.dev20230724155522.tar.gz` & `tmp/localstack-core-2.2.1.dev20230726070746.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.2.1.dev20230724155522.tar", last modified: Mon Jul 24 15:55:30 2023, max compression
+gzip compressed data, was "localstack-core-2.2.1.dev20230726070746.tar", last modified: Wed Jul 26 07:07:55 2023, max compression
```

## Comparing `localstack-core-2.2.1.dev20230724155522.tar` & `localstack-core-2.2.1.dev20230726070746.tar`

### file list

```diff
@@ -1,879 +1,879 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-24 15:55:22.000000 localstack-core-2.2.1.dev20230724155522/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.085532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86817 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   760811 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.089532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.093532 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.097532 localstack-core-2.2.1.dev20230724155522/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.101532 localstack-core-2.2.1.dev20230724155522/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.101532 localstack-core-2.2.1.dev20230724155522/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.101532 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82038 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.101532 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24628 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.101532 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.105532 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20012 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.105532 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155991 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.105532 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.105532 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10776 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15563 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.109532 localstack-core-2.2.1.dev20230724155522/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.113532 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2432 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    95774 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35553 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16887 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.117532 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.121532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1379 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.125532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.129532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.133532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.133532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.133532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.133532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.137532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.137532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.137532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.141532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.141532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.141532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.141532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.145532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.149532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.149532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.149532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.153532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.153532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10836 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.153532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.153532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.153532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.157532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4916 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8018 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.161532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7185 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.165532 localstack-core-2.2.1.dev20230724155522/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.169532 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.169532 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69946 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.169532 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.173532 localstack-core-2.2.1.dev20230724155522/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.173532 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17402 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7639 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24011 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47223 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33214 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-24 15:55:29.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39367 2023-07-24 15:55:30.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-24 15:55:29.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-24 15:55:29.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-24 15:55:26.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-24 15:55:26.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-24 15:55:29.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-24 15:55:29.000000 localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-24 15:55:30.177532 localstack-core-2.2.1.dev20230724155522/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-24 15:23:19.000000 localstack-core-2.2.1.dev20230724155522/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 07:07:55.370521 localstack-core-2.2.1.dev20230726070746/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.270521 localstack-core-2.2.1.dev20230726070746/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.270521 localstack-core-2.2.1.dev20230726070746/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-26 07:07:46.000000 localstack-core-2.2.1.dev20230726070746/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   760811 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82038 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24628 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155991 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2432 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    95774 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16887 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1379 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.322521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.322521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.334521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.334521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10836 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4916 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8018 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7185 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.358521 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69331 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.358521 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17676 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24011 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47223 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33214 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39367 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 07:07:51.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-26 07:07:51.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-26 07:07:55.370521 localstack-core-2.2.1.dev20230726070746/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/setup.py
```

### Comparing `localstack-core-2.2.1.dev20230724155522/LICENSE.txt` & `localstack-core-2.2.1.dev20230726070746/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/Makefile` & `localstack-core-2.2.1.dev20230726070746/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/PKG-INFO` & `localstack-core-2.2.1.dev20230726070746/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230724155522
+Version: 2.2.1.dev20230726070746
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230724155522/README.md` & `localstack-core-2.2.1.dev20230726070746/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/bin/localstack` & `localstack-core-2.2.1.dev20230726070746/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/bin/localstack-supervisor` & `localstack-core-2.2.1.dev20230726070746/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/accounts.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/acm/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/config/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/core.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/es/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/events/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/iam/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/kms/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/logs/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ses/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sns/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/sts/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/support/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/swf/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/app.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/chain.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/connect.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 
     def __init__(
         self, *, factory: "ClientFactory", client_creation_params: dict[str, str | Config | None]
     ):
         self._factory = factory
         self._client_creation_params = client_creation_params
 
+    def get_client(self, service: str):
+        return MetadataRequestInjector(
+            client=self._factory.get_client(service_name=service, **self._client_creation_params)
+        )
+
     def __getattr__(self, service: str):
         service = attribute_name_to_service_name(service)
         return MetadataRequestInjector(
             client=self._factory.get_client(service_name=service, **self._client_creation_params)
         )
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/forwarder.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/gateway.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/analytics.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/auth.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/codec.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/cors.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/fallback.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/internal.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/legacy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/logging.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/proxy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/region.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/routes.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/service.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/mocking.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/op_router.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/parser.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/serializer.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/service_router.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/protocol/validate.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/proxy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/scaffold.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/asgi.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/edge.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/hypercorn.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/werkzeug.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/serving/wsgi.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/skeleton.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/spec-patches.json` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/spec.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/aws/trace.py` & `localstack-core-2.2.1.dev20230726070746/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/cli/localstack.py` & `localstack-core-2.2.1.dev20230726070746/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/cli/lpm.py` & `localstack-core-2.2.1.dev20230726070746/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/cli/plugin.py` & `localstack-core-2.2.1.dev20230726070746/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/cli/plugins.py` & `localstack-core-2.2.1.dev20230726070746/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/cli/profiles.py` & `localstack-core-2.2.1.dev20230726070746/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/config.py` & `localstack-core-2.2.1.dev20230726070746/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/constants.py` & `localstack-core-2.2.1.dev20230726070746/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/deprecations.py` & `localstack-core-2.2.1.dev20230726070746/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/aws.py` & `localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/extensions/api/extension.py` & `localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/adapters.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/asgi.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/dispatcher.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/hypercorn.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/proxy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/request.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/resource.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/response.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/http/router.py` & `localstack-core-2.2.1.dev20230726070746/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/logging/format.py` & `localstack-core-2.2.1.dev20230726070746/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/logging/setup.py` & `localstack-core-2.2.1.dev20230726070746/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/__init__.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/api.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/core.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/debugpy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/ffmpeg.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/packages/terraform.py` & `localstack-core-2.2.1.dev20230726070746/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/plugins.py` & `localstack-core-2.2.1.dev20230726070746/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/runtime/analytics.py` & `localstack-core-2.2.1.dev20230726070746/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/runtime/hooks.py` & `localstack-core-2.2.1.dev20230726070746/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/runtime/init.py` & `localstack-core-2.2.1.dev20230726070746/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/runtime/main.py` & `localstack-core-2.2.1.dev20230726070746/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/runtime/shutdown.py` & `localstack-core-2.2.1.dev20230726070746/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/acm/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/context.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/helpers.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/integration.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/invocations.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/patches.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/router_asf.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/apigateway/templates.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/api_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/hooks.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/plugins.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/deploy.html` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/events.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/service_models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudformation/stores.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,16 @@
         if task:
             task.cancel()
 
     def restart_existing_alarms(self) -> None:
         """
         Only used re-create persistent state. Reschedules alarms that already exist
         """
-        service = "cloudwatch"
-        for region in aws_stack.get_valid_regions_for_service(service):
-            client = connect_to(region_name=region).get_client(service)
+        for region in aws_stack.get_valid_regions_for_service("cloudwatch"):
+            client = connect_to(region_name=region).cloudwatch
             result = client.describe_alarms()
             for metric_alarm in result["MetricAlarms"]:
                 arn = metric_alarm["AlarmArn"]
                 self.schedule_metric_alarm(alarm_arn=arn)
 
     def _is_alarm_supported(self, alarm_details: MetricAlarm) -> bool:
         required_parameters = ["Period", "Statistic", "MetricName", "Threshold"]
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/cloudwatch/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/server.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodb/utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/exceptions.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ec2/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/edge.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/es/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/events/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/events/scheduler.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/mappers.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/firehose/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/generic_proxy.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/iam/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/infra.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/internal.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kinesis/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/local_kms_server.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/kms/utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/logs/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/logs/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/messages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/moto.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/motoserver.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/cluster.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/opensearch/versions.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/plugins.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/providers.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/redshift/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/route53/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/route53resolver/utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/constants.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/cors.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/multipart_content.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/notifications.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/presigned_url.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/provider_stream.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_starter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/s3_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/virtual_host.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/s3/website_hosting.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/secretsmanager/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ses/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sns/constants.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sns/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sns/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sns/publisher.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/constants.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/exceptions.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/query_api.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sqs/utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/packages.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/stores.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/sts/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/services/transcribe/provider.py` & `localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/state/core.py` & `localstack-core-2.2.1.dev20230726070746/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/state/inspect.py` & `localstack-core-2.2.1.dev20230726070746/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/state/pickle.py` & `localstack-core-2.2.1.dev20230726070746/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/state/snapshot.py` & `localstack-core-2.2.1.dev20230726070746/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/asf_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/aws/util.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/filters.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/fixtures.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,39 @@
 import logging
 import os
 import re
 import socket
 import time
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
-import boto3
 import botocore.auth
 import botocore.config
 import botocore.credentials
 import botocore.session
 import pytest
 from _pytest.config import Config
 from _pytest.nodes import Item
 from botocore.exceptions import ClientError
 from botocore.regions import EndpointResolver
 from moto.core import BackendDict, BaseBackend
 from pytest_httpserver import HTTPServer
 from werkzeug import Request, Response
 
 from localstack import config, constants
-from localstack.aws.accounts import get_aws_account_id
 from localstack.constants import TEST_AWS_ACCESS_KEY_ID, TEST_AWS_SECRET_ACCESS_KEY
 from localstack.services.stores import (
     AccountRegionBundle,
     BaseStore,
     CrossAccountAttribute,
     CrossRegionAttribute,
     LocalAttribute,
 )
 from localstack.testing.aws.cloudformation_utils import load_template_file, render_template
 from localstack.testing.aws.util import get_lambda_logs, is_aws_cloud
 from localstack.utils import testutil
-from localstack.utils.aws import aws_stack
 from localstack.utils.aws.client import SigningHttpClient
 from localstack.utils.aws.resources import create_dynamodb_table
 from localstack.utils.collections import ensure_list
 from localstack.utils.functions import run_safe
 from localstack.utils.http import safe_requests as requests
 from localstack.utils.json import CustomEncoder, json_safe
 from localstack.utils.net import wait_for_port_open
@@ -49,55 +46,16 @@
 
 LOG = logging.getLogger(__name__)
 
 # URL of public HTTP echo server, used primarily for AWS parity/snapshot testing
 PUBLIC_HTTP_ECHO_SERVER_URL = "http://httpbin.org"
 
 
-def _resource(service):
-    if os.environ.get("TEST_TARGET") == "AWS_CLOUD":
-        return boto3.resource(service)
-    # can't set the timeouts to 0 like in the AWS CLI because the underlying http client requires values > 0
-    config = (
-        botocore.config.Config(
-            connect_timeout=1_000, read_timeout=1_000, retries={"total_max_attempts": 1}
-        )
-        if os.environ.get("TEST_DISABLE_RETRIES_AND_TIMEOUTS")
-        else None
-    )
-    return aws_stack.connect_to_resource_external(service, config=config)
-
-
-# TODO: remove usage of this fixture
 @pytest.fixture(scope="class")
-def create_boto_client(aws_client_factory):
-    def _factory_client(
-        service, region_name=None, aws_access_key_id=None, *, additional_config=None
-    ):
-        return aws_client_factory.get_client(
-            service_name=service, region_name=region_name, config=additional_config
-        )
-
-    return _factory_client
-
-
-@pytest.fixture(scope="class")
-def boto3_session():
-    if os.environ.get("TEST_TARGET", "") == "AWS_CLOUD":
-        return boto3.Session()
-
-    return boto3.Session(
-        # LocalStack assumes AWS_ACCESS_KEY_ID config contains the AWS_ACCOUNT_ID value.
-        aws_access_key_id=get_aws_account_id(),
-        aws_secret_access_key="__test_key__",
-    )
-
-
-@pytest.fixture(scope="class")
-def aws_http_client_factory(boto3_session):
+def aws_http_client_factory(aws_session):
     """
     Returns a factory for creating new ``SigningHttpClient`` instances using a configurable botocore request signer.
     The default signer is a SigV4QueryAuth. The credentials are extracted from the ``boto3_sessions`` fixture that
     transparently uses your global profile when TEST_TARGET=AWS_CLOUD, or test credentials when running against
     LocalStack.
 
     Example invocations
@@ -116,64 +74,52 @@
         signer_factory: Callable[
             [botocore.credentials.Credentials, str, str], botocore.auth.BaseSigner
         ] = botocore.auth.SigV4QueryAuth,
         endpoint_url: str = None,
         aws_access_key_id: str = None,
         aws_secret_access_key: str = None,
     ):
-        region = region or boto3_session.region_name
+        region = region or aws_session.region_name
         region = region or config.DEFAULT_REGION
 
         if aws_access_key_id or aws_secret_access_key:
             credentials = botocore.credentials.Credentials(
                 access_key=aws_access_key_id, secret_key=aws_secret_access_key
             )
         else:
-            credentials = boto3_session.get_credentials()
+            credentials = aws_session.get_credentials()
 
         creds = credentials.get_frozen_credentials()
 
         if not endpoint_url:
             if os.environ.get("TEST_TARGET", "") == "AWS_CLOUD":
                 # FIXME: this is a bit raw. we should probably re-use boto in a better way
-                resolver: EndpointResolver = boto3_session._session.get_component(
-                    "endpoint_resolver"
-                )
+                resolver: EndpointResolver = aws_session._session.get_component("endpoint_resolver")
                 endpoint_url = "https://" + resolver.construct_endpoint(service, region)["hostname"]
             else:
                 endpoint_url = config.get_edge_url()
 
         return SigningHttpClient(signer_factory(creds, service, region), endpoint_url=endpoint_url)
 
     return factory
 
 
 @pytest.fixture(scope="class")
-def dynamodb_resource():
-    return _resource("dynamodb")
-
-
-@pytest.fixture(scope="class")
 def s3_vhost_client(aws_client_factory):
     return aws_client_factory(config=botocore.config.Config(s3={"addressing_style": "virtual"})).s3
 
 
 # TODO: remove
 @pytest.fixture(scope="class")
 def s3_presigned_client(aws_client_factory):
     return aws_client_factory(
         aws_access_key_id=TEST_AWS_ACCESS_KEY_ID, aws_secret_access_key=TEST_AWS_SECRET_ACCESS_KEY
     ).s3
 
 
-@pytest.fixture(scope="class")
-def s3_resource():
-    return _resource("s3")
-
-
 @pytest.fixture
 def dynamodb_wait_for_table_active(aws_client):
     def wait_for_table_active(table_name: str, client=None):
         def wait():
             return (client or aws_client.dynamodb).describe_table(TableName=table_name)["Table"][
                 "TableStatus"
             ] == "ACTIVE"
@@ -233,15 +179,15 @@
             dynamodb_wait_for_table_active(table)
             aws_client.dynamodb.delete_table(TableName=table)
         except Exception as e:
             LOG.debug("error cleaning up table %s: %s", table, e)
 
 
 @pytest.fixture
-def s3_create_bucket(s3_resource, aws_client):
+def s3_create_bucket(s3_empty_bucket, aws_client):
     buckets = []
 
     def factory(**kwargs) -> str:
         if "Bucket" not in kwargs:
             kwargs["Bucket"] = "test-bucket-%s" % short_uid()
 
         if (
@@ -257,32 +203,53 @@
         return kwargs["Bucket"]
 
     yield factory
 
     # cleanup
     for bucket in buckets:
         try:
-            bucket = s3_resource.Bucket(bucket)
-            bucket.objects.all().delete()
-            bucket.object_versions.all().delete()
-            bucket.delete()
+            s3_empty_bucket(bucket)
+            aws_client.s3.delete_bucket(Bucket=bucket)
         except Exception as e:
             LOG.debug("error cleaning up bucket %s: %s", bucket, e)
 
 
 @pytest.fixture
 def s3_bucket(s3_create_bucket, aws_client) -> str:
     region = aws_client.s3.meta.region_name
     kwargs = {}
     if region != "us-east-1":
         kwargs["CreateBucketConfiguration"] = {"LocationConstraint": region}
     return s3_create_bucket(**kwargs)
 
 
 @pytest.fixture
+def s3_empty_bucket(aws_client):
+    """
+    Returns a factory that given a bucket name, deletes all objects and deletes all object versions
+    """
+    # Boto resource would make this a straightforward task, but our internal client does not support Boto resource
+    # FIXME: this won't work when bucket has more than 1000 objects
+    def factory(bucket_name: str):
+        response = aws_client.s3.list_objects_v2(Bucket=bucket_name)
+        objects = [{"Key": obj["Key"]} for obj in response["Contents"]]
+        aws_client.s3.delete_objects(Bucket=bucket_name, Delete={"Objects": objects})
+
+        response = aws_client.s3.list_object_versions(Bucket=bucket_name)
+        object_versions = [
+            {"Key": obj["Key"], "VersionId": obj["VersionId"]}
+            for obj in response.get("Versions", [])
+        ]
+        if object_versions:
+            aws_client.s3.delete_objects(Bucket=bucket_name, Delete={"Objects": object_versions})
+
+    yield factory
+
+
+@pytest.fixture
 def sqs_create_queue(aws_client):
     queue_urls = []
 
     def factory(**kwargs):
         if "QueueName" not in kwargs:
             kwargs["QueueName"] = "test-queue-%s" % short_uid()
 
@@ -689,57 +656,60 @@
 
         return poll_condition(is_stream_ready)
 
     return _wait_for_stream_ready
 
 
 @pytest.fixture()
-def kms_create_key(create_boto_client):
+def kms_create_key(aws_client_factory):
     key_ids = []
 
-    def _create_key(region=None, **kwargs):
+    def _create_key(region_name: str = None, **kwargs):
         if "Description" not in kwargs:
             kwargs["Description"] = f"test description - {short_uid()}"
-        key_metadata = create_boto_client("kms", region).create_key(**kwargs)["KeyMetadata"]
-        key_ids.append((region, key_metadata["KeyId"]))
+        key_metadata = aws_client_factory(region_name=region_name).kms.create_key(**kwargs)[
+            "KeyMetadata"
+        ]
+        key_ids.append((region_name, key_metadata["KeyId"]))
         return key_metadata
 
     yield _create_key
 
-    for region, key_id in key_ids:
+    for region_name, key_id in key_ids:
         try:
+
             # shortest amount of time you can schedule the deletion
-            create_boto_client("kms", region).schedule_key_deletion(
+            aws_client_factory(region_name=region_name).kms.schedule_key_deletion(
                 KeyId=key_id, PendingWindowInDays=7
             )
         except Exception as e:
             exception_message = str(e)
             # Some tests schedule their keys for deletion themselves.
             if (
                 "KMSInvalidStateException" not in exception_message
                 or "is pending deletion" not in exception_message
             ):
                 LOG.debug("error cleaning up KMS key %s: %s", key_id, e)
 
 
 @pytest.fixture()
-def kms_replicate_key(create_boto_client):
+def kms_replicate_key(aws_client_factory):
     key_ids = []
 
     def _replicate_key(region_from=None, **kwargs):
         region_to = kwargs.get("ReplicaRegion")
         key_ids.append((region_to, kwargs.get("KeyId")))
-        return create_boto_client("kms", region_from).replicate_key(**kwargs)
+        return aws_client_factory(region_name=region_from).kms.replicate_key(**kwargs)
 
     yield _replicate_key
 
     for region_to, key_id in key_ids:
         try:
             # shortest amount of time you can schedule the deletion
-            create_boto_client("kms", region_to).schedule_key_deletion(
+            aws_client_factory(region_name=region_to).kms.schedule_key_deletion(
                 KeyId=key_id, PendingWindowInDays=7
             )
         except Exception as e:
             LOG.debug("error cleaning up KMS key %s: %s", key_id, e)
 
 
 # kms_create_key fixture is used here not just to be able to create aliases without a key specified,
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/snapshot.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/pytest/util.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/prototype.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/report.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/transformer.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,40 @@
                 "$..s3.object.versionId",
                 "version-id",
                 reference_replacement=False,
             ),
         ]
 
     @staticmethod
+    def s3_dynamodb_notifications():
+        return [
+            TransformerUtility.jsonpath("$..uuid.S", "uuid"),
+            TransformerUtility.jsonpath("$..M.requestParameters.M.sourceIPAddress.S", "ip-address"),
+            TransformerUtility.jsonpath(
+                "$..M.responseElements.M.x-amz-id-2.S", "amz-id", reference_replacement=False
+            ),
+            TransformerUtility.jsonpath(
+                "$..M.responseElements.M.x-amz-request-id.S",
+                "amz-request-id",
+                reference_replacement=False,
+            ),
+            TransformerUtility.jsonpath("$..M.s3.M.bucket.M.name.S", "bucket-name"),
+            TransformerUtility.jsonpath("$..M.s3.M.bucket.M.arn.S", "bucket-arn"),
+            TransformerUtility.jsonpath(
+                "$..M.s3.M.bucket.M.ownerIdentity.M.principalId.S", "principal-id"
+            ),
+            TransformerUtility.jsonpath("$..M.s3.M.configurationId.S", "config-id"),
+            TransformerUtility.jsonpath("$..M.s3.M.object.M.key.S", "object-key"),
+            TransformerUtility.jsonpath(
+                "$..M.s3.M.object.M.sequencer.S", "sequencer", reference_replacement=False
+            ),
+            TransformerUtility.jsonpath("$..M.userIdentity.M.principalId.S", "principal-id"),
+        ]
+
+    @staticmethod
     def kinesis_api():
         """
         :return: array with Transformers, for kinesis api.
         """
         return [
             JsonpathTransformer(
                 jsonpath="$..Records..SequenceNumber",
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/cli.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/events.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/logger.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/metadata.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/publisher.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/analytics/usage.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/archives.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/asyncio.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/auth.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/arns.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_models.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_responses.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/aws_stack.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 import json
 import logging
 import os
 import re
 import socket
 import threading
+import warnings
 from functools import lru_cache
 from typing import Dict, Optional, Union
 
 import boto3
 import botocore
 import botocore.config
 
@@ -222,14 +223,18 @@
 
 def connect_to_resource(
     service_name, env=None, region_name=None, endpoint_url=None, *args, **kwargs
 ):
     """
     Generic method to obtain an AWS service resource using boto3, based on environment, region, or custom endpoint_url.
     """
+    warnings.warn(
+        "`connect_to_resource` is obsolete. Use `localstack.aws.connect`", DeprecationWarning
+    )
+
     return connect_to_service(
         service_name,
         client=False,
         env=env,
         region_name=region_name,
         endpoint_url=endpoint_url,
         *args,
@@ -244,14 +249,19 @@
     endpoint_url=None,
     config: botocore.config.Config = None,
     **kwargs,
 ):
     """
     Generic method to obtain an AWS service resource using boto3, based on environment, region, or custom endpoint_url.
     """
+    warnings.warn(
+        "`connect_to_resource_external` is obsolete. Use `localstack.aws.connect`",
+        DeprecationWarning,
+    )
+
     return create_external_boto_client(
         service_name,
         client=False,
         env=env,
         region_name=region_name,
         endpoint_url=endpoint_url,
         config=config,
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/client_types.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/queries.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/request_context.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/resources.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     region = s3_client.meta.region_name
     kwargs = {}
     if region != AWS_REGION_US_EAST_1:
         kwargs = {"CreateBucketConfiguration": {"LocationConstraint": region}}
     return s3_client.create_bucket(Bucket=bucket_name, **kwargs)
 
 
+# TODO: convert this into a fixture?
 def create_dynamodb_table(
     table_name: str,
     partition_key: str,
     stream_view_type: str = None,
     region_name: str = None,
     client=None,
     wait_for_active: bool = True,
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/aws/templating.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/bootstrap.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/collections.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/common.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/config_listener.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/container_networking.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/container_client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/coverage_docs.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/crypto.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/diagnose.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/docker_utils.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/files.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/functions.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/http.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/json.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/net.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/numbers.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/objects.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/patch.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/platform.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/run.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/scheduler.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/server/http2_server.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/server/proxy_server.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/serving.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/ssl.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/strings.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/sync.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/tagging.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/tail.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/testutil.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/threads.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/time.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/urls.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/venv.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack/utils/xml.py` & `localstack-core-2.2.1.dev20230726070746/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230724155522
+Version: 2.2.1.dev20230726070746
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/plux.json` & `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8445862130072657%*

 * *Differences: {"'localstack.hooks.configure_localstack_container'": '{insert: [(1, '*

 * *                                                      "'_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file')], "*

 * *                                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown')], "*

 * *                                         ' […]*

```diff
@@ -47,48 +47,48 @@
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
         "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin",
         "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
-        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file",
-        "configure_edge_port=localstack.plugins:configure_edge_port"
+        "configure_edge_port=localstack.plugins:configure_edge_port",
+        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener"
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
-        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
-        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package"
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
+        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230724155522/localstack_core.egg-info/requires.txt` & `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/pyproject.toml` & `localstack-core-2.2.1.dev20230726070746/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230724155522/setup.cfg` & `localstack-core-2.2.1.dev20230726070746/setup.cfg`

 * *Files identical despite different names*


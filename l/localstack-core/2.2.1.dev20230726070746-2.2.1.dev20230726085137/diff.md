# Comparing `tmp/localstack-core-2.2.1.dev20230726070746.tar.gz` & `tmp/localstack-core-2.2.1.dev20230726085137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.2.1.dev20230726070746.tar", last modified: Wed Jul 26 07:07:55 2023, max compression
+gzip compressed data, was "localstack-core-2.2.1.dev20230726085137.tar", last modified: Wed Jul 26 08:51:45 2023, max compression
```

## Comparing `localstack-core-2.2.1.dev20230726070746.tar` & `localstack-core-2.2.1.dev20230726085137.tar`

### file list

```diff
@@ -1,879 +1,879 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 07:07:55.370521 localstack-core-2.2.1.dev20230726070746/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.270521 localstack-core-2.2.1.dev20230726070746/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.270521 localstack-core-2.2.1.dev20230726070746/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-26 07:07:46.000000 localstack-core-2.2.1.dev20230726070746/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   760811 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.274521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.278521 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.282521 localstack-core-2.2.1.dev20230726070746/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.286521 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82038 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24628 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155991 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.290521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61875 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27391 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4654 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.294521 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.298521 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.302521 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2432 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    95774 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16887 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.306521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1379 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.310521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.318521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.322521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.322521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.330521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.334521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.334521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.338521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10836 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.342521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4916 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8018 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.346521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.350521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7185 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.354521 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.358521 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69331 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.358521 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17676 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24011 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47223 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33214 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.362521 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 07:07:55.366521 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39367 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 07:07:51.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-26 07:07:51.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-26 07:07:55.000000 localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-26 07:07:55.370521 localstack-core-2.2.1.dev20230726070746/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-26 06:31:59.000000 localstack-core-2.2.1.dev20230726070746/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.184181 localstack-core-2.2.1.dev20230726085137/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 08:51:45.184181 localstack-core-2.2.1.dev20230726085137/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.092183 localstack-core-2.2.1.dev20230726085137/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-26 08:51:37.000000 localstack-core-2.2.1.dev20230726085137/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86817 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.096183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   760811 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.100183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51460 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.104183 localstack-core-2.2.1.dev20230726085137/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.108182 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.108182 localstack-core-2.2.1.dev20230726085137/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.108182 localstack-core-2.2.1.dev20230726085137/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.108182 localstack-core-2.2.1.dev20230726085137/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.108182 localstack-core-2.2.1.dev20230726085137/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.112182 localstack-core-2.2.1.dev20230726085137/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.112182 localstack-core-2.2.1.dev20230726085137/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.112182 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15100 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82038 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.112182 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24628 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.112182 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.116182 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20012 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.116182 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155991 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.116182 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3628 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.116182 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12423 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50113 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21376 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2559 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7281 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2267 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5740 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21384 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3288 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9386 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27408 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3311 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2004 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3533 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4953 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1251 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3692 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13431 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6773 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5037 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10776 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5772 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41269 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27724 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5368 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5958 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.120182 localstack-core-2.2.1.dev20230726085137/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.124182 localstack-core-2.2.1.dev20230726085137/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2432 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    95774 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35553 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68151 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15009 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16887 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.128182 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.132182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1379 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.136182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.140182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.148182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.152182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.152182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.152182 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10836 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.156181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.160181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.160181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.160181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4916 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8018 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.164181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.168181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.168181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.168181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7185 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.172181 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.176181 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69331 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.176181 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17676 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24011 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47223 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33214 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.180181 localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.184181 localstack-core-2.2.1.dev20230726085137/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 08:51:45.184181 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-26 08:51:44.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39367 2023-07-26 08:51:45.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 08:51:44.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-26 08:51:44.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 08:51:41.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-26 08:51:41.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-26 08:51:44.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-26 08:51:44.000000 localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-26 08:51:45.184181 localstack-core-2.2.1.dev20230726085137/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-26 08:18:25.000000 localstack-core-2.2.1.dev20230726085137/setup.py
```

### Comparing `localstack-core-2.2.1.dev20230726070746/LICENSE.txt` & `localstack-core-2.2.1.dev20230726085137/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/Makefile` & `localstack-core-2.2.1.dev20230726085137/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/PKG-INFO` & `localstack-core-2.2.1.dev20230726085137/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230726070746
+Version: 2.2.1.dev20230726085137
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230726070746/README.md` & `localstack-core-2.2.1.dev20230726085137/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/bin/localstack` & `localstack-core-2.2.1.dev20230726085137/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/bin/localstack-supervisor` & `localstack-core-2.2.1.dev20230726085137/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/accounts.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/acm/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/config/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/core.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/es/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/events/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/iam/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/kms/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/logs/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ses/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sns/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/sts/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/support/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/swf/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/app.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/chain.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/connect.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/forwarder.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/gateway.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/analytics.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/auth.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/codec.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/cors.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/fallback.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/legacy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/logging.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/proxy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/region.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/routes.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/mocking.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/op_router.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/parser.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/serializer.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/service_router.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/protocol/validate.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/proxy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/scaffold.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/asgi.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/edge.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/hypercorn.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/werkzeug.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/serving/wsgi.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/skeleton.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/spec-patches.json` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/spec.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/aws/trace.py` & `localstack-core-2.2.1.dev20230726085137/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/cli/localstack.py` & `localstack-core-2.2.1.dev20230726085137/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/cli/lpm.py` & `localstack-core-2.2.1.dev20230726085137/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/cli/plugin.py` & `localstack-core-2.2.1.dev20230726085137/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/cli/plugins.py` & `localstack-core-2.2.1.dev20230726085137/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/cli/profiles.py` & `localstack-core-2.2.1.dev20230726085137/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/config.py` & `localstack-core-2.2.1.dev20230726085137/localstack/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1033,26 +1033,32 @@
 
 # Whether to return and parse access key ids starting with an "A", like on AWS
 PARITY_AWS_ACCESS_KEY_ID = is_env_true("PARITY_AWS_ACCESS_KEY_ID")
 
 # Show exceptions for CloudFormation deploy errors
 CFN_VERBOSE_ERRORS = is_env_true("CFN_VERBOSE_ERRORS")
 
+# How localstack will react to encountering unsupported resource types.
+# By default unsupported resource types will be ignored.
+# EXPERIMENTAL
+CFN_IGNORE_UNSUPPORTED_RESOURCE_TYPES = is_env_not_false("CFN_IGNORE_UNSUPPORTED_RESOURCE_TYPES")
+
 # Selectively enable/disable new resource providers
 # e.g. CFN_RESOURCE_PROVIDER_OVERRIDES='{"AWS::Lambda::Version": "GenericBaseModel","AWS::Lambda::Function": "ResourceProvider"}'
 CFN_RESOURCE_PROVIDER_OVERRIDES = os.environ.get("CFN_RESOURCE_PROVIDER_OVERRIDES", "{}")
 
 # HINT: Please add deprecated environment variables to deprecations.py
 
 # list of environment variable names used for configuration.
 # Make sure to keep this in sync with the above!
 # Note: do *not* include DATA_DIR in this list, as it is treated separately
 CONFIG_ENV_VARS = [
     "ALLOW_NONSTANDARD_REGIONS",
     "BUCKET_MARKER_LOCAL",
+    "CFN_IGNORE_UNSUPPORTED_RESOURCE_TYPES",
     "CFN_VERBOSE_ERRORS",
     "CFN_RESOURCE_PROVIDER_OVERRIDES",
     "CI",
     "CUSTOM_SSL_CERT_PATH",
     "DEBUG",
     "DEBUG_HANDLER_CHAIN",
     "DEFAULT_REGION",
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/constants.py` & `localstack-core-2.2.1.dev20230726085137/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/deprecations.py` & `localstack-core-2.2.1.dev20230726085137/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/aws.py` & `localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/extensions/api/extension.py` & `localstack-core-2.2.1.dev20230726085137/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/adapters.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/asgi.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/dispatcher.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/hypercorn.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/proxy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/request.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/resource.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/response.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/http/router.py` & `localstack-core-2.2.1.dev20230726085137/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/logging/format.py` & `localstack-core-2.2.1.dev20230726085137/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/logging/setup.py` & `localstack-core-2.2.1.dev20230726085137/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/__init__.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/api.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/core.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/debugpy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/ffmpeg.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/packages/terraform.py` & `localstack-core-2.2.1.dev20230726085137/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/plugins.py` & `localstack-core-2.2.1.dev20230726085137/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/runtime/analytics.py` & `localstack-core-2.2.1.dev20230726085137/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/runtime/hooks.py` & `localstack-core-2.2.1.dev20230726085137/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/runtime/init.py` & `localstack-core-2.2.1.dev20230726085137/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/runtime/main.py` & `localstack-core-2.2.1.dev20230726085137/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/runtime/shutdown.py` & `localstack-core-2.2.1.dev20230726085137/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/acm/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/context.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/helpers.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/integration.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/invocations.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/patches.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/router_asf.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/apigateway/templates.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/api_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/hooks.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/plugins.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deploy.html` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/deployment_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import builtins
 import json
 import logging
 import re
 from copy import deepcopy
 from typing import Callable, List
 
+from localstack import config
 from localstack.utils import common
 from localstack.utils.aws import aws_stack
 from localstack.utils.common import select_attributes, short_uid
 from localstack.utils.functions import run_safe
 from localstack.utils.json import json_safe
 from localstack.utils.objects import recurse_object
 from localstack.utils.strings import is_string
@@ -249,7 +250,36 @@
 
 def dump_resource_as_json(resource: dict) -> str:
     return str(run_safe(lambda: json.dumps(json_safe(resource))) or resource)
 
 
 def get_action_name_for_resource_change(res_change: str) -> str:
     return {"Add": "CREATE", "Remove": "DELETE", "Modify": "UPDATE"}.get(res_change)
+
+
+def check_not_found_exception(e, resource_type, resource, resource_status=None):
+    # we expect this to be a "not found" exception
+    markers = [
+        "NoSuchBucket",
+        "ResourceNotFound",
+        "NoSuchEntity",
+        "NotFoundException",
+        "404",
+        "not found",
+        "not exist",
+    ]
+
+    markers_hit = [m for m in markers if m in str(e)]
+    if not markers_hit:
+        LOG.warning(
+            "Unexpected error processing resource type %s: Exception: %s - %s - status: %s",
+            resource_type,
+            str(e),
+            resource,
+            resource_status,
+        )
+        if config.CFN_VERBOSE_ERRORS:
+            raise e
+        else:
+            return False
+
+    return True
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,16 +186,17 @@
         }
 
         if status_reason:
             event["ResourceStatusReason"] = status_reason
 
         self.events.insert(0, event)
 
-    def set_resource_status(self, resource_id: str, status: str, physical_res_id: str = None):
+    def set_resource_status(self, resource_id: str, status: str):
         """Update the deployment status of the given resource ID and publish a corresponding stack event."""
+        physical_res_id = self.resources.get(resource_id, {}).get("PhysicalResourceId")
         self._set_resource_status_details(resource_id, physical_res_id=physical_res_id)
         state = self.resource_states.setdefault(resource_id, {})
         state["PreviousResourceStatus"] = state.get("ResourceStatus")
         state["ResourceStatus"] = status
         state["LastUpdatedTimestamp"] = timestamp_millis()
         self.add_stack_event(resource_id, physical_res_id, status)
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 import base64
 import json
 import logging
 import re
 import traceback
 import uuid
-from typing import Any, Callable, Literal, Optional, Type, TypedDict
-
-import botocore
+from typing import Literal, Optional, Type, TypedDict
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
 from localstack.aws.connect import connect_to
-from localstack.services.cloudformation import usage
 from localstack.services.cloudformation.deployment_utils import (
     PLACEHOLDER_AWS_NO_VALUE,
-    dump_resource_as_json,
-    fix_boto_parameters_based_on_report,
     get_action_name_for_resource_change,
-    log_not_available_message,
     remove_none_values,
 )
 from localstack.services.cloudformation.engine.entities import Stack, StackChangeSet
 from localstack.services.cloudformation.engine.parameters import StackParameter
 from localstack.services.cloudformation.engine.template_utils import (
     fn_equals_type_conversion,
     get_deps_for_resource,
 )
-from localstack.services.cloudformation.engine.types import DeployTemplates, FuncDetails
 from localstack.services.cloudformation.resource_provider import (
+    PROVIDER_DEFAULTS,
     Credentials,
     ResourceProviderExecutor,
     ResourceProviderPayload,
-    check_not_found_exception,
     get_resource_type,
 )
 from localstack.services.cloudformation.service_models import (
     DependencyNotYetSatisfied,
     GenericBaseModel,
 )
 from localstack.services.cloudformation.stores import exports_map
 from localstack.utils.aws import aws_stack
 from localstack.utils.functions import prevent_stack_overflow
 from localstack.utils.json import clone_safe
 from localstack.utils.objects import get_all_subclasses
-from localstack.utils.strings import first_char_to_lower, to_bytes, to_str
+from localstack.utils.strings import to_bytes, to_str
 from localstack.utils.threads import start_worker_thread
 
 from localstack.services.cloudformation.models import *  # noqa: F401, isort:skip
 
 ACTION_CREATE = "create"
 ACTION_DELETE = "delete"
 AWS_URL_SUFFIX = "localhost.localstack.cloud"  # value is "amazonaws.com" in real AWS
@@ -75,157 +68,70 @@
 
 
 # ---------------------
 # CF TEMPLATE HANDLING
 # ---------------------
 
 
-def get_deployment_config(res_type: str) -> DeployTemplates | None:
-    resource_class = RESOURCE_MODELS.get(res_type)
-    if resource_class:
-        return resource_class.get_deploy_templates()
-    else:
-        usage.missing_resource_types.record(res_type)
-
-
-# TODO(ds): remove next
-def retrieve_resource_details(
-    resource_id, resource_status, resources: dict[str, Type[GenericBaseModel]], stack_name
-):
-    resource = resources.get(resource_id)
-    resource_id = resource_status.get("PhysicalResourceId") or resource_id
-    if not resource:
-        resource = {}
-    resource_type = get_resource_type(resource)
-    resource_props = resource.get("Properties")
-    if resource_props is None:
-        raise Exception(
-            f'Unable to find properties for resource "{resource_id}": {resource} - {resources}'
-        )
-    try:
-        # TODO(srw): assign resource objects rather than fetching state all the time
-        # convert resource props to resource entity
-        instance = get_resource_model_instance(resource_id, resources)
-        if instance:
-            state = instance.fetch_and_update_state(stack_name=stack_name, resources=resources)
-            return state
-
-        message = (
-            f"Unexpected resource type {resource_type} when resolving "
-            f"references of resource {resource_id}: {dump_resource_as_json(resource)}"
-        )
-        log_not_available_message(resource_type=resource_type, message=message)
-
-    except DependencyNotYetSatisfied:
-        if config.CFN_VERBOSE_ERRORS:
-            LOG.exception(f"dependency not yet satisfied for {resource_id}")
-        return
-
-    except Exception as e:
-        check_not_found_exception(e, resource_type, resource, resource_status)
-
-    return None
-
-
-# TODO(srw): this becomes a property lookup
-# TODO(ds): remove next
-def extract_resource_attribute(
-    resource_type,
-    resource_state,
-    attribute,
-    resource_id=None,
-    resource=None,
-    resources=None,
-    stack_name=None,
+def get_attr_from_model_instance(
+    resource: dict, attribute: str, resource_type: str, resource_id: Optional[str] = None
 ):
-    LOG.debug("Extract resource attribute: %s %s", resource_type, attribute)
-    is_ref_attribute = attribute in ["PhysicalResourceId", "Ref"]
-    resource = resource or {}
-    if not resource and resources:
-        resource = resources[resource_id]
-
-    if not resource_state:
-        resource_state = retrieve_resource_details(resource_id, {}, resources, stack_name)
-        if not resource_state:
-            raise DependencyNotYetSatisfied(
-                resource_ids=resource_id,
-                message=f'Unable to fetch details for resource "{resource_id}" (attribute "{attribute}")',
-            )
+    def _use_legacy():
+        # TODO: unify legacy detection with ResourceProvider
+        provider_config = json.loads(config.CFN_RESOURCE_PROVIDER_OVERRIDES)
+        # any config overwrites take precedence over the default list
+        PROVIDER_CONFIG = {**PROVIDER_DEFAULTS, **provider_config}
+        if resource_type in PROVIDER_CONFIG:
+            return PROVIDER_CONFIG[resource_type] == "GenericBaseModel"
 
-    if isinstance(resource_state, GenericBaseModel):
-        if hasattr(resource_state, "get_cfn_attribute"):
-            try:
-                return resource_state.get_cfn_attribute(attribute)
-            except Exception:
-                if config.CFN_VERBOSE_ERRORS:
-                    LOG.exception("could not fetch cfn attribute {attribute} from resource")
-        raise Exception(
-            f'Unable to extract attribute "{attribute}" from "{resource_type}" model class {type(resource_state)}'
-        )
-
-    # extract resource specific attributes
-    # TODO: remove the code below - move into resource model classes!
-
-    resource_props = resource.get("Properties", {})
-    attribute_lower = first_char_to_lower(attribute)
-    result = resource_state.get(attribute) or resource_state.get(attribute_lower)
-    if result is None and isinstance(resource, dict):
-        result = resource_props.get(attribute) or resource_props.get(attribute_lower)
-        if result is None:
-            result = get_attr_from_model_instance(
-                resource,
-                attribute,
-                resource_type=resource_type,
-                resource_id=resource_id,
-            )
-    if is_ref_attribute:
-        # TODO: remove
-        for attr in ["Id", "PhysicalResourceId", "Ref"]:
-            if result is None:
-                for obj in [resource_state, resource]:
-                    result = result or obj.get(attr)
-    return result
+        return True
 
+    if _use_legacy():
+        # TODO: open a PR with this branch removed to see where the legacy models are not behaving correctly
+        model_class = RESOURCE_MODELS.get(resource_type)
+        if not model_class:
+            LOG.debug('Unable to find model class for resource type "%s"', resource_type)
+            return
+        try:
+            inst = model_class(resource_name=resource_id, resource_json=resource)
 
-def get_attr_from_model_instance(
-    resource: dict, attribute: str, resource_type: str, resource_id: Optional[str] = None
-):
-    model_class = RESOURCE_MODELS.get(resource_type)
-    if not model_class:
-        LOG.debug('Unable to find model class for resource type "%s"', resource_type)
-    try:
-        inst = model_class(resource_name=resource_id, resource_json=resource)
-        return inst.get_cfn_attribute(attribute)
-    except Exception:
-        log_method = getattr(LOG, "debug")
-        if config.CFN_VERBOSE_ERRORS:
-            log_method = getattr(LOG, "exception")
-        log_method("Failed to retrieve model attribute: %s", attribute)
-
-
-def get_ref_from_model(resources: dict, logical_resource_id: str) -> Optional[str]:
-    resource = resources[logical_resource_id]
-    resource_type = get_resource_type(resource)
-    model_class = RESOURCE_MODELS.get(resource_type)
-    if model_class:
-        return model_class(resource_name=logical_resource_id, resource_json=resource).get_ref()
+            if hasattr(inst, "get_cfn_attribute"):
+                try:
+                    return inst.get_cfn_attribute(attribute)
+                except Exception:
+                    if config.CFN_VERBOSE_ERRORS:
+                        LOG.exception("could not fetch cfn attribute {attribute} from resource")
+            raise Exception(
+                f'Unable to extract attribute "{attribute}" from "{resource_type}" model class {type(inst)}'
+            )
+        except Exception:
+            log_method = getattr(LOG, "debug")
+            if config.CFN_VERBOSE_ERRORS:
+                log_method = getattr(LOG, "exception")
+            log_method("Failed to retrieve resource attribute: %s.%s", resource_id, attribute)
 
-    LOG.error("Unsupported resource type: %s", resource_type)
+    else:
+        # TODO: write code for property GetAtt lookup
+        return resource.get("Properties", {}).get(attribute)
 
 
 def resolve_ref(
     stack_name: str,
     resources: dict,
-    mappings: dict,
-    conditions: dict[str, bool],
     parameters: dict[str, StackParameter],
     ref: str,
-    attribute: str,
 ):
-    # pseudo parameters
+    """
+    ref always needs to be a static string
+    ref can be one of these:
+    1. a pseudo-parameter (e.g. AWS::Region)
+    2. a parameter
+    3. the id of a resource (PhysicalResourceId
+    """
+    # pseudo parameter
     if ref == "AWS::Region":
         return aws_stack.get_region()
     if ref == "AWS::Partition":
         return "aws"
     if ref == "AWS::StackName":
         return stack_name
     if ref == "AWS::StackId":
@@ -237,74 +143,30 @@
         return PLACEHOLDER_AWS_NO_VALUE
     if ref == "AWS::NotificationARNs":
         # TODO!
         return {}
     if ref == "AWS::URLSuffix":
         return AWS_URL_SUFFIX
 
-    if attribute == "Ref":
-        # ref always needs to be a static string
-        # ref can be one of these:
-        # 1. a parameter
-        # 2. a pseudo-parameter (e.g. AWS::Region)
-        # 3. the "value" of a resource
-
-        if parameter := parameters.get(ref):
-            parameter_type: str = parameter["ParameterType"]
-            parameter_value = parameter.get("ResolvedValue") or parameter.get("ParameterValue")
-
-            if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith("List<"):
-                return [p.strip() for p in parameter_value.split(",")]
-            else:
-                return parameter_value
-
-        resource = resources.get(ref)
-        if not resource:
-            raise Exception("Should be detected earlier.")
-
-        # TODO: this shouldn't be needed when dependency graph and deployment status is honored
-        resolve_refs_recursively(
-            stack_name, resources, mappings, conditions, parameters, resources.get(ref)
-        )
-        return get_ref_from_model(resources, ref)
-
-    if resources.get(ref):
-        if isinstance(resources[ref].get(attribute), (str, int, float, bool, dict)):
-            return resources[ref][attribute]
-
-    # TODO: when do we go into the branch below?
-    # TODO(ds): remove all below next
-    # fetch resource details
-    resource_new = retrieve_resource_details(ref, {}, resources, stack_name)
-    if not resource_new:
-        raise DependencyNotYetSatisfied(
-            resource_ids=ref,
-            message='Unable to fetch details for resource "%s" (resolving attribute "%s")'
-            % (ref, attribute),
-        )
+    # parameter
+    if parameter := parameters.get(ref):
+        parameter_type: str = parameter["ParameterType"]
+        parameter_value = parameter.get("ResolvedValue") or parameter.get("ParameterValue")
+
+        if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith("List<"):
+            return [p.strip() for p in parameter_value.split(",")]
+        else:
+            return parameter_value
 
+    # resource
     resource = resources.get(ref)
-    resource_type = get_resource_type(resource)
-    result = extract_resource_attribute(
-        resource_type,
-        resource_new,
-        attribute,
-        resource_id=ref,
-        resource=resource,
-        resources=resources,
-        stack_name=stack_name,
-    )
-    if result is None:
-        LOG.warning(
-            'Unable to extract reference attribute "%s" from resource: %s %s',
-            attribute,
-            resource_new,
-            resource,
-        )
-    return result
+    if not resource:
+        raise Exception("Should be detected earlier.")
+
+    return resources[ref].get("PhysicalResourceId")
 
 
 # Using a @prevent_stack_overflow decorator here to avoid infinite recursion
 # in case we load stack exports that have circular dependencies (see issue 3438)
 # TODO: Potentially think about a better approach in the future
 @prevent_stack_overflow(match_parameters=True)
 def resolve_refs_recursively(
@@ -401,23 +263,15 @@
 ):
     if isinstance(value, dict):
         keys_list = list(value.keys())
         stripped_fn_lower = keys_list[0].lower().split("::")[-1] if len(keys_list) == 1 else None
 
         # process special operators
         if keys_list == ["Ref"]:
-            ref = resolve_ref(
-                stack_name,
-                resources,
-                mappings,
-                conditions,
-                parameters,
-                value["Ref"],
-                attribute="Ref",
-            )
+            ref = resolve_ref(stack_name, resources, parameters, value["Ref"])
             if ref is None:
                 msg = 'Unable to resolve Ref for resource "%s" (yet)' % value["Ref"]
                 LOG.debug("%s - %s", msg, resources.get(value["Ref"]) or set(resources.keys()))
                 raise DependencyNotYetSatisfied(resource_ids=value["Ref"], message=msg)
             ref = resolve_refs_recursively(
                 stack_name, resources, mappings, conditions, parameters, ref
             )
@@ -487,23 +341,15 @@
 
         if stripped_fn_lower == "findinmap":
             # "Fn::FindInMap"
             mapping_id = value[keys_list[0]][0]
 
             if isinstance(mapping_id, dict) and "Ref" in mapping_id:
                 # TODO: ??
-                mapping_id = resolve_ref(
-                    stack_name,
-                    resources,
-                    mappings,
-                    conditions,
-                    parameters,
-                    mapping_id["Ref"],
-                    "Ref",
-                )
+                mapping_id = resolve_ref(stack_name, resources, parameters, mapping_id["Ref"])
 
             selected_map = mappings.get(mapping_id)
             if not selected_map:
                 raise Exception(
                     f"Cannot find Mapping with ID {mapping_id} for Fn::FindInMap: {value[keys_list[0]]} {list(resources.keys())}"  # TODO: verify
                 )
 
@@ -686,17 +532,15 @@
                 )
             if not isinstance(resolved, str):
                 resolved = str(resolved)
             return resolved
         if len(parts) == 1:
             if parts[0] in resources:
                 # Logical resource ID or parameter name specified => Use Ref for lookup
-                result = resolve_ref(
-                    stack_name, resources, mappings, conditions, parameters, parts[0], "Ref"
-                )
+                result = resolve_ref(stack_name, resources, parameters, parts[0])
 
                 if result is None:
                     raise DependencyNotYetSatisfied(
                         resource_ids=parts[0],
                         message=f"Unable to resolve attribute ref {ref_expression}",
                     )
                 # TODO: is this valid?
@@ -726,109 +570,20 @@
         return match.group(0)
 
     regex = r"\$\{([^\}]+)\}"
     result = re.sub(regex, _replace, result)
     return result
 
 
-def evaluate_resource_condition(
-    stack_name: str, resources: dict, mappings: dict, conditions: dict[str, bool], resource: dict
-) -> bool:
-    condition = resource.get("Condition")
-    if condition:
+def evaluate_resource_condition(conditions: dict[str, bool], resource: dict) -> bool:
+    if condition := resource.get("Condition"):
         return conditions.get(condition, True)
     return True
 
 
-# TODO: move (registry/util)
-def get_resource_model_instance(resource_id: str, resources) -> Optional[GenericBaseModel]:
-    """Obtain a typed resource entity instance representing the given stack resource."""
-    resource = resources[resource_id]
-    resource_type = get_resource_type(resource)
-    resource_class = RESOURCE_MODELS.get(resource_type)
-    if not resource_class:
-        return None
-    instance = resource_class(resource)
-    return instance
-
-
-def invoke_function(
-    function: Callable,
-    params: dict,
-    resource_type: str,
-    func_details: FuncDetails,
-    action_name: str,
-    resource: Any,
-) -> Any:
-    try:
-        LOG.debug(
-            'Request for resource type "%s" in region %s: %s %s',
-            resource_type,
-            aws_stack.get_region(),
-            func_details["function"],
-            params,
-        )
-        try:
-            result = function(**params)
-        except botocore.exceptions.ParamValidationError as e:
-            # alternatively we could also use the ParamValidator directly
-            report = e.kwargs.get("report")
-            if not report:
-                raise
-
-            LOG.debug("Converting parameters to allowed types")
-            converted_params = fix_boto_parameters_based_on_report(params, report)
-            LOG.debug("Original parameters:  %s", params)
-            LOG.debug("Converted parameters: %s", converted_params)
-
-            result = function(**converted_params)
-    except Exception as e:
-        if action_name == "delete" and check_not_found_exception(e, resource_type, resource):
-            return
-        log_method = getattr(LOG, "warning")
-        if config.CFN_VERBOSE_ERRORS:
-            log_method = getattr(LOG, "exception")
-        log_method("Error calling %s with params: %s for resource: %s", function, params, resource)
-        raise e
-
-    return result
-
-
-# TODO: this shouldn't be called for stack parameters
-# TODO: refactor / remove (should just be a lookup on the resource state)
-def determine_resource_physical_id(
-    resource_id: str, resources: dict, stack_name: str
-) -> Optional[str]:
-    assert resource_id and isinstance(resource_id, str)
-
-    resource = resources.get(resource_id)
-    if not resource:
-        return
-    resource_type = get_resource_type(resource)
-
-    # determine result from resource class
-    resource_class = RESOURCE_MODELS.get(resource_type)
-    if resource_class:
-        resource_inst = resource_class(resource)
-        resource_inst.fetch_state_if_missing(stack_name=stack_name, resources=resources)
-        result = resource_inst.physical_resource_id
-        if result:
-            return result
-
-    # TODO: should be able to remove this as well and unify with the one above
-    res_id = resource.get("PhysicalResourceId")
-    if res_id:
-        return res_id
-    LOG.info(
-        'Unable to determine PhysicalResourceId for "%s" resource, ID "%s"',
-        resource_type,
-        resource_id,
-    )
-
-
 # -----------------------
 # MAIN TEMPLATE DEPLOYER
 # -----------------------
 
 
 Action = str
 
@@ -844,15 +599,14 @@
 
 
 class ChangeConfig(TypedDict):
     Type: str
     ResourceChange: ResourceChange
 
 
-# TODO: replace
 class TemplateDeployer:
     def __init__(self, stack):
         self.stack = stack
 
         try:
             self.provider_config = json.loads(config.CFN_RESOURCE_PROVIDER_OVERRIDES)
         except json.JSONDecodeError:
@@ -961,17 +715,14 @@
             }
             if len(resources) == 0:
                 break
             for resource_id, resource in resources.items():
                 try:
                     # TODO: cache condition value in resource details on deployment and use cached value here
                     if evaluate_resource_condition(
-                        self.stack_name,
-                        self.resources,
-                        self.mappings,
                         self.stack.resolved_conditions,
                         resource,
                     ):
                         executor = self.create_resource_provider_executor()
                         resource_provider_payload = self.create_resource_provider_payload(
                             "Remove", logical_resource_id=resource_id
                         )
@@ -998,39 +749,18 @@
         self.stack.set_stack_status("DELETE_COMPLETE")
         self.stack.set_time_attribute("DeletionTime")
 
     # ----------------------------
     # DEPENDENCY RESOLUTION UTILS
     # ----------------------------
 
-    def is_deployable_resource(self, resource):
-        resource_type = get_resource_type(resource)
-        entry = get_deployment_config(resource_type)
-        if entry is None:
-            resource_str = dump_resource_as_json(resource)
-            LOG.warning(f'Unable to deploy resource type "{resource_type}": {resource_str}')
-        return bool(entry and entry.get(ACTION_CREATE))
-
     def is_deployed(self, resource):
-        # TODO: make this a check on the actual resource status instead(!)
-        resource_status = {}
-        resource_id = resource["LogicalResourceId"]
-        details = retrieve_resource_details(
-            resource_id, resource_status, self.stack.resources, self.stack.stack_name
-        )
-        return bool(details)
-
-    def is_updateable(self, resource):
-        """Return whether the given resource can be updated or not."""
-        if not self.is_deployable_resource(resource) or not self.is_deployed(resource):
-            return False
-        resource_instance = get_resource_model_instance(
-            resource["LogicalResourceId"], self.stack.resources
-        )
-        return resource_instance.is_updatable()
+        return self.stack.resource_states.get(resource["LogicalResourceId"], {}).get(
+            "ResourceStatus"
+        ) in ["CREATE_COMPLETE", "UPDATE_COMPLETE"]
 
     def all_resource_dependencies_satisfied(self, resource) -> bool:
         unsatisfied = self.get_unsatisfied_dependencies(resource)
         return not unsatisfied
 
     def get_unsatisfied_dependencies(self, resource):
         res_deps = self.get_resource_dependencies(
@@ -1042,25 +772,24 @@
         return self.get_unsatisfied_dependencies_for_resources(res_deps_mapped, resource)
 
     def get_unsatisfied_dependencies_for_resources(
         self, resources, depending_resource=None, return_first=True
     ):
         result = {}
         for resource_id, resource in resources.items():
-            if self.is_deployable_resource(resource):
-                if not self.is_deployed(resource):
-                    LOG.debug(
-                        "Dependency for resource %s not yet deployed: %s %s",
-                        depending_resource,
-                        resource_id,
-                        resource,
-                    )
-                    result[resource_id] = resource
-                    if return_first:
-                        break
+            if not self.is_deployed(resource):
+                LOG.debug(
+                    "Dependency for resource %s not yet deployed: %s %s",
+                    depending_resource,
+                    resource_id,
+                    resource,
+                )
+                result[resource_id] = resource
+                if return_first:
+                    break
         return result
 
     def get_resource_dependencies(self, resource: dict) -> set[str]:
         """
         Takes a resource and returns its dependencies on other resources via a str -> str mapping
         """
         # Note: using the original, unmodified template here to preserve Ref's ...
@@ -1074,46 +803,14 @@
 
     def init_resource_status(self, resources=None, stack=None, action="CREATE"):
         resources = resources or self.resources
         stack = stack or self.stack
         for resource_id, resource in resources.items():
             stack.set_resource_status(resource_id, f"{action}_IN_PROGRESS")
 
-    # Stack is needed here
-    def update_resource_details(self, resource_id, stack=None, action="CREATE"):
-        stack = stack or self.stack
-        # update physical resource id
-        resource = stack.resources[resource_id]
-
-        physical_id = resource.get("PhysicalResourceId")
-
-        physical_id = physical_id or determine_resource_physical_id(
-            resource_id, resources=stack.resources, stack_name=stack.stack_name
-        )
-        if not resource.get("PhysicalResourceId") or action == "UPDATE":
-            if physical_id:
-                resource["PhysicalResourceId"] = physical_id
-
-        # Fetch state for compatibility purposes
-        # Since we now have the PhysicalResourceId available without a fetch_state, other attributes that still depend on fetch-state state might not work otherwise
-        if not resource:
-            return
-        resource_type = get_resource_type(resource)
-        resource_class = RESOURCE_MODELS.get(resource_type)
-        if resource_class:
-            resource_inst = resource_class(resource)
-            resource_inst.fetch_state_if_missing(
-                stack_name=stack.stack_name, resources=stack.resources
-            )
-
-        # set resource status
-        stack.set_resource_status(resource_id, f"{action}_COMPLETE", physical_res_id=physical_id)
-
-        return physical_id
-
     def get_change_config(
         self, action: str, resource: dict, change_set_id: Optional[str] = None
     ) -> ChangeConfig:
         result = ChangeConfig(
             **{
                 "Type": "Resource",
                 "ResourceChange": ResourceChange(
@@ -1390,17 +1087,15 @@
         """
         resource = new_resources[resource_id]
         res_change = change["ResourceChange"]
         action = res_change["Action"]
 
         # TODO: this needs to happen much earlier
         # check resource condition, if present
-        if not evaluate_resource_condition(
-            stack.stack_name, stack.resources, stack.mappings, stack.resolved_conditions, resource
-        ):
+        if not evaluate_resource_condition(stack.resolved_conditions, resource):
             LOG.debug(
                 'Skipping deployment of "%s", as resource condition evaluates to false', resource_id
             )
             return
 
         # resolve refs in resource details
         resolve_refs_recursively(
@@ -1409,73 +1104,58 @@
             stack.mappings,
             stack.resolved_conditions,
             stack.resolved_parameters,
             resource,
         )
 
         if action in ["Add", "Modify"]:
-            if action == "Add" and not self.is_deployable_resource(resource):
-                return False
             is_deployed = self.is_deployed(resource)
             # TODO: Attaching the cached _deployed info here, as we should not change the "Add"/"Modify" attribute
             #  here, which is used further down the line to determine the resource action CREATE/UPDATE. This is a
             #  temporary workaround for now - to be refactored once we introduce proper stack resource state models.
             res_change["_deployed"] = is_deployed
             if not is_deployed:
                 return True
             if action == "Add":
                 return False
-            if action == "Modify" and not self.is_updateable(resource):
-                LOG.debug(
-                    'Action "update" not yet implemented for CF resource type %s',
-                    resource.get("Type"),
-                )
-                return False
         elif action == "Remove":
-            should_remove = self.is_deployable_resource(resource)
-            if not should_remove:
-                LOG.debug(
-                    f"Action 'remove' not yet implemented for CF resource type {resource.get('Type')}"
-                )
-            return should_remove
+            return True
         return True
 
     # Stack is needed here
     def apply_change(self, change: ChangeConfig, stack: Stack):
         change_details = change["ResourceChange"]
         action = change_details["Action"]
         resource_id = change_details["LogicalResourceId"]
         resources = stack.resources
         resource = resources[resource_id]
 
         # TODO: this should not be needed as resources are filtered out if the
         # condition evaluates to False.
-        if not evaluate_resource_condition(
-            stack.stack_name, resources, stack.mappings, stack.resolved_conditions, resource
-        ):
+        if not evaluate_resource_condition(stack.resolved_conditions, resource):
             return
 
         # remove AWS::NoValue entries
         resource_props = resource.get("Properties")
         if resource_props:
             resource["Properties"] = remove_none_values(resource_props)
 
         executor = self.create_resource_provider_executor()
         resource_provider_payload = self.create_resource_provider_payload(
             action, logical_resource_id=resource_id
         )
 
         # TODO: verify event
-        executor.deploy_loop(resource_provider_payload)  # noqa
+        progress_event = executor.deploy_loop(resource_provider_payload)  # noqa
 
         # TODO: update resource state with returned state from progress event
 
         # update resource status and physical resource id
         stack_action = get_action_name_for_resource_change(action)
-        self.update_resource_details(resource_id, stack=stack, action=stack_action)
+        stack.set_resource_status(resource_id, f"{stack_action}_COMPLETE")
 
     def create_resource_provider_executor(self) -> ResourceProviderExecutor:
         return ResourceProviderExecutor(
             stack_name=self.stack.stack_name,
             stack_id=self.stack.stack_id,
             provider_config=self.provider_config,
             # FIXME: ugly
@@ -1488,29 +1168,30 @@
     ) -> ResourceProviderPayload:
         creds: Credentials = {
             "accessKeyId": "test",
             "secretAccessKey": "test",
             "sessionToken": "",
         }
         resource = self.resources[logical_resource_id]
+
         resource_provider_payload: ResourceProviderPayload = {
             "awsAccountId": "000000000000",
             "callbackContext": {},
             "stackId": self.stack.stack_name,
             "resourceType": resource["Type"],
             "resourceTypeVersion": "000000",
             # TODO: not actually a UUID
             "bearerToken": str(uuid.uuid4()),
             # TODO: get the current region
             "region": "us-east-1",
             "action": action,
             "requestData": {
                 "logicalResourceId": logical_resource_id,
                 "resourceProperties": resource["Properties"],
-                "previousResourceProperties": None,
+                "previousResourceProperties": None,  # TODO
                 "callerCredentials": creds,
                 "providerCredentials": creds,
                 "systemTags": {},
                 "previousSystemTags": {},
                 "stackTags": {},
                 "previousStackTags": {},
             },
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/events.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         user_name = self.props.get("UserName")
         access_key_id = self.physical_resource_id
         if access_key_id:
             keys = connect_to().iam.list_access_keys(UserName=user_name)["AccessKeyMetadata"]
             return [key for key in keys if key["AccessKeyId"] == access_key_id][0]
 
     def update_resource(self, new_resource, stack_name, resources):
+        # TODO: Fix this behavior by migrating to a new resource provider
         access_key_id = self.physical_resource_id
         new_props = new_resource["Properties"]
         user_name = new_props.get("UserName")
         status = new_props.get("Status")
 
         connect_to().iam.update_access_key(
             UserName=user_name, AccessKeyId=access_key_id, Status=status
@@ -229,15 +230,14 @@
     def fetch_state(self, stack_name, resources):
         role_name = self.props.get("RoleName")
         client = connect_to().iam
         return client.get_role(RoleName=role_name)["Role"]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
-        # _states contains the old state of the resource
         _states = new_resource.get("_state_", None)
         client = connect_to().iam
         if _states:
             props_policy = props.get("AssumeRolePolicyDocument")
             name_changed = props.get("RoleName") != _states.get("RoleName")
             policy_changed = props_policy and props_policy != _states.get(
                 "AssumeRolePolicyDocument", ""
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/sqs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,141 @@
 import json
+import logging
+
+from botocore.exceptions import ClientError
 
 from localstack.aws.connect import connect_to
+from localstack.services.cloudformation.deployment_utils import (
+    generate_default_name,
+    params_list_to_dict,
+    params_select_attributes,
+)
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils.aws import arns
+from localstack.utils.common import short_uid
 
+LOG = logging.getLogger(__name__)
 
-class KMSKey(GenericBaseModel):
-    @staticmethod
-    def cloudformation_type():
-        return "AWS::KMS::Key"
 
-    def get_cfn_attribute(self, attribute_name):
-        if attribute_name == "Arn":
-            return arns.kms_key_arn(self.physical_resource_id)
-        return super(KMSKey, self).get_cfn_attribute(attribute_name)
+class QueuePolicy(GenericBaseModel):
+    @classmethod
+    def cloudformation_type(cls):
+        return "AWS::SQS::QueuePolicy"
 
     def fetch_state(self, stack_name, resources):
-        client = connect_to().kms
-        physical_res_id = self.physical_resource_id
-        props = self.props
-        res_tags = props.get("Tags", [])
-        if not physical_res_id:
-            # TODO: find a more efficient approach for this?
-            for key in client.list_keys()["Keys"]:
-                details = client.describe_key(KeyId=key["KeyId"])["KeyMetadata"]
-                tags = client.list_resource_tags(KeyId=key["KeyId"]).get("Tags", [])
-                tags = [{"Key": tag["TagKey"], "Value": tag["TagValue"]} for tag in tags]
-                if (
-                    tags == res_tags
-                    and details.get("Description") == props.get("Description")
-                    and props.get("KeyUsage") in [None, details.get("KeyUsage")]
-                ):
-                    physical_res_id = key["KeyId"]
-                    # TODO should this be removed from here? It seems that somewhere along the execution
-                    #  chain the 'PhysicalResourceId' gets overwritten with None, hence setting it here
-                    self.resource_json["PhysicalResourceId"] = physical_res_id
-                    break
-        if not physical_res_id:
-            return
-        return client.describe_key(KeyId=physical_res_id)
+        if self.resource_json.get("PhysicalResourceId"):
+            return {"something": "something"}  # gotta return <something> since {} is falsey :)
 
     @classmethod
     def get_deploy_templates(cls):
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            kms_client = connect_to().kms
+            sqs_client = connect_to().sqs
             resource_provider = cls(resource)
             props = resource_provider.props
-            params = {}
-            if props.get("KeyPolicy"):
-                params["Policy"] = json.dumps(props["KeyPolicy"])
-
-            if props.get("Tags"):
-                params["Tags"] = [
-                    {"TagKey": tag["Key"], "TagValue": tag["Value"]}
-                    for tag in props.get("Tags", [])
-                ]
-
-            for key in ["Description", "KeySpec", "KeyUsage"]:
-                if props.get(key):
-                    params[key] = props[key]
-
-            new_key = kms_client.create_key(**params)
-            key_id = new_key["KeyMetadata"]["KeyId"]
-
-            # key is created but some fields map to separate api calls
-            if props.get("EnableKeyRotation", False):
-                kms_client.enable_key_rotation(KeyId=key_id)
-            else:
-                kms_client.disable_key_rotation(KeyId=key_id)
-
-            if props.get("Enabled", True):
-                kms_client.enable_key(KeyId=key_id)
-            else:
-                kms_client.disable_key(KeyId=key_id)
 
-            return new_key
+            resource["PhysicalResourceId"] = "%s-%s-%s" % (
+                stack_name,
+                logical_resource_id,
+                short_uid(),
+            )
+
+            policy = json.dumps(props["PolicyDocument"])
+            for queue in props["Queues"]:
+                sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": policy})
 
-        def _handle_key_result(result, resource_id, resources, resource_type):
-            resources[resource_id]["PhysicalResourceId"] = result["KeyMetadata"]["KeyId"]
+        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
+            sqs_client = connect_to().sqs
+            resource_provider = cls(resource)
+            props = resource_provider.props
+
+            for queue in props["Queues"]:
+                try:
+                    sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": ""})
+                except ClientError as err:
+                    if "AWS.SimpleQueueService.NonExistentQueue" != err.response["Error"]["Code"]:
+                        raise
 
         return {
-            "create": [
-                {"function": _create, "result_handler": _handle_key_result},
-            ],
+            "create": {"function": _create},
             "delete": {
-                # TODO Key needs to be deleted in KMS backend
-                "function": "schedule_key_deletion",
-                "parameters": {"KeyId": "PhysicalResourceId"},
+                "function": _delete,
             },
         }
 
 
-class KMSAlias(GenericBaseModel):
-    @staticmethod
-    def cloudformation_type():
-        return "AWS::KMS::Alias"
+class SQSQueue(GenericBaseModel):
+    @classmethod
+    def cloudformation_type(cls):
+        return "AWS::SQS::Queue"
+
+    def get_cfn_attribute(self, attribute_name):
+        if attribute_name == "Arn":
+            return arns.sqs_queue_arn(self.properties["QueueName"])
+        return super().get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
-        aliases = connect_to().kms.list_aliases()["Aliases"]
-        for alias in aliases:
-            if alias["AliasName"] == self.props.get("AliasName"):
-                return alias
-        return None
+        queue_name = self.props["QueueName"]
+        sqs_client = connect_to().sqs
+        queues = sqs_client.list_queues()
+        result = list(
+            filter(
+                lambda item:
+                # TODO possibly find a better way to compare resource_id with queue URLs
+                item.endswith("/%s" % queue_name),
+                queues.get("QueueUrls", []),
+            )
+        )
+        if not result:
+            return None
+        result = sqs_client.get_queue_attributes(QueueUrl=result[0], AttributeNames=["All"])[
+            "Attributes"
+        ]
+        result["Arn"] = result["QueueArn"]
+        return result
 
     @staticmethod
-    def get_deploy_templates():
+    def add_defaults(resource, stack_name: str):
+        role_name = resource.get("Properties", {}).get("QueueName")
+
+        if not role_name:
+            resource["Properties"]["QueueName"] = generate_default_name(
+                stack_name, resource["LogicalResourceId"]
+            )
+            if resource["Properties"].get("FifoQueue"):
+                resource["Properties"]["QueueName"] += ".fifo"
+
+    @classmethod
+    def get_deploy_templates(cls):
+        def _queue_url(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
+            provider = cls(resource)
+            queue_url = provider.physical_resource_id or properties.get("QueueUrl")
+            if queue_url:
+                return queue_url
+            return arns.sqs_queue_url_for_arn(properties["QueueArn"])
+
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
-            resource["PhysicalResourceId"] = resource["Properties"]["AliasName"]
+            resource["PhysicalResourceId"] = result["QueueUrl"]
 
         return {
             "create": {
-                "function": "create_alias",
-                "parameters": {"AliasName": "AliasName", "TargetKeyId": "TargetKeyId"},
+                "function": "create_queue",
+                "parameters": {
+                    "QueueName": "QueueName",
+                    "Attributes": params_select_attributes(
+                        "ContentBasedDeduplication",
+                        "DelaySeconds",
+                        "FifoQueue",
+                        "MaximumMessageSize",
+                        "MessageRetentionPeriod",
+                        "VisibilityTimeout",
+                        "RedrivePolicy",
+                        "ReceiveMessageWaitTimeSeconds",
+                    ),
+                    "tags": params_list_to_dict("Tags"),
+                },
                 "result_handler": _handle_result,
             },
             "delete": {
-                "function": "delete_alias",
-                "parameters": {"AliasName": "AliasName"},
+                "function": "delete_queue",
+                "parameters": {"QueueUrl": _queue_url},
             },
         }
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,144 @@
-import json
 import logging
-
-from botocore.exceptions import ClientError
+import re
+from typing import Dict
 
 from localstack.aws.connect import connect_to
-from localstack.services.cloudformation.deployment_utils import (
-    generate_default_name,
-    params_list_to_dict,
-    params_select_attributes,
-)
+from localstack.services.cloudformation.deployment_utils import generate_default_name
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns
-from localstack.utils.common import short_uid
+from localstack.utils.common import to_str
 
 LOG = logging.getLogger(__name__)
 
 
-class QueuePolicy(GenericBaseModel):
-    @classmethod
-    def cloudformation_type(cls):
-        return "AWS::SQS::QueuePolicy"
+class SFNActivity(GenericBaseModel):
+    @staticmethod
+    def cloudformation_type():
+        return "AWS::StepFunctions::Activity"
 
     def fetch_state(self, stack_name, resources):
-        if self.resource_json.get("PhysicalResourceId"):
-            return {"something": "something"}  # gotta return <something> since {} is falsey :)
-
-    @classmethod
-    def get_deploy_templates(cls):
-        def _create(logical_resource_id: str, resource: dict, stack_name: str):
-            sqs_client = connect_to().sqs
-            resource_provider = cls(resource)
-            props = resource_provider.props
-
-            resource["PhysicalResourceId"] = "%s-%s-%s" % (
-                stack_name,
-                logical_resource_id,
-                short_uid(),
-            )
+        activity_arn = self.physical_resource_id
+        if not activity_arn:
+            return None
+        client = connect_to().stepfunctions
+        result = client.describe_activity(activityArn=activity_arn)
+        return result
 
-            policy = json.dumps(props["PolicyDocument"])
-            for queue in props["Queues"]:
-                sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": policy})
-
-        def _delete(logical_resource_id: str, resource: dict, stack_name: str):
-            sqs_client = connect_to().sqs
-            resource_provider = cls(resource)
-            props = resource_provider.props
-
-            for queue in props["Queues"]:
-                try:
-                    sqs_client.set_queue_attributes(QueueUrl=queue, Attributes={"Policy": ""})
-                except ClientError as err:
-                    if "AWS.SimpleQueueService.NonExistentQueue" != err.response["Error"]["Code"]:
-                        raise
+    @staticmethod
+    def get_deploy_templates():
+        def _handle_result(result: dict, logical_resource_id: str, resource: dict):
+            resource["Properties"]["Arn"] = result["activityArn"]
+            resource["PhysicalResourceId"] = result["activityArn"]
 
         return {
-            "create": {"function": _create},
+            "create": {
+                "function": "create_activity",
+                "parameters": {"name": "Name", "tags": "Tags"},
+                "result_handler": _handle_result,
+            },
             "delete": {
-                "function": _delete,
+                "function": "delete_activity",
+                "parameters": {"activityArn": "PhysicalResourceId"},
             },
         }
 
 
-class SQSQueue(GenericBaseModel):
-    @classmethod
-    def cloudformation_type(cls):
-        return "AWS::SQS::Queue"
+class SFNStateMachine(GenericBaseModel):
+    @staticmethod
+    def cloudformation_type():
+        return "AWS::StepFunctions::StateMachine"
 
-    def get_cfn_attribute(self, attribute_name):
+    def get_cfn_attribute(self, attribute_name: str):
         if attribute_name == "Arn":
-            return arns.sqs_queue_arn(self.properties["QueueName"])
-        return super().get_cfn_attribute(attribute_name)
+            return self.props.get("Arn")
+        if attribute_name == "Name":
+            return self.props.get("StateMachineName")
+        return super(SFNStateMachine, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
-        queue_name = self.props["QueueName"]
-        sqs_client = connect_to().sqs
-        queues = sqs_client.list_queues()
-        result = list(
-            filter(
-                lambda item:
-                # TODO possibly find a better way to compare resource_id with queue URLs
-                item.endswith("/%s" % queue_name),
-                queues.get("QueueUrls", []),
-            )
-        )
-        if not result:
+        sm_name = self.props.get("StateMachineName") or self.logical_resource_id
+        sfn_client = connect_to().stepfunctions
+        state_machines = sfn_client.list_state_machines()["stateMachines"]
+        sm_arn = [m["stateMachineArn"] for m in state_machines if m["name"] == sm_name]
+        if not sm_arn:
             return None
-        result = sqs_client.get_queue_attributes(QueueUrl=result[0], AttributeNames=["All"])[
-            "Attributes"
-        ]
-        result["Arn"] = result["QueueArn"]
+        result = sfn_client.describe_state_machine(stateMachineArn=sm_arn[0])
         return result
 
+    def update_resource(self, new_resource, stack_name, resources):
+        props = new_resource["Properties"]
+        client = connect_to().stepfunctions
+        sm_arn = self.props.get("stateMachineArn")
+        if not sm_arn:
+            self.state = self.fetch_state(stack_name=stack_name, resources=resources)
+            sm_arn = self.state["stateMachineArn"]
+        kwargs = {
+            "stateMachineArn": sm_arn,
+            "definition": props["DefinitionString"],
+        }
+        return client.update_state_machine(**kwargs)
+
     @staticmethod
     def add_defaults(resource, stack_name: str):
-        role_name = resource.get("Properties", {}).get("QueueName")
-
+        role_name = resource.get("Properties", {}).get("StateMachineName")
         if not role_name:
-            resource["Properties"]["QueueName"] = generate_default_name(
+            resource["Properties"]["StateMachineName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
-            if resource["Properties"].get("FifoQueue"):
-                resource["Properties"]["QueueName"] += ".fifo"
 
     @classmethod
     def get_deploy_templates(cls):
-        def _queue_url(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
-            provider = cls(resource)
-            queue_url = provider.physical_resource_id or properties.get("QueueUrl")
-            if queue_url:
-                return queue_url
-            return arns.sqs_queue_url_for_arn(properties["QueueArn"])
-
         def _handle_result(result: dict, logical_resource_id: str, resource: dict):
-            resource["PhysicalResourceId"] = result["QueueUrl"]
+            resource["Properties"]["Arn"] = result["stateMachineArn"]
+            resource["PhysicalResourceId"] = result["stateMachineArn"]
+
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            def _get_definition(properties):
+                # TODO: support "Definition" parameter
+                definition_str = properties.get("DefinitionString")
+                s3_location = properties.get("DefinitionS3Location")
+                if not definition_str and s3_location:
+                    # TODO: currently not covered by tests - add a test to mimick the behavior of "sam deploy ..."
+                    s3_client = connect_to().s3
+                    LOG.debug("Fetching state machine definition from S3: %s", s3_location)
+                    result = s3_client.get_object(
+                        Bucket=s3_location["Bucket"], Key=s3_location["Key"]
+                    )
+                    definition_str = to_str(result["Body"].read())
+                substitutions = properties.get("DefinitionSubstitutions")
+                if substitutions is not None:
+                    definition_str = _apply_substitutions(definition_str, substitutions)
+                return definition_str
+
+            return {
+                "name": properties.get("StateMachineName"),
+                "definition": _get_definition(properties),
+                "roleArn": properties.get("RoleArn"),
+                "type": properties.get("StateMachineType", None),
+            }
 
         return {
             "create": {
-                "function": "create_queue",
-                "parameters": {
-                    "QueueName": "QueueName",
-                    "Attributes": params_select_attributes(
-                        "ContentBasedDeduplication",
-                        "DelaySeconds",
-                        "FifoQueue",
-                        "MaximumMessageSize",
-                        "MessageRetentionPeriod",
-                        "VisibilityTimeout",
-                        "RedrivePolicy",
-                        "ReceiveMessageWaitTimeSeconds",
-                    ),
-                    "tags": params_list_to_dict("Tags"),
-                },
+                "function": "create_state_machine",
+                "parameters": _create_params,
                 "result_handler": _handle_result,
             },
             "delete": {
-                "function": "delete_queue",
-                "parameters": {"QueueUrl": _queue_url},
+                "function": "delete_state_machine",
+                "parameters": {"stateMachineArn": "PhysicalResourceId"},
             },
         }
+
+
+def _apply_substitutions(definition: str, substitutions: Dict[str, str]) -> str:
+    substitution_regex = re.compile("\\${[a-zA-Z0-9_]+}")  # might be a bit too strict in some cases
+    tokens = substitution_regex.findall(definition)
+    result = definition
+    for token in tokens:
+        raw_token = token[2:-1]  # strip ${ and }
+        if raw_token not in substitutions.keys():
+            raise
+        result = result.replace(token, substitutions[raw_token])
+
+    return result
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/resource_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 from botocore.exceptions import UnknownServiceError
 from plugin import Plugin, PluginManager
 
 from localstack import config
 from localstack.aws.connect import ServiceLevelClientFactory, connect_to
 from localstack.services.cloudformation import usage
 from localstack.services.cloudformation.deployment_utils import (
+    check_not_found_exception,
     convert_data_types,
     fix_account_id_in_arns,
     fix_boto_parameters_based_on_report,
+    log_not_available_message,
     remove_none_values,
 )
 from localstack.services.cloudformation.engine.quirks import PHYSICAL_RESOURCE_ID_SPECIAL_CASES
 from localstack.services.cloudformation.service_models import KEY_RESOURCE_STATE, GenericBaseModel
 from localstack.utils.aws import aws_stack
 
 if TYPE_CHECKING:
@@ -39,15 +41,15 @@
 Properties = TypeVar("Properties")
 
 PUBLIC_REGISTRY: dict[str, Type[ResourceProvider]] = {}
 
 # by default we use the GenericBaseModel (the legacy model), unless the resource is listed below
 # add your new provider here when you want it to be the default
 PROVIDER_DEFAULTS = {
-    # "AWS::IAM::User": "GenericBaseModel",
+    # "AWS::IAM::User": "ResourceProvider",
     # "AWS::SSM::Parameter": "GenericBaseModel",
     # "AWS::OpenSearchService::Domain": "GenericBaseModel",
 }
 
 
 class OperationStatus(Enum):
     PENDING = auto()
@@ -181,45 +183,20 @@
         raise ValueError(f"Invalid argument: {resource}")
     try:
         resource_type: str = resource["Type"]
 
         if resource_type.startswith("Custom::"):
             return "AWS::CloudFormation::CustomResource"
         return resource_type
-    except Exception as e:
-        print(e)
-
-
-def check_not_found_exception(e, resource_type, resource, resource_status=None):
-    # we expect this to be a "not found" exception
-    markers = [
-        "NoSuchBucket",
-        "ResourceNotFound",
-        "NoSuchEntity",
-        "NotFoundException",
-        "404",
-        "not found",
-        "not exist",
-    ]
-
-    markers_hit = [m for m in markers if m in str(e)]
-    if not markers_hit:
+    except Exception:
         LOG.warning(
-            "Unexpected error processing resource type %s: Exception: %s - %s - status: %s",
-            resource_type,
-            str(e),
-            resource,
-            resource_status,
+            "Failed to retrieve resource type %s",
+            resource.get("Type"),
+            exc_info=LOG.isEnabledFor(logging.DEBUG),
         )
-        if config.CFN_VERBOSE_ERRORS:
-            raise e
-        else:
-            return False
-
-    return True
 
 
 def invoke_function(
     function: Callable,
     params: dict,
     resource_type: str,
     func_details: FuncDetails,
@@ -396,14 +373,15 @@
     def update(self, request: ResourceRequest[Properties]) -> ProgressEvent[Properties]:
         physical_resource_id = self.all_resources[request.logical_resource_id]["PhysicalResourceId"]
         resource_provider = self.resource_provider_cls(
             # TODO: other top level keys
             resource_json={
                 "Type": self.resource_type,
                 "Properties": request.desired_state,
+                "_state_": request.previous_state,
                 "PhysicalResourceId": physical_resource_id,
                 "LogicalResourceId": request.logical_resource_id,
             },
             region_name=request.region_name,
         )
         if not resource_provider.is_updatable():
             LOG.warning(
@@ -420,41 +398,58 @@
         LOG.info("Updating resource %s of type %s", request.logical_resource_id, self.resource_type)
 
         resource_provider.update_resource(
             self.all_resources[request.logical_resource_id],
             stack_name=request.stack_name,
             resources=self.all_resources,
         )
+
+        # incredibly hacky :|
+        resource_provider.resource_json["PhysicalResourceId"] = self.all_resources[
+            request.logical_resource_id
+        ]["PhysicalResourceId"]
         resource_provider.fetch_and_update_state(
             stack_name=request.stack_name, resources=self.all_resources
         )
+        self.all_resources[request.logical_resource_id][
+            "_state_"
+        ] = resource_provider.resource_json["_state_"]
+
         return ProgressEvent(
             status=OperationStatus.SUCCESS,
-            resource_model=self.all_resources[request.logical_resource_id]["Properties"],
+            resource_model=resource_provider.props,
         )
 
     def delete(self, request: ResourceRequest[Properties]) -> ProgressEvent[Properties]:
         return self.create_or_delete(request)
 
     def create_or_delete(self, request: ResourceRequest[Properties]) -> ProgressEvent[Properties]:
         resource_provider = self.resource_provider_cls(
             # TODO: other top level keys
             resource_json={
                 "Type": self.resource_type,
                 "Properties": request.desired_state,
                 "PhysicalResourceId": self.all_resources[request.logical_resource_id].get(
                     "PhysicalResourceId"
                 ),
+                "_state_": request.previous_state,
+                "LogicalResourceId": request.logical_resource_id,
             },
             region_name=request.region_name,
         )
         # TODO: only really necessary for the create and update operation
         resource_provider.add_defaults(
             self.all_resources[request.logical_resource_id], request.stack_name
         )
+        # for some reason add_defaults doesn't even change the values in the resource provider...
+        # incredibly hacky again but should take care of the defaults
+        resource_provider.resource_json["Properties"] = self.all_resources[
+            request.logical_resource_id
+        ]["Properties"]
+        resource_provider.properties = self.all_resources[request.logical_resource_id]["Properties"]
 
         func_details = resource_provider.get_deploy_templates()
         # TODO: be less strict about the return value of func_details
         LOG.debug(
             'Running action "%s" for resource type "%s" id "%s"',
             request.action,
             self.resource_type,
@@ -541,15 +536,28 @@
                         self.all_resources[request.logical_resource_id],
                     )
                 else:
                     result_handler(
                         result, request.logical_resource_id, self.all_resources, self.resource_type
                     )
 
-        return ProgressEvent(status=OperationStatus.SUCCESS, resource_model=resource["Properties"])
+        if request.action.lower() == "add":
+            resource_provider.resource_json["PhysicalResourceId"] = self.all_resources[
+                request.logical_resource_id
+            ]["PhysicalResourceId"]
+
+            # incredibly hacky :|
+            resource_provider.fetch_and_update_state(
+                stack_name=request.stack_name, resources=self.all_resources
+            )
+            self.all_resources[request.logical_resource_id][
+                "_state_"
+            ] = resource_provider.resource_json["_state_"]
+
+        return ProgressEvent(status=OperationStatus.SUCCESS, resource_model=resource_provider.props)
 
 
 class NoResourceProvider(Exception):
     pass
 
 
 def resolve_json_pointer(resource_props: Properties, primary_id_path: str) -> str:
@@ -593,51 +601,69 @@
     ) -> ProgressEvent[Properties]:
         payload = copy.deepcopy(raw_payload)
 
         for current_iteration in range(max_iterations):
             resource_type = get_resource_type(
                 {"Type": raw_payload["resourceType"]}
             )  # TODO: simplify signature of get_resource_type to just take the type
-            resource_provider = self.load_resource_provider(resource_type)
-            event = self.execute_action(resource_provider, payload)
+            try:
+                resource_provider = self.load_resource_provider(resource_type)
+                event = self.execute_action(resource_provider, payload)
+
+                if event.status == OperationStatus.SUCCESS:
+                    logical_resource_id = raw_payload["requestData"]["logicalResourceId"]
+                    resource = self.resources[logical_resource_id]
+                    if "PhysicalResourceId" not in resource:
+                        # branch for non-legacy providers
+                        # TODO: move out of if? (physical res id can be set earlier possibly)
+                        if isinstance(resource_provider, LegacyResourceProvider):
+                            raise Exception(
+                                "A GenericBaseModel should always have a PhysicalResourceId set after deployment"
+                            )
 
-            if event.status == OperationStatus.SUCCESS:
-                logical_resource_id = raw_payload["requestData"]["logicalResourceId"]
-                resource = self.resources[logical_resource_id]
-                if "PhysicalResourceId" not in resource:
-                    # branch for non-legacy providers
-                    # TODO: move out of if? (physical res id can be set earlier possibly)
-                    if isinstance(resource_provider, LegacyResourceProvider):
-                        raise Exception(
-                            "A GenericBaseModel should always have a PhysicalResourceId set after deployment"
-                        )
+                        if not hasattr(resource_provider, "SCHEMA"):
+                            raise Exception(
+                                "A ResourceProvider should always have a SCHEMA property defined."
+                            )
 
-                    if not hasattr(resource_provider, "SCHEMA"):
-                        raise Exception(
-                            "A ResourceProvider should always have a SCHEMA property defined."
+                        resource_type_schema = resource_provider.SCHEMA
+                        physical_resource_id = (
+                            self.extract_physical_resource_id_from_model_with_schema(
+                                event.resource_model,
+                                raw_payload["resourceType"],
+                                resource_type_schema,
+                            )
                         )
 
-                    resource_type_schema = resource_provider.SCHEMA
-                    physical_resource_id = self.extract_physical_resource_id_from_model_with_schema(
-                        event.resource_model, raw_payload["resourceType"], resource_type_schema
-                    )
+                        resource["PhysicalResourceId"] = physical_resource_id
+                        resource["Properties"] = event.resource_model
+                    return event
+
+                # update the shared state
+                context = {**payload["callbackContext"], **event.custom_context}
+                payload["callbackContext"] = context
+                payload["requestData"]["resourceProperties"] = event.resource_model
+
+                if current_iteration == 0:
+                    time.sleep(0)
+                else:
+                    time.sleep(sleep_time)
+
+            except NoResourceProvider:
+                log_not_available_message(
+                    raw_payload["resourceType"],
+                    f"No resource provider found for \"{raw_payload['resourceType']}\"",
+                )
+
+                if config.CFN_IGNORE_UNSUPPORTED_RESOURCE_TYPES:
+                    # TODO: figure out a better way to handle non-implemented here?
+                    return ProgressEvent(OperationStatus.SUCCESS, resource_model={})
+                else:
+                    raise  # re-raise here if explicitly enabled
 
-                    resource["PhysicalResourceId"] = physical_resource_id
-                    resource["Properties"] = event.resource_model
-                return event
-
-            # update the shared state
-            context = {**payload["callbackContext"], **event.custom_context}
-            payload["callbackContext"] = context
-            payload["requestData"]["resourceProperties"] = event.resource_model
-
-            if current_iteration == 0:
-                time.sleep(0)
-            else:
-                time.sleep(sleep_time)
         else:
             raise TimeoutError("Could not perform deploy loop action")
 
     def execute_action(
         self, resource_provider: ResourceProvider, raw_payload: ResourceProviderPayload
     ) -> ProgressEvent[Properties]:
         change_type = raw_payload["action"]
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/service_models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/service_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import Optional, TypedDict
 
+from localstack.services.cloudformation.deployment_utils import check_not_found_exception
 from localstack.utils.aws import aws_stack
 
 LOG = logging.getLogger(__name__)
 
 # dict key used to store the deployment state of a resource
 KEY_RESOURCE_STATE = "_state_"
 
@@ -81,51 +82,41 @@
     # GENERIC BASE METHODS
     # ----------------------
 
     def get_cfn_attribute(self, attribute_name):
         """Retrieve the given CF attribute for this resource"""
         return self.props.get(attribute_name)
 
-    # TODO: make this stricter
-    def get_ref(self):
-        return self.physical_resource_id
-
     # ---------------------
     # GENERIC UTIL METHODS
     # ---------------------
 
     # TODO: remove
     def fetch_and_update_state(self, *args, **kwargs):
         if self.physical_resource_id is None:
             return None
 
-        from localstack.services.cloudformation.engine import template_deployer
-
         try:
             state = self.fetch_state(*args, **kwargs)
             self.update_state(state)
             return state
         except Exception as e:
-            if not template_deployer.check_not_found_exception(
-                e, self.resource_type, self.properties
-            ):
-                LOG.debug("Unable to fetch state for resource %s: %s", self, e)
-
-    # TODO: remove
-    def fetch_state_if_missing(self, *args, **kwargs):
-        if not self.state:
-            self.fetch_and_update_state(*args, **kwargs)
-        return self.state
+            if not check_not_found_exception(e, self.resource_type, self.properties):
+                LOG.warning(
+                    "Unable to fetch state for resource %s: %s",
+                    self,
+                    e,
+                    exc_info=LOG.isEnabledFor(logging.DEBUG),
+                )
 
     # TODO: remove
     def update_state(self, details):
         """Update the deployment state of this resource (existing attributes will be overwritten)."""
         details = details or {}
         self.state.update(details)
-        return self.props
 
     @property
     def physical_resource_id(self) -> str | None:
         """Return the (cached) physical resource ID."""
         return self.resource_json.get("PhysicalResourceId")
 
     @property
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudformation/stores.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/cloudwatch/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/server.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodb/utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/exceptions.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ec2/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/edge.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/es/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/events/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/events/scheduler.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/mappers.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/firehose/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/generic_proxy.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,17 @@
             #     Tags=model["Tags"],
             # )
 
             # this kind of logic below was previously done in either a result_handler or a custom "_post_create" function
             for group in model.get("Groups", []):
                 iam_client.add_user_to_group(GroupName=group, UserName=model["UserName"])
 
+            for policy_arn in model.get("ManagedPolicyArns", []):
+                iam_client.attach_user_policy(UserName=model["UserName"], PolicyArn=policy_arn)
+
             request.custom_context[REPEATED_INVOCATION] = True
             return ProgressEvent(
                 status=OperationStatus.IN_PROGRESS,
                 resource_model=model,
                 custom_context=request.custom_context,
             )
 
@@ -137,15 +140,16 @@
     def update(
         self,
         request: ResourceRequest[IAMUserProperties],
     ) -> ProgressEvent[IAMUserProperties]:
         """
         Update a resource
         """
-        raise NotImplementedError
+        return ProgressEvent(OperationStatus.SUCCESS, request.desired_state)
+        # raise NotImplementedError
 
 
 class IAMUserProviderPlugin(CloudFormationResourceProviderPlugin):
     name = "AWS::IAM::User"
 
     def __init__(self):
         self.factory: Optional[Type[ResourceProvider]] = None
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.2.1.dev20230726085137/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/infra.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/internal.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kinesis/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/local_kms_server.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/kms/utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/logs/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/logs/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/messages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/moto.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/motoserver.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/opensearch/versions.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/plugins.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/providers.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/redshift/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/route53/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/route53resolver/utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/constants.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/cors.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/multipart_content.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/notifications.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/presigned_url.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/provider_stream.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_starter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/s3_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/virtual_host.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/s3/website_hosting.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/secretsmanager/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ses/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/constants.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sns/publisher.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/constants.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/exceptions.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/query_api.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sqs/utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.2.1.dev20230726085137/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/packages.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/stores.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/sts/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/services/transcribe/provider.py` & `localstack-core-2.2.1.dev20230726085137/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/state/core.py` & `localstack-core-2.2.1.dev20230726085137/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/state/inspect.py` & `localstack-core-2.2.1.dev20230726085137/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/state/pickle.py` & `localstack-core-2.2.1.dev20230726085137/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/state/snapshot.py` & `localstack-core-2.2.1.dev20230726085137/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/asf_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/aws/util.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/filters.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/fixtures.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/snapshot.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/pytest/util.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/prototype.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/report.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.2.1.dev20230726085137/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/cli.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/events.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/logger.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/metadata.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/publisher.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/analytics/usage.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/archives.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/asyncio.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/auth.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/arns.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_models.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_responses.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/aws_stack.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/client_types.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/queries.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/request_context.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/resources.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/aws/templating.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/bootstrap.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/collections.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/common.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/config_listener.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_networking.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/container_client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/coverage_docs.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/crypto.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/diagnose.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/docker_utils.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/files.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/functions.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/http.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/json.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/net.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/numbers.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/objects.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/patch.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/platform.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/run.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/scheduler.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/server/http2_server.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/server/proxy_server.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/serving.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/ssl.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/strings.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/sync.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/tagging.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/tail.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/testutil.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/threads.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/time.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/urls.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/venv.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack/utils/xml.py` & `localstack-core-2.2.1.dev20230726085137/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230726070746
+Version: 2.2.1.dev20230726085137
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/plux.json` & `localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8685548293391431%*

 * *Differences: {"'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infr […]*

```diff
@@ -51,44 +51,44 @@
         "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
         "configure_edge_port=localstack.plugins:configure_edge_port",
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
+        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
-        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package"
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230726070746/localstack_core.egg-info/requires.txt` & `localstack-core-2.2.1.dev20230726085137/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/pyproject.toml` & `localstack-core-2.2.1.dev20230726085137/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230726070746/setup.cfg` & `localstack-core-2.2.1.dev20230726085137/setup.cfg`

 * *Files identical despite different names*


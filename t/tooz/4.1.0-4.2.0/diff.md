# Comparing `tmp/tooz-4.1.0.tar.gz` & `tmp/tooz-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooz-4.1.0.tar", last modified: Tue May 30 16:50:49 2023, max compression
+gzip compressed data, was "tooz-4.2.0.tar", last modified: Wed Jul 26 12:02:55 2023, max compression
```

## Comparing `tooz-4.1.0.tar` & `tooz-4.2.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.165196 tooz-4.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-30 16:50:03.000000 tooz-4.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-30 16:50:03.000000 tooz-4.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-05-30 16:50:03.000000 tooz-4.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-05-30 16:50:03.000000 tooz-4.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3817 2023-05-30 16:50:48.000000 tooz-4.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2023-05-30 16:50:03.000000 tooz-4.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25004 2023-05-30 16:50:48.000000 tooz-4.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-30 16:50:03.000000 tooz-4.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2023-05-30 16:50:49.165196 tooz-4.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-05-30 16:50:03.000000 tooz-4.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-30 16:50:03.000000 tooz-4.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/compatibility.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7249 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.145194 tooz-4.1.0/doc/source/user/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/coordinator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/group_membership.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/hashring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/leader_election.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/lock.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-05-30 16:50:03.000000 tooz-4.1.0/doc/source/user/tutorial/partitioner.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.149194 tooz-4.1.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/coordinator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/coordinator_heartbeat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/group_membership.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/group_membership_watch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/leader_election.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/lock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-05-30 16:50:03.000000 tooz-4.1.0/examples/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.149194 tooz-4.1.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-05-30 16:50:03.000000 tooz-4.1.0/playbooks/stop-redis.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.141194 tooz-4.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.153195 tooz-4.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.153195 tooz-4.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.153195 tooz-4.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.153195 tooz-4.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-30 16:50:03.000000 tooz-4.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-05-30 16:50:03.000000 tooz-4.1.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2023-05-30 16:50:03.000000 tooz-4.1.0/run-examples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2023-05-30 16:50:03.000000 tooz-4.1.0/run-tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2023-05-30 16:50:03.000000 tooz-4.1.0/setup-consul-env.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2023-05-30 16:50:03.000000 tooz-4.1.0/setup-etcd-env.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2023-05-30 16:50:49.165196 tooz-4.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2023-05-30 16:50:03.000000 tooz-4.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-05-30 16:50:03.000000 tooz-4.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.157195 tooz-4.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2023-05-30 16:50:03.000000 tooz-4.1.0/tools/compat-matrix.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.157195 tooz-4.1.0/tooz/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31905 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.161195 tooz-4.1.0/tooz/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20604 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/consul.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12833 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/etcd3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15726 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20558 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8482 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/ipc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20294 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/memcached.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8318 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8085 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/pgsql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30379 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/zake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24742 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/drivers/zookeeper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.161195 tooz-4.1.0/tooz/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.165196 tooz-4.1.0/tooz/tests/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/drivers/test_etcd3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2992 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/drivers/test_etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/drivers/test_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41543 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_memcache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_postgresql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2023-05-30 16:50:03.000000 tooz-4.1.0/tooz/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-30 16:50:49.157195 tooz-4.1.0/tooz.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2023-05-30 16:50:49.000000 tooz-4.1.0/tooz.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2023-05-30 16:50:48.000000 tooz-4.1.0/tooz.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2491 2023-05-30 16:50:03.000000 tooz-4.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.041489 tooz-4.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-07-26 12:02:28.000000 tooz-4.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-07-26 12:02:28.000000 tooz-4.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-07-26 12:02:28.000000 tooz-4.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-07-26 12:02:28.000000 tooz-4.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3817 2023-07-26 12:02:54.000000 tooz-4.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2023-07-26 12:02:28.000000 tooz-4.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25054 2023-07-26 12:02:54.000000 tooz-4.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-26 12:02:28.000000 tooz-4.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2023-07-26 12:02:55.045489 tooz-4.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-07-26 12:02:28.000000 tooz-4.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-07-26 12:02:28.000000 tooz-4.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/compatibility.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7249 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/doc/source/user/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/coordinator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/group_membership.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/hashring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/leader_election.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/lock.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-07-26 12:02:28.000000 tooz-4.2.0/doc/source/user/tutorial/partitioner.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/coordinator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/coordinator_heartbeat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/group_membership.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/group_membership_watch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/leader_election.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/lock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-07-26 12:02:28.000000 tooz-4.2.0/examples/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.033489 tooz-4.2.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-07-26 12:02:28.000000 tooz-4.2.0/playbooks/stop-redis.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.029489 tooz-4.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-26 12:02:28.000000 tooz-4.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-07-26 12:02:28.000000 tooz-4.2.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2023-07-26 12:02:28.000000 tooz-4.2.0/run-examples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2023-07-26 12:02:28.000000 tooz-4.2.0/run-tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2023-07-26 12:02:28.000000 tooz-4.2.0/setup-consul-env.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2023-07-26 12:02:28.000000 tooz-4.2.0/setup-etcd-env.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2023-07-26 12:02:55.045489 tooz-4.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2023-07-26 12:02:28.000000 tooz-4.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-07-26 12:02:28.000000 tooz-4.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2023-07-26 12:02:28.000000 tooz-4.2.0/tools/compat-matrix.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.037489 tooz-4.2.0/tooz/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31905 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/coordination.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.041489 tooz-4.2.0/tooz/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20604 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/consul.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12833 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/etcd3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15726 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20558 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8482 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/ipc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20294 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/memcached.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8215 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8085 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/pgsql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30379 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/zake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24742 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/drivers/zookeeper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.041489 tooz-4.2.0/tooz/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.041489 tooz-4.2.0/tooz/tests/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/drivers/test_etcd3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2992 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/drivers/test_etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/drivers/test_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41543 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_memcache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4034 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_postgresql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2023-07-26 12:02:28.000000 tooz-4.2.0/tooz/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-26 12:02:55.041489 tooz-4.2.0/tooz.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2023-07-26 12:02:55.000000 tooz-4.2.0/tooz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2023-07-26 12:02:54.000000 tooz-4.2.0/tooz.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2491 2023-07-26 12:02:28.000000 tooz-4.2.0/tox.ini
```

### Comparing `tooz-4.1.0/.pre-commit-config.yaml` & `tooz-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/.zuul.yaml` & `tooz-4.2.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/AUTHORS` & `tooz-4.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/CONTRIBUTING.rst` & `tooz-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/ChangeLog` & `tooz-4.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+4.2.0
+-----
+
+* Fix: Add timeout for mysql driver
+
 4.1.0
 -----
 
 * Revert "Moves supported python runtimes from version 3.8 to 3.10"
 
 4.0.0
 -----
```

### Comparing `tooz-4.1.0/LICENSE` & `tooz-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/PKG-INFO` & `tooz-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 4.1.0
+Version: 4.2.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
```

### Comparing `tooz-4.1.0/README.rst` & `tooz-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/requirements.txt` & `tooz-4.2.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/conf.py` & `tooz-4.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/index.rst` & `tooz-4.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/install/index.rst` & `tooz-4.2.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/reference/index.rst` & `tooz-4.2.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/compatibility.rst` & `tooz-4.2.0/doc/source/user/compatibility.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/drivers.rst` & `tooz-4.2.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/tutorial/coordinator.rst` & `tooz-4.2.0/doc/source/user/tutorial/coordinator.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/tutorial/group_membership.rst` & `tooz-4.2.0/doc/source/user/tutorial/group_membership.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/tutorial/leader_election.rst` & `tooz-4.2.0/doc/source/user/tutorial/leader_election.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/doc/source/user/tutorial/lock.rst` & `tooz-4.2.0/doc/source/user/tutorial/lock.rst`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/coordinator.py` & `tooz-4.2.0/examples/coordinator.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/coordinator_heartbeat.py` & `tooz-4.2.0/examples/coordinator_heartbeat.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/group_membership.py` & `tooz-4.2.0/examples/group_membership.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/group_membership_watch.py` & `tooz-4.2.0/examples/group_membership_watch.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/hashring.py` & `tooz-4.2.0/examples/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/leader_election.py` & `tooz-4.2.0/examples/leader_election.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/lock.py` & `tooz-4.2.0/examples/lock.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/examples/partitioner.py` & `tooz-4.2.0/examples/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml` & `tooz-4.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml` & `tooz-4.2.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/releasenotes/source/conf.py` & `tooz-4.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/setup-consul-env.sh` & `tooz-4.2.0/setup-consul-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/setup-etcd-env.sh` & `tooz-4.2.0/setup-etcd-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/setup.cfg` & `tooz-4.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/setup.py` & `tooz-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tools/compat-matrix.py` & `tooz-4.2.0/tools/compat-matrix.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/__init__.py` & `tooz-4.2.0/tooz/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/_retry.py` & `tooz-4.2.0/tooz/_retry.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/coordination.py` & `tooz-4.2.0/tooz/coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/consul.py` & `tooz-4.2.0/tooz/drivers/consul.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/etcd.py` & `tooz-4.2.0/tooz/drivers/etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/etcd3.py` & `tooz-4.2.0/tooz/drivers/etcd3.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/etcd3gw.py` & `tooz-4.2.0/tooz/drivers/etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/file.py` & `tooz-4.2.0/tooz/drivers/file.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/ipc.py` & `tooz-4.2.0/tooz/drivers/ipc.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/memcached.py` & `tooz-4.2.0/tooz/drivers/memcached.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/mysql.py` & `tooz-4.2.0/tooz/drivers/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     MYSQL_DEFAULT_PORT = 3306
 
     def __init__(self, name, parsed_url, options):
         super(MySQLLock, self).__init__(name)
         self.acquired = False
         self._conn = MySQLDriver.get_connection(parsed_url, options, True)
 
-    def acquire(self, blocking=True, shared=False):
+    def acquire(self, blocking=True, shared=False, timeout=0):
 
         if shared:
             raise tooz.NotImplemented
 
         @_retry.retry(stop_max_delay=blocking)
         def _lock():
             # NOTE(sileht): mysql-server (<5.7.5) allows only one lock per
@@ -54,22 +54,20 @@
             #
             # So, we track locally the lock status with self.acquired
             if self.acquired is True:
                 if blocking:
                     raise _retry.TryAgain
                 return False
 
-            _, timeout = utils.convert_blocking(blocking)
             try:
                 if not self._conn.open:
                     self._conn.connect()
                 cur = self._conn.cursor()
                 cur.execute(
-                    ("SELECT GET_LOCK(%s, "
-                     f"{timeout if timeout is not None else '0'});"),
+                    (f"SELECT GET_LOCK(%s, {timeout});"),
                     self.name
                 )
                 # Can return NULL on error
                 if cur.fetchone()[0] == 1:
                     self.acquired = True
                     return True
             except pymysql.MySQLError as e:
```

### Comparing `tooz-4.1.0/tooz/drivers/pgsql.py` & `tooz-4.2.0/tooz/drivers/pgsql.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/redis.py` & `tooz-4.2.0/tooz/drivers/redis.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/zake.py` & `tooz-4.2.0/tooz/drivers/zake.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/drivers/zookeeper.py` & `tooz-4.2.0/tooz/drivers/zookeeper.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/hashring.py` & `tooz-4.2.0/tooz/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/locking.py` & `tooz-4.2.0/tooz/locking.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/partitioner.py` & `tooz-4.2.0/tooz/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/__init__.py` & `tooz-4.2.0/tooz/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/drivers/test_etcd3.py` & `tooz-4.2.0/tooz/tests/drivers/test_etcd3.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/drivers/test_etcd3gw.py` & `tooz-4.2.0/tooz/tests/drivers/test_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/drivers/test_file.py` & `tooz-4.2.0/tooz/tests/drivers/test_file.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_coordination.py` & `tooz-4.2.0/tooz/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_etcd.py` & `tooz-4.2.0/tooz/tests/test_etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_hashring.py` & `tooz-4.2.0/tooz/tests/test_hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_memcache.py` & `tooz-4.2.0/tooz/tests/test_memcache.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_mysql.py` & `tooz-4.2.0/tooz/tests/test_mysql.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,13 +88,27 @@
 
     @mock.patch("pymysql.Connect")
     def test_parsing_timeout_settings(self, sql_mock):
         c = self._create_coordinator("mysql://localhost:3306/test")
         c.start()
 
         name = tests.get_random_uuid()
-        blocking_value = 10.12
+        blocking_value = False
+        timeout = 10.1
+        lock = c.get_lock(name)
+        with mock.patch.object(lock, 'acquire', wraps=True, autospec=True) as \
+                mock_acquire:
+            with lock(blocking_value, timeout):
+                mock_acquire.assert_called_once_with(blocking_value, timeout)
+
+    @mock.patch("pymysql.Connect")
+    def test_parsing_blocking_settings(self, sql_mock):
+        c = self._create_coordinator("mysql://localhost:3306/test")
+        c.start()
+
+        name = tests.get_random_uuid()
+        blocking_value = True
         lock = c.get_lock(name)
         with mock.patch.object(lock, 'acquire', wraps=True, autospec=True) as \
                 mock_acquire:
             with lock(blocking_value):
                 mock_acquire.assert_called_once_with(blocking_value)
```

### Comparing `tooz-4.1.0/tooz/tests/test_partitioner.py` & `tooz-4.2.0/tooz/tests/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_postgresql.py` & `tooz-4.2.0/tooz/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/tests/test_utils.py` & `tooz-4.2.0/tooz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz/utils.py` & `tooz-4.2.0/tooz/utils.py`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz.egg-info/PKG-INFO` & `tooz-4.2.0/tooz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 4.1.0
+Version: 4.2.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
```

### Comparing `tooz-4.1.0/tooz.egg-info/SOURCES.txt` & `tooz-4.2.0/tooz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz.egg-info/entry_points.txt` & `tooz-4.2.0/tooz.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tooz.egg-info/requires.txt` & `tooz-4.2.0/tooz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tooz-4.1.0/tox.ini` & `tooz-4.2.0/tox.ini`

 * *Files identical despite different names*


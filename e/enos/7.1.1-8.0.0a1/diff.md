# Comparing `tmp/enos-7.1.1.tar.gz` & `tmp/enos-8.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enos-7.1.1.tar", max compression
+gzip compressed data, was "enos-8.0.0a1.tar", max compression
```

## Comparing `enos-7.1.1.tar` & `enos-8.0.0a1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    35148 2021-03-03 15:45:14.312860 enos-7.1.1/LICENSE
--rw-r--r--   0        0        0     3427 2021-06-01 17:12:26.824000 enos-7.1.1/README.rst
--rw-r--r--   0        0        0        0 2021-03-03 15:45:14.316860 enos-7.1.1/enos/__init__.py
--rw-r--r--   0        0        0      529 2021-04-28 15:36:26.880345 enos-7.1.1/enos/ansible/enos.yml
--rw-r--r--   0        0        0      372 2021-04-28 15:36:26.880345 enos-7.1.1/enos/ansible/group_vars/all.yml
--rw-r--r--   0        0        0      378 2021-04-28 15:36:26.880345 enos-7.1.1/enos/ansible/init_os.yml
--rw-r--r--   0        0        0     4979 2021-03-03 15:45:14.316860 enos-7.1.1/enos/ansible/plugins/callback/influxdb_events.py
--rw-r--r--   0        0        0       44 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/defaults/main.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/backup.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/bench.yml
--rw-r--r--   0        0        0     1417 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/deploy.yml
--rw-r--r--   0        0        0      311 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/main.yml
--rw-r--r--   0        0        0      116 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/cadvisor/tasks/pull.yml
--rw-r--r--   0        0        0      280 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/defaults/main.yml
--rw-r--r--   0        0        0    23358 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/files/collectd.conf
--rw-r--r--   0        0        0       25 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/files/contextswitch.conf
--rw-r--r--   0        0        0      359 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/files/haproxy.conf
--rw-r--r--   0        0        0     9676 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/files/haproxy.py
--rw-r--r--   0        0        0      156 2021-03-03 15:45:14.317860 enos-7.1.1/enos/ansible/roles/collectd/files/protocols.conf
--rw-r--r--   0        0        0      119 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-compute.conf
--rw-r--r--   0        0        0      353 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
--rw-r--r--   0        0        0      249 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
--rw-r--r--   0        0        0       69 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
--rw-r--r--   0        0        0       70 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
--rw-r--r--   0        0        0      211 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-network.conf
--rw-r--r--   0        0        0      216 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-nova.conf
--rw-r--r--   0        0        0      128 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/backup.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/bench.yml
--rw-r--r--   0        0        0     1881 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/deploy.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/main.yml
--rw-r--r--   0        0        0       70 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/tasks/pull.yml
--rw-r--r--   0        0        0      114 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/templates/influx.conf.j2
--rw-r--r--   0        0        0      386 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/templates/memcached.conf.j2
--rw-r--r--   0        0        0      455 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/templates/mysql.conf.j2
--rw-r--r--   0        0        0     1081 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       42 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/grafana/defaults/main.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.318860 enos-7.1.1/enos/ansible/roles/grafana/tasks/backup.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/grafana/tasks/bench.yml
--rw-r--r--   0        0        0     1646 2021-04-28 15:36:26.880345 enos-7.1.1/enos/ansible/roles/grafana/tasks/deploy.yml
--rw-r--r--   0        0        0      120 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/grafana/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/grafana/tasks/main.yml
--rw-r--r--   0        0        0      113 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/grafana/tasks/pull.yml
--rw-r--r--   0        0        0       36 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/defaults/main.yml
--rw-r--r--   0        0        0    10241 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/files/config.toml
--rw-r--r--   0        0        0     9721 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/files/types.db
--rw-r--r--   0        0        0      357 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/backup.yml
--rw-r--r--   0        0        0        4 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/bench.yml
--rw-r--r--   0        0        0     1582 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/deploy.yml
--rw-r--r--   0        0        0      207 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/main.yml
--rw-r--r--   0        0        0      113 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/influx/tasks/pull.yml
--rw-r--r--   0        0        0     1104 2021-03-24 17:11:42.489462 enos-7.1.1/enos/ansible/roles/init_os/tasks/deploy.yml
--rw-r--r--   0        0        0       40 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/init_os/tasks/main.yml
--rw-r--r--   0        0        0      493 2021-03-03 15:45:14.319860 enos-7.1.1/enos/ansible/roles/init_os/tasks/pull.yml
--rw-r--r--   0        0        0     3568 2021-04-28 15:36:26.880345 enos-7.1.1/enos/ansible/roles/init_os/templates/init.sh.j2
--rwxr-xr-x   0        0        0    25493 2022-03-18 12:27:58.283161 enos-7.1.1/enos/cli.py
--rw-r--r--   0        0        0        0 2021-03-03 15:45:14.321860 enos-7.1.1/enos/provider/__init__.py
--rw-r--r--   0        0        0     1815 2021-04-28 15:36:26.881346 enos-7.1.1/enos/provider/chameleonbaremetal.py
--rw-r--r--   0        0        0     1293 2021-04-28 15:36:26.881346 enos-7.1.1/enos/provider/chameleonkvm.py
--rw-r--r--   0        0        0     2456 2021-04-29 16:27:16.777027 enos-7.1.1/enos/provider/enos_vagrant.py
--rw-r--r--   0        0        0     6117 2021-04-29 16:27:16.520029 enos-7.1.1/enos/provider/g5k.py
--rw-r--r--   0        0        0      818 2021-03-03 15:45:14.321860 enos-7.1.1/enos/provider/host.py
--rw-r--r--   0        0        0     3002 2021-04-28 15:36:26.881346 enos-7.1.1/enos/provider/openstack.py
--rw-r--r--   0        0        0     1636 2021-05-21 09:07:54.938698 enos-7.1.1/enos/provider/provider.py
--rw-r--r--   0        0        0     2797 2021-04-28 15:36:26.882346 enos-7.1.1/enos/provider/static.py
--rw-r--r--   0        0        0     2757 2021-04-28 15:36:26.882346 enos-7.1.1/enos/provider/vmong5k.py
--rw-r--r--   0        0        0     9863 2021-06-01 08:24:12.173336 enos-7.1.1/enos/resources/inventory.sample
--rw-r--r--   0        0        0    21531 2021-04-28 15:36:26.882346 enos-7.1.1/enos/resources/passwords.yml
--rw-r--r--   0        0        0      513 2021-04-28 15:36:26.883345 enos-7.1.1/enos/resources/workload/create-and-update-image.yaml
--rw-r--r--   0        0        0     1069 2021-04-28 15:36:26.883345 enos-7.1.1/enos/resources/workload/nova-boot-list-cc.yml
--rw-r--r--   0        0        0      715 2021-06-01 15:53:22.563891 enos-7.1.1/enos/resources/workload/run.yml
--rw-r--r--   0        0        0      189 2021-04-28 15:36:26.883345 enos-7.1.1/enos/services/__init__.py
--rw-r--r--   0        0        0    14967 2022-03-28 16:22:42.440279 enos-7.1.1/enos/services/kolla.py
--rw-r--r--   0        0        0     8416 2021-06-01 16:24:09.225736 enos-7.1.1/enos/services/rally.py
--rw-r--r--   0        0        0     3760 2021-06-01 16:24:09.225736 enos-7.1.1/enos/services/shaker.py
--rwxr-xr-x   0        0        0    11791 2021-06-01 16:24:27.250539 enos-7.1.1/enos/tasks/__init__.py
--rw-r--r--   0        0        0     5658 2021-05-20 08:19:23.434355 enos-7.1.1/enos/tasks/new.py
--rw-r--r--   0        0        0    11478 2022-03-18 12:27:58.000161 enos-7.1.1/enos/tasks/up.py
--rw-r--r--   0        0        0      911 2021-03-03 15:45:14.321860 enos-7.1.1/enos/templates/Vagrantfile.j2
--rw-r--r--   0        0        0    10240 2021-03-03 15:45:14.321860 enos-7.1.1/enos/templates/grafana_dashboard.json
--rw-r--r--   0        0        0     2051 2021-04-29 16:17:03.816563 enos-7.1.1/enos/templates/reservation.yaml.j2
--rw-r--r--   0        0        0        0 2021-03-03 15:45:14.321860 enos-7.1.1/enos/utils/__init__.py
--rw-r--r--   0        0        0     3333 2021-04-14 17:03:24.315094 enos-7.1.1/enos/utils/build.py
--rw-r--r--   0        0        0     3285 2021-06-01 16:24:27.378537 enos-7.1.1/enos/utils/cli.py
--rw-r--r--   0        0        0     1930 2022-03-30 19:41:34.950171 enos-7.1.1/enos/utils/constants.py
--rw-r--r--   0        0        0     1009 2021-06-01 16:24:27.121540 enos-7.1.1/enos/utils/errors.py
--rw-r--r--   0        0        0     6576 2021-06-01 16:24:27.121540 enos-7.1.1/enos/utils/extra.py
--rw-r--r--   0        0        0     1669 2022-03-30 19:41:50.509226 enos-7.1.1/pyproject.toml
--rw-r--r--   0        0        0     5318 2022-03-30 19:48:04.292011 enos-7.1.1/setup.py
--rw-r--r--   0        0        0     4708 2022-03-30 19:48:04.293146 enos-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-10-20 13:50:57.843485 enos-8.0.0a1/LICENSE
+-rw-r--r--   0        0        0     3270 2023-04-25 13:33:13.806401 enos-8.0.0a1/README.rst
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/__init__.py
+-rw-r--r--   0        0        0      529 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/enos.yml
+-rw-r--r--   0        0        0      372 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/group_vars/all.yml
+-rw-r--r--   0        0        0      378 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/init_os.yml
+-rw-r--r--   0        0        0     4979 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/plugins/callback/influxdb_events.py
+-rw-r--r--   0        0        0       44 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/bench.yml
+-rw-r--r--   0        0        0     1417 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/deploy.yml
+-rw-r--r--   0        0        0      311 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/main.yml
+-rw-r--r--   0        0        0      116 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/pull.yml
+-rw-r--r--   0        0        0      280 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/defaults/main.yml
+-rw-r--r--   0        0        0    23358 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/files/collectd.conf
+-rw-r--r--   0        0        0       25 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/contextswitch.conf
+-rw-r--r--   0        0        0      359 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/haproxy.conf
+-rw-r--r--   0        0        0     9676 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/files/haproxy.py
+-rw-r--r--   0        0        0      156 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/protocols.conf
+-rw-r--r--   0        0        0      119 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-compute.conf
+-rw-r--r--   0        0        0      353 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
+-rw-r--r--   0        0        0      249 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
+-rw-r--r--   0        0        0       69 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
+-rw-r--r--   0        0        0      211 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-network.conf
+-rw-r--r--   0        0        0      216 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-nova.conf
+-rw-r--r--   0        0        0      128 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/bench.yml
+-rw-r--r--   0        0        0     1881 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/deploy.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/main.yml
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/tasks/pull.yml
+-rw-r--r--   0        0        0      114 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/templates/influx.conf.j2
+-rw-r--r--   0        0        0      386 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/templates/memcached.conf.j2
+-rw-r--r--   0        0        0      455 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/templates/mysql.conf.j2
+-rw-r--r--   0        0        0     1081 2022-11-07 08:45:07.825216 enos-8.0.0a1/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0       42 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/bench.yml
+-rw-r--r--   0        0        0     1646 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/deploy.yml
+-rw-r--r--   0        0        0      120 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/grafana/tasks/pull.yml
+-rw-r--r--   0        0        0       36 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/defaults/main.yml
+-rw-r--r--   0        0        0    10241 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/files/config.toml
+-rw-r--r--   0        0        0     9721 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/files/types.db
+-rw-r--r--   0        0        0      357 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/bench.yml
+-rw-r--r--   0        0        0     1582 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/deploy.yml
+-rw-r--r--   0        0        0      207 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/influx/tasks/pull.yml
+-rw-r--r--   0        0        0     1112 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/ansible/roles/init_os/tasks/deploy.yml
+-rw-r--r--   0        0        0       40 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/init_os/tasks/main.yml
+-rw-r--r--   0        0        0      493 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/ansible/roles/init_os/tasks/pull.yml
+-rw-r--r--   0        0        0     3434 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/ansible/roles/init_os/templates/init.sh.j2
+-rwxr-xr-x   0        0        0    25701 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/cli.py
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/__init__.py
+-rw-r--r--   0        0        0     1815 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/chameleonbaremetal.py
+-rw-r--r--   0        0        0     1293 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/chameleonkvm.py
+-rw-r--r--   0        0        0     2417 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/provider/enos_vagrant.py
+-rw-r--r--   0        0        0     5813 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/provider/g5k.py
+-rw-r--r--   0        0        0      818 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/host.py
+-rw-r--r--   0        0        0     2963 2023-04-25 13:33:13.806401 enos-8.0.0a1/enos/provider/openstack.py
+-rw-r--r--   0        0        0     1636 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/provider.py
+-rw-r--r--   0        0        0     2786 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/provider/static.py
+-rw-r--r--   0        0        0     2757 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/provider/vmong5k.py
+-rw-r--r--   0        0        0     9471 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/resources/inventory.sample
+-rw-r--r--   0        0        0     9666 2022-11-08 12:27:03.004104 enos-8.0.0a1/enos/resources/multinode
+-rw-r--r--   0        0        0    21559 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/resources/passwords.yml
+-rw-r--r--   0        0        0      513 2022-11-07 08:45:34.949389 enos-8.0.0a1/enos/resources/workload/create-and-update-image.yaml
+-rw-r--r--   0        0        0     1069 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/resources/workload/nova-boot-list-cc.yml
+-rw-r--r--   0        0        0      715 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/resources/workload/run.yml
+-rw-r--r--   0        0        0      189 2022-11-07 08:45:07.829217 enos-8.0.0a1/enos/services/__init__.py
+-rw-r--r--   0        0        0    14973 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/services/kolla.py
+-rw-r--r--   0        0        0     8376 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/services/rally.py
+-rw-r--r--   0        0        0     3720 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/services/shaker.py
+-rwxr-xr-x   0        0        0    11791 2022-11-07 10:41:09.316608 enos-8.0.0a1/enos/tasks/__init__.py
+-rw-r--r--   0        0        0     5701 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/tasks/new.py
+-rw-r--r--   0        0        0    12116 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/tasks/up.py
+-rw-r--r--   0        0        0      911 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/templates/Vagrantfile.j2
+-rw-r--r--   0        0        0    10240 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/templates/grafana_dashboard.json
+-rw-r--r--   0        0        0     2049 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/templates/reservation.yaml.j2
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/utils/__init__.py
+-rw-r--r--   0        0        0     3229 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/utils/build.py
+-rw-r--r--   0        0        0     3285 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/utils/cli.py
+-rw-r--r--   0        0        0     1932 2023-04-25 14:21:48.249279 enos-8.0.0a1/enos/utils/constants.py
+-rw-r--r--   0        0        0     1009 2022-11-07 08:45:07.833218 enos-8.0.0a1/enos/utils/errors.py
+-rw-r--r--   0        0        0     6257 2023-04-25 13:33:13.810401 enos-8.0.0a1/enos/utils/extra.py
+-rw-r--r--   0        0        0     1907 2023-04-25 14:25:55.272235 enos-8.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 enos-8.0.0a1/PKG-INFO
```

### Comparing `enos-7.1.1/LICENSE` & `enos-8.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/README.rst` & `enos-8.0.0a1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|Build Status| |Doc Status| |Pypi| |Code style| |License|
+|Doc Status| |Pypi| |Code style| |License|
 
 Join us on gitter :  |Join the chat at
 https://gitter.im/BeyondTheClouds/enos|
 
 About Enos
 ==========
 
@@ -65,16 +65,14 @@
 Links
 =====
 
 -  Docs - https://beyondtheclouds.github.io/enos/
 -  Discovery - https://beyondtheclouds.github.io/
 -  Docker - https://hub.docker.com/r/beyondtheclouds/
 
-.. |Build Status| image:: https://travis-ci.org/BeyondTheClouds/enos.svg?branch=master
-   :target: https://travis-ci.org/BeyondTheClouds/enos
 .. |Join the chat at https://gitter.im/BeyondTheClouds/enos| image:: https://badges.gitter.im/BeyondTheClouds/enos.svg
    :target: https://gitter.im/BeyondTheClouds/enos?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
 .. |Code style| image:: https://api.codacy.com/project/badge/Grade/87536e9c0f0d47e08d1b9e0950c9d14b
    :target: https://www.codacy.com/app/msimonin/enos?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=BeyondTheClouds/enos&amp;utm_campaign=Badge_Grade
 .. |License| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
 .. |Pypi| image:: https://badge.fury.io/py/enos.svg
```

### Comparing `enos-7.1.1/enos/ansible/enos.yml` & `enos-8.0.0a1/enos/ansible/enos.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/plugins/callback/influxdb_events.py` & `enos-8.0.0a1/enos/ansible/plugins/callback/influxdb_events.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/cadvisor/tasks/deploy.yml` & `enos-8.0.0a1/enos/ansible/roles/cadvisor/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/collectd/files/collectd.conf` & `enos-8.0.0a1/enos/ansible/roles/collectd/files/collectd.conf`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/collectd/files/haproxy.py` & `enos-8.0.0a1/enos/ansible/roles/collectd/files/haproxy.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/collectd/tasks/deploy.yml` & `enos-8.0.0a1/enos/ansible/roles/collectd/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2` & `enos-8.0.0a1/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/grafana/tasks/deploy.yml` & `enos-8.0.0a1/enos/ansible/roles/grafana/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/influx/files/config.toml` & `enos-8.0.0a1/enos/ansible/roles/influx/files/config.toml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/influx/files/types.db` & `enos-8.0.0a1/enos/ansible/roles/influx/files/types.db`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/influx/tasks/deploy.yml` & `enos-8.0.0a1/enos/ansible/roles/influx/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/ansible/roles/init_os/tasks/deploy.yml` & `enos-8.0.0a1/enos/ansible/roles/init_os/tasks/deploy.yml`

 * *Files 22% similar despite different names*

```diff
@@ -12,30 +12,26 @@
     path: /srv/init_os/init.sh
     mode: 0755
 
 - name: Get the reference on the kolla-toolbox image
   shell: "{% raw %} docker images --format '{{ .Repository }}:{{ .Tag }}' | grep kolla-toolbox {% endraw %}"
   register: kolla_toolbox_image
 
+# Run without detaching to get exit status, but handle errors separately (next task).
+# This avoids displaying a huge error if the init script fails.
 - name: Launch init in kolla_toolbox container
   docker_container:
     name: kolla_toolbox
     env: "{{ os_env }}"
-    command: "/srv/init_os/init.sh"
+    command: ["/srv/init_os/init.sh"]
     image: "{{ kolla_toolbox_image.stdout }}"
+    detach: false
     volumes:
       - /srv/init_os:/srv/init_os
+  ignore_errors: true
   register: docker_output
 
-- name: Wait for the end of the init...
-  command: "docker ps -q --filter id={{ docker_output.ansible_facts.docker_container.Id }}"
-  register: finished
-  until: finished.stdout == ""
-  delay: 5
-  retries:  100
-
-- name: Init report
-  command: "docker logs {{ docker_output.ansible_facts.docker_container.Id }}"
-  register: init_output
-
-- name: Init report
-  debug: var=init_output
+- name: Check exit status of init script
+  assert:
+    that: "not docker_output.failed"
+    fail_msg: "Openstack init script failed"
+    success_msg: "Openstack init script completed successfully"
```

### Comparing `enos-7.1.1/enos/ansible/roles/init_os/templates/init.sh.j2` & `enos-8.0.0a1/enos/ansible/roles/init_os/templates/init.sh.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env bash
 
 set -x
 
-DNS_NAMESERVER={{ provider_net.dns }}
-SUBNET_RANGE={{ provider_net.cidr }}
-ALLOCATION_POOL_START={{ provider_net.start }}
-ALLOCATION_POOL_END={{ provider_net.end }}
+DNS_NAMESERVER={{ provider_net.dns|default("9.9.9.9", true) }}
+SUBNET_RANGE={{ provider_net.network }}
 GATEWAY={{ provider_net.gateway }}
 
 ## Images
 openstack image show debian-10 || openstack image create --disk-format=qcow2 --container-format=bare --property architecture=x86_64 --public --file /srv/init_os/debian-10.qcow2 debian-10
 openstack image show cirros.uec || openstack image create --disk-format=qcow2 --container-format=bare --property architecture=x86_64 --public --file /srv/init_os/cirros.uec.qcow2 cirros.uec
 
 
@@ -28,15 +26,15 @@
 ### private-subnet
 openstack subnet show private-subnet || openstack subnet create private-subnet --network private --subnet-range 10.0.0.0/24 --gateway 10.0.0.1 --dns-nameserver $DNS_NAMESERVER --ip-version 4
 
 ### public
 openstack network show public || openstack network create public --share --provider-physical-network physnet1 --provider-network-type flat --external
 
 ### public-subnet
-openstack subnet show public-subnet || openstack subnet create public-subnet --network public --subnet-range $SUBNET_RANGE --no-dhcp --allocation-pool start=$ALLOCATION_POOL_START,end=$ALLOCATION_POOL_END --gateway $GATEWAY --dns-nameserver $DNS_NAMESERVER --ip-version 4
+openstack subnet show public-subnet || openstack subnet create public-subnet --network public --subnet-range $SUBNET_RANGE --no-dhcp --gateway $GATEWAY --dns-nameserver $DNS_NAMESERVER --ip-version 4
 
 
 # Router
 openstack router show router || openstack router create router
 openstack router show router -c external_gateway_info -f value | fgrep -v None || openstack router set router --external-gateway public
 openstack router show router -c interfaces_info -f value|fgrep -v "[]" || openstack router add subnet router private-subnet
```

### Comparing `enos-7.1.1/enos/cli.py` & `enos-8.0.0a1/enos/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,15 +567,15 @@
                        [default: centos].
     --box BOX          Reference box for host virtual machines (vagrant)
     --cluster CLUSTER  Cluster where the image is built (g5k and vmong5k)
                        [default: parasilo].
     --directory DIR    Directory in which the image will be baked (vmong5k)
                        [default: ~/.enos].
     --environment ENV  Reference environment for deployment (g5k)
-                       [default: debian10-x64-min].
+                       [default: debian10-min].
     --image IMAGE      Reference image path to bake on top of it (vmong5k)
                        [default: /grid5000/virt-images/debian10-x64-base.qcow2].
     --type TYPE        Installation type of the BASE distribution
                        [default: binary].
     """
 
     logging.debug('phase[build]: args=%s' % kwargs)
@@ -729,14 +729,19 @@
     # Parse command arguments: `enos -vv help new`
     # cli_args =
     #  {'--help': False, '--quiet': False, '--verbose': 2, '--version': False,
     #   '<command>': 'help','<args>': ['new'], }
     enos_global_args = docopt(__doc__ or "",
                               version=C.VERSION,
                               options_first=True,)
+    # Set global enoslib options
+    import enoslib
+    # Use the "old-style" Ansible output in order to get more detailed
+    # output, useful in case of errors.
+    enoslib.set_config(ansible_stdout="classic")
 
     # Set the logging level
     _set_logging_level(
         is_quiet=enos_global_args.pop('--quiet', False),
         verbose_level=enos_global_args.pop('--verbose', 0))
 
     # Get the command to execute and its associated function
```

### Comparing `enos-7.1.1/enos/provider/chameleonbaremetal.py` & `enos-8.0.0a1/enos/provider/chameleonbaremetal.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/provider/chameleonkvm.py` & `enos-8.0.0a1/enos/provider/chameleonkvm.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/provider/enos_vagrant.py` & `enos-8.0.0a1/enos/provider/enos_vagrant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 import logging
 
 from enos.provider.provider import Provider
-from enos.utils.extra import gen_enoslib_roles
+from enos.utils.extra import expand_groups, gen_enoslib_roles
 
 import enoslib.infra.enos_vagrant.provider as enoslib_vagrant
 from enoslib.infra.enos_vagrant.configuration import Configuration
-from enoslib.service.netem.netem import expand_groups
 
 # - SPHINX_DEFAULT_CONFIG
 DEFAULT_CONFIG = {
     'type': 'vagrant',          # Name of the provider
     'backend': 'virtualbox',    # Name of the virtualization technology
     'box': 'generic/debian10',  # Box -- https://app.vagrantup.com/boxes/search
     'user': 'root',             # SSH user
```

### Comparing `enos-7.1.1/enos/provider/g5k.py` & `enos-8.0.0a1/enos/provider/g5k.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 import copy
 import logging
 
-from enoslib.service.netem.netem import expand_groups
-from enoslib.infra.enos_g5k import (provider, g5k_api_utils, remote)
+from enoslib import run_command
+from enoslib.infra.enos_g5k import (provider, g5k_api_utils)
 from enoslib.infra.enos_g5k.configuration import Configuration
 
 from enos.provider.provider import Provider
-from enos.utils.extra import gen_enoslib_roles
+from enos.utils.extra import expand_groups, gen_enoslib_roles
 from enos.utils.constants import (NETWORK_INTERFACE,
                                   NEUTRON_EXTERNAL_INTERFACE)
 
 
 LOGGER = logging.getLogger(__name__)
 
 # - SPHINX_DEFAULT_CONFIG
 DEFAULT_CONFIG = {
     'type': 'g5k',                   # Name of the provider
     'job_name': 'enos',              # Job name in oarstat/gant
     'walltime': '02:00:00',          # Reservation duration time
-    'env_name': 'debian10-x64-min',  # Environment to deploy (see `kaenv3 -l`)
-    'reservation': '',               # Reservation date
+    'env_name': 'debian11-min',      # Environment to deploy (see `kaenv3 -l`)
     'job_type': 'deploy',            # deploy, besteffort, ...
     'queue': 'default'               # default, production, testing
 }
 # + SPHINX_DEFAULT_CONFIG
 
 DEFAULT_CONN_PARAMS = {'user': 'root'}
 
@@ -117,50 +116,42 @@
                          {"machines": machines,
                           "networks": networks}})
 
     return enoslib_conf
 
 
 def _provision(roles):
-    nodes = []
-    for value in roles.values():
-        nodes.extend(value)
-
-    # remove duplicate hosts
-    # Note(jrbalderrama): do we have to implement hash/equals in Host?
-    nodes = set([node.address for node in nodes])
-
     # Provision nodes so we can run Ansible on it
-    remote.exec_command_on_nodes(
-        nodes,
+    run_command(
         'apt-get update && apt-get -y --force-yes install python',
-        'Installing python...')
+        task_name='Installing python...',
+        roles=roles)
 
     # Bind volumes of docker in /tmp (free storage location on G5k)
-    remote.exec_command_on_nodes(
-        nodes,
+    run_command(
         ('mkdir -p /tmp/docker/volumes; '
          'mkdir -p /var/lib/docker/volumes'),
-        'Creating docker volumes directory in /tmp')
-    remote.exec_command_on_nodes(
-        nodes,
+        task_name='Creating docker volumes directory in /tmp',
+        roles=roles)
+    run_command(
         ('(mount | grep /tmp/docker/volumes) || '
          'mount --bind /tmp/docker/volumes /var/lib/docker/volumes'),
-        'Bind mount')
+        task_name='Bind mount',
+        roles=roles)
 
     # Bind nova local storage in /tmp
-    remote.exec_command_on_nodes(
-        nodes,
+    run_command(
         'mkdir -p /tmp/nova ; mkdir -p /var/lib/nova',
-        'Creating nova directory in /tmp')
-    remote.exec_command_on_nodes(
-        nodes,
+        task_name='Creating nova directory in /tmp',
+        roles=roles)
+    run_command(
         ('(mount | grep /tmp/nova) || '
          'mount --bind /tmp/nova /var/lib/nova'),
-        'Bind mount')
+        task_name='Bind mount',
+        roles=roles)
 
 
 class G5k(Provider):
     """Grid'5000 provider implementation.
     """
 
     def init(self, config, force=False):
```

### Comparing `enos-7.1.1/enos/provider/host.py` & `enos-8.0.0a1/enos/provider/host.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/provider/openstack.py` & `enos-8.0.0a1/enos/provider/openstack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from enos.provider.provider import Provider
 from enos.utils.constants import NETWORK_INTERFACE
-from enos.utils.extra import gen_enoslib_roles
-from enoslib.service.netem.netem import expand_groups
+from enos.utils.extra import expand_groups, gen_enoslib_roles
 from enoslib.infra.enos_openstack.provider import Openstack as Enos_Openstack
 from enoslib.infra.enos_openstack.configuration import Configuration
 
 import logging
 
 
 # - SPHINX_DEFAULT_CONFIG
```

### Comparing `enos-7.1.1/enos/provider/provider.py` & `enos-8.0.0a1/enos/provider/provider.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/provider/static.py` & `enos-8.0.0a1/enos/provider/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 import copy
 import logging
 
-from enoslib.service.netem.netem import expand_groups
 import enoslib.infra.enos_static.provider as enos_static
 from enoslib.infra.enos_static.configuration import Configuration
 
 from enos.provider.provider import Provider
+from enos.utils.extra import expand_groups
 
 # - SPHINX_DEFAULT_CONFIG
 DEFAULT_CONFIG = {'type': 'static'}
 # + SPHINX_DEFAULT_CONFIG
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `enos-7.1.1/enos/provider/vmong5k.py` & `enos-8.0.0a1/enos/provider/vmong5k.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/resources/inventory.sample` & `enos-8.0.0a1/enos/resources/inventory.sample`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,22 @@
 monitoring
 
 [tls-backend:children]
 control
 
 # You can explicitly specify which hosts run each project by updating the
 # groups in the sections below. Common services are grouped together.
+
+[common:children]
+control
+network
+compute
+storage
+monitoring
+
 [chrony-server:children]
 haproxy
 
 [chrony:children]
 control
 network
 compute
@@ -62,42 +70,35 @@
 
 [prometheus:children]
 monitoring
 
 [kafka:children]
 control
 
-[karbor:children]
-control
-
 [kibana:children]
 control
 
 [telegraf:children]
 compute
 control
 monitoring
 network
 storage
 
 [elasticsearch:children]
 control
 
-[haproxy:children]
-network
+[hacluster:children]
+control
 
-[hyperv]
-#hyperv_host
+[hacluster-remote:children]
+compute
 
-[hyperv:vars]
-#ansible_user=user
-#ansible_password=password
-#ansible_port=5986
-#ansible_connection=winrm
-#ansible_winrm_server_cert_validation=ignore
+[haproxy:children]
+network
 
 [mariadb:children]
 control
 
 [rabbitmq:children]
 control
 
@@ -116,17 +117,14 @@
 
 [monasca:children]
 monitoring
 
 [storm:children]
 monitoring
 
-[mongodb:children]
-control
-
 [keystone:children]
 control
 
 [glance:children]
 control
 
 [nova:children]
@@ -172,17 +170,14 @@
 
 [ironic:children]
 control
 
 [magnum:children]
 control
 
-[qinling:children]
-control
-
 [sahara:children]
 control
 
 [mistral:children]
 control
 
 [manila:children]
@@ -194,17 +189,14 @@
 [aodh:children]
 control
 
 [cyborg:children]
 control
 compute
 
-[congress:children]
-control
-
 [panko:children]
 control
 
 [gnocchi:children]
 control
 
 [tacker:children]
@@ -228,17 +220,14 @@
 
 [watcher:children]
 control
 
 [rally:children]
 control
 
-[searchlight:children]
-control
-
 [octavia:children]
 control
 
 [designate:children]
 control
 
 [placement:children]
@@ -265,14 +254,27 @@
 # Additional control implemented here. These groups allow you to control which
 # services run on which hosts at a per-service level.
 #
 # Word of caution: Some services are required to run on the same host to
 # function appropriately. For example, neutron-metadata-agent must run on the
 # same host as the l3-agent and (depending on configuration) the dhcp-agent.
 
+# Common
+[cron:children]
+common
+
+[fluentd:children]
+common
+
+[kolla-logs:children]
+common
+
+[kolla-toolbox:children]
+common
+
 # Elasticsearch Curator
 [elasticsearch-curator:children]
 elasticsearch
 
 # Glance
 [glance-api:children]
 glance
@@ -313,14 +315,15 @@
 neutron
 
 [neutron-metadata-agent:children]
 neutron
 
 [neutron-ovn-metadata-agent:children]
 compute
+network
 
 [neutron-bgp-dragent:children]
 neutron
 
 [neutron-infoblox-ipam-agent:children]
 neutron
 
@@ -362,24 +365,14 @@
 compute
 storage
 ironic
 
 [tgtd:children]
 storage
 
-# Karbor
-[karbor-api:children]
-karbor
-
-[karbor-protection:children]
-karbor
-
-[karbor-operationengine:children]
-karbor
-
 # Manila
 [manila-api:children]
 manila
 
 [manila-scheduler:children]
 manila
 
@@ -489,21 +482,14 @@
 # Magnum
 [magnum-api:children]
 magnum
 
 [magnum-conductor:children]
 magnum
 
-# Qinling
-[qinling-api:children]
-qinling
-
-[qinling-engine:children]
-qinling
-
 # Sahara
 [sahara-api:children]
 sahara
 
 [sahara-engine:children]
 sahara
 
@@ -571,24 +557,14 @@
 
 [cyborg-agent:children]
 compute
 
 [cyborg-conductor:children]
 cyborg
 
-# Congress
-[congress-api:children]
-congress
-
-[congress-datasource:children]
-congress
-
-[congress-policy-engine:children]
-congress
-
 # Panko
 [panko-api:children]
 panko
 
 # Gnocchi
 [gnocchi-api:children]
 gnocchi
@@ -633,25 +609,21 @@
 
 [senlin-engine:children]
 senlin
 
 [senlin-health-manager:children]
 senlin
 
-# Searchlight
-[searchlight-api:children]
-searchlight
-
-[searchlight-listener:children]
-searchlight
-
 # Octavia
 [octavia-api:children]
 octavia
 
+[octavia-driver-agent:children]
+octavia
+
 [octavia-health-manager:children]
 octavia
 
 [octavia-housekeeping:children]
 octavia
 
 [octavia-worker:children]
@@ -772,15 +744,18 @@
 
 [masakari-api:children]
 control
 
 [masakari-engine:children]
 control
 
-[masakari-monitors:children]
+[masakari-hostmonitor:children]
+control
+
+[masakari-instancemonitor:children]
 compute
 
 [ovn-controller:children]
 ovn-controller-compute
 ovn-controller-network
 
 [ovn-controller-compute:children]
```

### Comparing `enos-7.1.1/enos/resources/passwords.yml` & `enos-8.0.0a1/enos/resources/passwords.yml`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,15 @@
     Q4jQ1StkzoexyHbk6g0nK6BL7zT3TAHF
 
     -----END PRIVATE KEY-----
 
     '
   public_key: ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDGbtIjUg5phfe47RO+ucoLmXyrjjuHLA8o7h92dj2JzTRyLvz9sC+9I8U98it9bQLRbye0M/2jzR7csgNHD0X3wQsUfdslvb6pIv5o9F5IWeRQUmJ+rpuC1wf3vyAIE4e02eXTjOBejDsf0ch/ZIA1Z+vUEeL19J7JMUN1MbDAURmLVP8wK41XoRiq26MNSELTXXgV88/b2untDvdZeSi0WbOMJ7Epz+uU3AWStOYgASMK0Qhmtwb4StXNH5QlgjQDiy2tRMvgcrvLbGWXRcK8As7ZRuUmJC4rIuShV0OG/cL5H62c5LWZlXhGJWmcgI+RNd7025QNo6IY88g8N7ZNMahKSTrDfX5+SDiv/l6T+qqjzkUEEEk3YlPLS1gm2mV5Xb1Atss7k3H3dELZpIobBTMOuMYT8cdRB6VCxlcZt+Ia8en+vgEDes1/BRe2TQXMlwAiEQt4jCA4uQ0yi5vLpbeujnYkh+LDnqKsItAa+Ui6Qj/S2xjKn/9zT5A0ujQI3NR5El5O3e2/SweCsSznzMsFE9QLJjZZ1t1cxpvQrDsh8QNgoRDEarjKDCM5UnDy1WRmJ17qNiF8t8ugUaNOeQM2rfmq+530qi6a3/qbQeE5m4jgwhRZO1tHbR9RiTvMENuLgBNPgd0RiNfCCwZLIoMo0I4K9X2Ojhc73lTo5Q==
 kuryr_keystone_password: demo
+libvirt_sasl_password: demo
 magnum_database_password: demo
 magnum_keystone_password: demo
 manila_database_password: demo
 manila_keystone_password: demo
 mariadb_backup_database_password: demo
 memcache_secret_key: demo
 metadata_secret: demo
```

### Comparing `enos-7.1.1/enos/resources/workload/create-and-update-image.yaml` & `enos-8.0.0a1/enos/resources/workload/create-and-update-image.yaml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/resources/workload/nova-boot-list-cc.yml` & `enos-8.0.0a1/enos/resources/workload/nova-boot-list-cc.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/resources/workload/run.yml` & `enos-8.0.0a1/enos/resources/workload/run.yml`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/services/kolla.py` & `enos-8.0.0a1/enos/services/kolla.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from typing import Any, Dict, List, Optional
 
 import enoslib as elib
 import yaml
 from ansible.plugins.loader import filter_loader as ansible_filter_loader
 from enos.utils import constants as C
 
-# Default kolla-ansible package to install (OpenStack ussuri)
-KOLLA_PKG = 'kolla-ansible~=10.0'
+# Default kolla-ansible package to install (OpenStack Wallaby)
+KOLLA_PKG = 'kolla-ansible~=12.0'
 
 # Kolla recommends installing ansible manually.  Currently 2.9 is supported.
 # Refers to the kolla-ansible User Guides for future versions. See,
 # https://docs.openstack.org/kolla-ansible/stein/user/quickstart.html#install-dependencies-not-using-a-virtual-environment
 ANSIBLE_PKG = 'ansible>=2.9,<2.10'
 
 # Current python version
@@ -341,18 +341,18 @@
         # Install kolla-ansible and its dependencies
         with elib.play_on(roles={}, pattern_hosts="localhost") as yaml:
             yaml.local_action(
                 **title(f'Install {pip_package} in {venv}'),
                 module="pip",
                 # Pin Jinja2 version to fix the renaming of `contextfilter`
                 # into `pass_context.evalcontextfilter`.
-                # See https://github.com/BeyondTheClouds/enos/pull/346#issuecomment-1080851796
+                # See https://github.com/BeyondTheClouds/enos/pull/346#issuecomment-1080851796  # noqa
                 name=[ANSIBLE_PKG, 'influxdb', 'Jinja2==3.0.3', pip_package],
                 virtualenv=str(venv),
                 virtualenv_python=PY_VERSION)
 
         return venv
 
 
 def title(title: str) -> Dict[str, str]:
     "A title for an ansible yaml commands"
-    return {"display_name": "Kolla : " + title}
+    return {"task_name": "Kolla : " + title}
```

### Comparing `enos-7.1.1/enos/services/rally.py` & `enos-8.0.0a1/enos/services/rally.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 import json
 import uuid
 import shlex
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import enoslib as elib
-import enoslib.types as elib_t
 
 # Virtual environment path for Rally on the remote machine
 VENV = '~/rally-venv'
 
 # Rally OpenStack package to install with pip
 PKG = 'rally-openstack~=2.1.0'
 
 
 class RallyOpenStack():
     # Resources with agents that have Rally
-    rsc: elib_t.Roles
+    rsc: elib.Roles
 
     # Name of the rally deployment
     name: str
 
     # Tracker of done Rally tasks [(scenario name, {hostname: Rally-uuid})]
     _tasks: List[Tuple[str, Dict[str, str]]]
 
     def __init__(self,
-                 agents: List[elib_t.Host],
+                 agents: List[elib.Host],
                  environment_name: str = 'enos'):
         """Deploy Rally OpenStack on a list of agents.
 
         Args:
           agents: The list of agents to deploy Rally OpenStack on.
           environment_name: Name of this rally environment.
 
@@ -41,15 +40,15 @@
         """
         self.rsc = {'all': agents}
         self.env_name = environment_name
 
         RallyOpenStack.pull(agents)
 
     @staticmethod
-    def pull(agents: List[elib_t.Host]):
+    def pull(agents: List[elib.Host]):
         'Installs Rally OpenStack'
         logging.info("Pull: installing rally in a virtual environment")
 
         with elib.play_on(roles={'all': agents},
                           priors=[elib.api.__python3__],
                           gather_facts=False) as yaml:
             yaml.pip(**title(f'install virtualenv {VENV}'), name='virtualenv')
@@ -209,8 +208,8 @@
             return False
         else:
             return True
 
 
 def title(title: str) -> Dict[str, str]:
     "A title for ansible yaml commands"
-    return {"display_name": "Rally : " + title}
+    return {"task_name": "Rally : " + title}
```

### Comparing `enos-7.1.1/enos/services/shaker.py` & `enos-8.0.0a1/enos/services/shaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,44 @@
 "Installs and run Shaker on a list of agents"
 import logging
 import uuid
 from pathlib import Path
 from typing import Dict, List
 
 import enoslib as elib
-import enoslib.types as elib_t
 
 # Docker image for Shaker
 IMG = 'performa/shaker:latest'
 
 
 class Shaker():
     # Resources with agents that have Shaker
-    rsc: elib_t.Roles
+    rsc: elib.Roles
 
     # Directory that is mount in the docker as Shaker home
     home: str
 
     # Authentication variables for OpenStack (as in openrc)
     _openstack_auth: Dict[str, str] = {}
 
-    def __init__(self, agents: List[elib_t.Host]):
+    def __init__(self, agents: List[elib.Host]):
         """Deploy Shaker OpenStack on a list of agents.
 
         Args:
           agents: The list of agents to deploy Shaker OpenStack on.
 
         Reference:
           https://opendev.org/performa/shaker
         """
         self.rsc = {'all': agents}
         self.home = "~/shaker_home_" + str(uuid.uuid4())
         Shaker.pull(agents)
 
     @staticmethod
-    def pull(agents: List[elib_t.Host]):
+    def pull(agents: List[elib.Host]):
         'Pulling the docker image of Shaker '
         logging.info("Pull: get docker image for Shaker")
 
         with elib.play_on(roles={'all': agents},
                           gather_facts=False) as yaml:
             yaml.docker_image(
                 **title(f'pulling docker image {IMG}'),
@@ -103,8 +102,8 @@
 
     def destroy(self):
         pass
 
 
 def title(title: str) -> Dict[str, str]:
     "A title for an ansible yaml commands"
-    return {"display_name": "Shaker : " + title}
+    return {"task_name": "Shaker : " + title}
```

### Comparing `enos-7.1.1/enos/tasks/__init__.py` & `enos-8.0.0a1/enos/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/tasks/new.py` & `enos-8.0.0a1/enos/tasks/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     resources_conf = None
     registry_conf = None
 
     # Refine options based on the provider
     if provider == 'g5k':
         resources_conf = G5K_RSC
         registry_conf = G5K_EXTERNAL_REG
-        provider_required_keys += ['walltime', 'job_name']
+        provider_required_keys += ['job_name', 'job_type', 'env_name', 'walltime'] # noqa
     elif provider == 'vagrant':
         provider_conf.update(backend=backend)
         resources_conf = VAGRANT_RSC
         registry_conf = INTERNAL_REG
         provider_required_keys.append('backend')
     elif provider == 'chameleonkvm':
         provider_conf.update(
@@ -135,15 +135,15 @@
             image='<set a Glance image (see `openstack image list`)>')
         registry_conf = INTERNAL_REG
         resources_conf = OS_RSC
         provider_required_keys += ['user', 'key_name', 'image']
     elif provider == 'vmong5k':
         resources_conf = VMONG5K_RSC
         registry_conf = INTERNAL_REG
-        provider_required_keys += ['walltime', 'job_name']
+        provider_required_keys += ['walltime', 'job_name', 'env_name']
     elif provider == 'static':
         resources_conf = STATIC_RSC
         registry_conf = INTERNAL_REG
 
     LOGGER.debug(f'Generating {output_path} file with '
                  f'provider conf {provider_conf}, '
                  f'registry conf {registry_conf}, and '
```

### Comparing `enos-7.1.1/enos/tasks/up.py` & `enos-8.0.0a1/enos/tasks/up.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 import logging
 import os
 from pathlib import Path
 from operator import methodcaller
 
 import enoslib as elib
 import enoslib.api as elib_api
-import enoslib.types as elib_t
 from enoslib.enos_inventory import EnosInventory
 
 from enos.services import KollaAnsible
 import enos.utils.constants as C
-from enos.utils.extra import (generate_inventory,
-                              get_vip_pool, make_provider, pop_ip, seekpath)
+from enos.utils.extra import (generate_inventory, get_vip_pool,
+                              make_provider, ip_generator, seekpath)
 
 from typing import Optional, Dict, Any
 
 LOGGER = logging.getLogger(__name__)
 
 
 def up(env: elib.Environment,
@@ -57,56 +56,67 @@
     provider_conf = dict(provider.default_config(), **config['provider'])
     config.update(provider=provider_conf)
     LOGGER.debug(f"Loaded config {config}")
     env['config'] = config
 
     # Call the provider to initialize resources
     rsc, networks = provider.init(config, is_force_deploy)
+    # Note(rcherrueau): I keep track of this extra information for a
+    # futur migration to enoslib-v6:
+    # > enos-0 ansible_host=192.168.121.128 ansible_port='22'
+    # > ansible_ssh_common_args='-o StrictHostKeyChecking=no -o
+    # > UserKnownHostsFile=/dev/null'
+    # > ansible_ssh_private_key_file='/home/rfish/prog/enos/.vagrant/machines/enos-0/libvirt/private_key' # noqa
+    # > ansible_ssh_user='root' enos_devices="['eth1','eth2']"
+    # > network_interface='eth1' network_interface_dev='eth1'
+    # > network_interface_ip='192.168.42.245'
+    # > neutron_external_interface='eth2'
+    # > neutron_external_interface_dev='eth2'
+    # > neutron_external_interface_ip='192.168.43.245'
+    rsc = elib.sync_info(rsc, networks)
     LOGGER.debug(f"Provider resources: {rsc}")
     LOGGER.debug(f"Provider network information: {networks}")
 
+    # Configure node-specific variables such as "network_interface".
+    # Enoslib will then include these variables in the inventory so that
+    # Kolla will be able to use them.
+    for host in rsc.all():
+        for network_name in [C.NETWORK_INTERFACE, C.API_INTERFACE,
+                             C.NEUTRON_EXTERNAL_INTERFACE]:
+            if networks[network_name]:
+                physical_interfaces = host.filter_interfaces(networks[network_name]) # noqa
+                if physical_interfaces:
+                    host.set_extra(**{network_name: physical_interfaces[0]})
+
     # Generates inventory for ansible/kolla
     inventory = os.path.join(str(env.env_name), 'multinode')
     inventory_conf = env['config'].get('inventory')
     if not inventory_conf:
         LOGGER.debug("No inventory specified, using the sample.")
         base_inventory = os.path.join(C.RSCS_DIR, 'inventory.sample')
     else:
         base_inventory = seekpath(inventory_conf)
     generate_inventory(rsc, networks, base_inventory, inventory)
     LOGGER.info('Generates inventory %s' % inventory)
     env['inventory'] = inventory
 
-    # Fills rsc with information such as network_interface and then
-    # ensures rsc contains all groups defined by the inventory (e.g.,
+    # Ensures rsc contains all groups defined by the inventory (e.g.,
     # 'enos/registry', 'enos/influx', 'haproxy', ...).
     #
-    # Note(rcherrueau): I keep track of this extra information for a
-    # futur migration to enoslib-v6:
-    # > enos-0 ansible_host=192.168.121.128 ansible_port='22'
-    # > ansible_ssh_common_args='-o StrictHostKeyChecking=no -o
-    # > UserKnownHostsFile=/dev/null'
-    # > ansible_ssh_private_key_file='/home/rfish/prog/enos/.vagrant/machines/enos-0/libvirt/private_key' # noqa
-    # > ansible_ssh_user='root' enos_devices="['eth1','eth2']"
-    # > network_interface='eth1' network_interface_dev='eth1'
-    # > network_interface_ip='192.168.42.245'
-    # > neutron_external_interface='eth2'
-    # > neutron_external_interface_dev='eth2'
-    # > neutron_external_interface_ip='192.168.43.245'
-    rsc = elib.discover_networks(rsc, networks)
     rsc = build_rsc_with_inventory(rsc, env['inventory'])
     env['rsc'] = rsc
     env['networks'] = networks
 
     # Get variables required by the application
     vip_pool = get_vip_pool(networks)
+    ips = ip_generator(vip_pool)
     env['config'].update({
-        'vip':               pop_ip(vip_pool),
-        'influx_vip':        pop_ip(vip_pool),
-        'grafana_vip':       pop_ip(vip_pool),
+        'vip':               next(ips),
+        'influx_vip':        next(ips),
+        'grafana_vip':       next(ips),
         'resultdir':         str(env.env_name),
         'rabbitmq_password': "demo",
         'database_password': "demo",
         'cwd':               str(Path.cwd()),
     })
 
     # Ensure python3 is on remote targets (kolla requirement)
@@ -143,15 +153,17 @@
 
     # Install kolla-ansible and run bootstrap-servers
     kolla_globals_values = {
         'kolla_internal_vip_address': env['config']['vip'],
         'influx_vip': env['config']['influx_vip'],
         'resultdir': str(env.env_name),
         'docker_custom_config': mk_kolla_docker_custom_config(docker),
-        'cwd':  os.getcwd()
+        'docker_disable_default_iptables_rules': False,
+        'docker_disable_default_network': False,
+        'cwd': os.getcwd()
     }
     kolla_globals_values.update(env['config'].get('kolla', {}))
     kolla_ansible = KollaAnsible(
         config_dir=env.env_name,
         inventory_path=inventory,
         pip_package=env['config'].get('kolla-ansible'),
         globals_values=kolla_globals_values)
@@ -175,14 +187,15 @@
         for k, v in os_auth_rc.items():
             admin_openrc.write(f'export {k}="{v}"\n')
 
     LOGGER.debug(f"{admin_openrc_path} generated with {os_auth_rc}")
 
     # Set up machines with bare dependencies
     with elib.play_on(inventory_path=inventory, pattern_hosts='baremetal',
+                      gather_facts=True,
                       extra_vars=kolla_ansible.globals_values) as yml:
         # Remove IP on the external interface if any
         yml.shell(
             "ip addr flush {{ neutron_external_interface }}",
             **title('Remove IP on the external interface (if any)'),
             when="neutron_external_interface is defined")
 
@@ -196,15 +209,15 @@
             **title('Install the bare necessities (pip)'),
             name=['docker', 'influxdb'],
             executable='pip3')
 
         # nscd prevents kolla-toolbox to start. See,
         # https://bugs.launchpad.net/kolla-ansible/+bug/1680139
         yml.systemd(
-            **title('Install the bare necessities (pip)'),
+            **title('Stop nscd to prevent kolla-toolbox error'),
             name='nscd', state='stopped', ignore_errors=True)
 
         # Break RabbitMQ, which expects the hostname to resolve to the
         # API network address.  Remove the troublesome entry.  See
         # https://bugs.launchpad.net/kolla-ansible/+bug/1837699 and
         # https://bugs.launchpad.net/kolla-ansible/+bug/1862739
         for banned_ip in ['127.0.1.1', '127.0.2.1']:
@@ -232,15 +245,15 @@
 
 
 # Utils
 
 def title(title: str) -> Dict[str, str]:
     "A title for an ansible yaml commands"
 
-    return {"display_name": "enos up : " + title}
+    return {"task_name": "enos up : " + title}
 
 
 def mk_kolla_docker_custom_config(docker: elib.Docker) -> Dict[str, Any]:
     '''Docker daemon conf for kolla-ansible that reflects elib.Docker
 
     Kolla-ansible overwrites the Docker daemon configuration that is setup by
     enoslib.  This function makes a specific Docker custom config for
@@ -261,15 +274,15 @@
             'insecure-registries': [mirror],
         })
 
     return docker_custom_config
 
 
 def build_rsc_with_inventory(
-        rsc: elib_t.Roles, inventory_path: str) -> elib_t.Roles:
+        rsc: elib.Roles, inventory_path: str) -> elib.Roles:
     '''Return a new `rsc` with roles from the inventory.
 
     In enos, we have a strong binding between enoslib roles and kolla-ansible
     groups.  We need for instance to know hosts of the 'enos/registry' group.
     This method takes an enoslib Roles object and an inventory_path and returns
     a new Roles object that contains all groups (as in the inventory file) with
     their hosts (as in enoslib).
```

### Comparing `enos-7.1.1/enos/templates/Vagrantfile.j2` & `enos-8.0.0a1/enos/templates/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/templates/grafana_dashboard.json` & `enos-8.0.0a1/enos/templates/grafana_dashboard.json`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/templates/reservation.yaml.j2` & `enos-8.0.0a1/enos/templates/reservation.yaml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # enable_monitoring: no
 
 
 # kolla-ansible executable (could be a PyPi package, a git
 # repository, a local directory ...)
 # See https://beyondtheclouds.github.io/enos/customization/index.html#changing-kolla-version
 #
-# kolla-ansible: {{ kolla_ansible }}
+kolla-ansible: {{ kolla_ansible }}
 
 
 # Custom kolla-ansible parameters (as in `globals.yml`)
 # See https://beyondtheclouds.github.io/enos/customization/index.html#customize-kolla-variables
 #
 # kolla:
 #   kolla_base_distro: "centos"
```

### Comparing `enos-7.1.1/enos/utils/build.py` & `enos-8.0.0a1/enos/utils/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     'inventory': 'inventories/inventory.sample',
     'kolla': {
         'enable_heat': 'yes',
         'kolla_base_distro': '{{ base }}',
         'kolla_install_type': '{{ distribution }}',
         'nova_compute_virt_type': 'qemu'
     },
-    'kolla_ref': 'stable/rocky',
-    'kolla_repo': 'https://git.openstack.org/openstack/kolla-ansible',
     'registry': {
         'type': 'internal'
     },
     'working_dir': '{{ directory }}',
     'strategy': 'copy'
 }
```

### Comparing `enos-7.1.1/enos/utils/cli.py` & `enos-8.0.0a1/enos/utils/cli.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/utils/constants.py` & `enos-8.0.0a1/enos/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 # fake interface a give it the neutron_external_interface role
 NEUTRON_EXTERNAL_INTERFACE = 'neutron_external_interface'
 
 # In case we need to create a fake interface, this will be the nic name.
 FAKE_NEUTRON_EXTERNAL_INTERFACE = 'nei'
 
 # ENOS Setup
-VERSION = '7.1.1'
+VERSION = '8.0.0a1'
```

### Comparing `enos-7.1.1/enos/utils/errors.py` & `enos-8.0.0a1/enos/utils/errors.py`

 * *Files identical despite different names*

### Comparing `enos-7.1.1/enos/utils/extra.py` & `enos-8.0.0a1/enos/utils/extra.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import importlib
 import logging
 import os
-from typing import Dict, Union, Any, Callable
+import re
+from typing import Dict, Union, Any, Callable, Iterable
 
 from enos.provider.provider import Provider
 import enos.utils.constants as C
 from enos.utils.errors import (EnosFilePathError,
                                EnosUnknownProvider,
                                MissingEnvState)
 import enoslib as elib
 import enoslib.api as elib_api
-from netaddr import IPRange
 
 # These roles are mandatory for the
 # the original inventory to be valid
 # Note that they may be empty
 # e.g. if cinder isn't installed storage may be a empty group
 # in the inventory
 KOLLA_MANDATORY_GROUPS = [
@@ -29,33 +29,24 @@
 def generate_inventory(roles, networks, base_inventory, dest):
     """
     Generate the inventory.
     It will generate a group for each role in roles and
     concatenate them with the base_inventory file.
     The generated inventory is written in dest
     """
-    # NOTE(msimonin): if len(networks) is <= 1
-    # provision a fake one that will map the external network
-
-    fake_interfaces = []
-    fake_networks = []
     provider_net = lookup_network(networks, [C.NEUTRON_EXTERNAL_INTERFACE])
     if not provider_net:
-        logging.error(f"The {C.NEUTRON_EXTERNAL_INTERFACE} network is missing")
-        logging.error("EnOS will try to fix that ....")
-        fake_interfaces = [C.FAKE_NEUTRON_EXTERNAL_INTERFACE]
-        fake_networks = [C.NEUTRON_EXTERNAL_INTERFACE]
+        msg = f"The {C.NEUTRON_EXTERNAL_INTERFACE} network is missing"
+        raise ValueError(msg)
 
     elib_api.generate_inventory(
         roles,
         networks,
         dest,
-        check_networks=True,
-        fake_interfaces=fake_interfaces,
-        fake_networks=fake_networks)
+        check_networks=False)
 
     with open(dest, 'a') as f:
         f.write("\n")
         # generate mandatory groups that are empty
         mandatory = [group for group in KOLLA_MANDATORY_GROUPS
                      if group not in roles.keys()]
         for group in mandatory:
@@ -69,17 +60,16 @@
 
 
 def lookup_network(networks, roles):
     """Lookup a network by its roles (in order).
     We assume that one role can't be found in two different networks
     """
     for role in roles:
-        for network in networks:
-            if role in network["roles"]:
-                return network
+        if networks[role]:
+            return networks[role][0]
     return None
 
 
 def get_vip_pool(networks):
     """Get the provider net where vip can be taken.
     In kolla-ansible this is the network with the api_interface role.
     In kolla-ansible api_interface defaults to network_interface.
@@ -90,38 +80,20 @@
         return provider_net
 
     msg = "You must declare %s" % " or ".join(
         [C.API_INTERFACE, C.NETWORK_INTERFACE])
     raise Exception(msg)
 
 
-def pop_ip(provider_net):
-    """Picks an ip from the provider_net
-    It will first take ips in the extra_ips if possible.
-    extra_ips is a list of isolated ips whereas ips described
-    by the [provider_net.start, provider.end] range is a continuous
-    list of ips.
-    """
-    # Construct the pool of ips
-    extra_ips = provider_net.get('extra_ips', [])
-    if len(extra_ips) > 0:
-        ip = extra_ips.pop()
-        provider_net['extra_ips'] = extra_ips
-        return ip
-
-    ips = list(IPRange(provider_net['start'],
-                       provider_net['end']))
-
-    # Get the next ip
-    ip = str(ips.pop())
-
-    # Remove this ip from the env
-    provider_net['end'] = str(ips.pop())
-
-    return ip
+def ip_generator(provider_net) -> Iterable[str]:
+    """Iterator that picks successive IP addresses from the provider_net.
+    """
+    # This is an iterator that returns ipaddress.IPv4Address objects
+    for ip in provider_net.free_ips:
+        yield str(ip)
 
 
 def make_provider(provider_conf: Union[str, Dict[str, Any]]) -> Provider:
     """Instantiates the provider.
 
     Seeks into the configuration for the `provider` value. The value
     SHOULD be, either a *string*, or a *dictionary with a `type` key*
@@ -163,14 +135,39 @@
                 # Puts the resources in a default topology group
                 yield {"group": "default_group",
                        "role": k2,
                        "flavor": k1,
                        "number": v2}
 
 
+def expand_groups(grp):
+    """Expand group names.
+
+     Args:
+        grp (string): group names to expand
+
+    Returns:
+        list of groups
+
+    Examples:
+
+        * grp[1-3] will be expanded to [grp1, grp2, grp3]
+        * grp1 will be expanded to [grp1]
+    """
+    p = re.compile(r"(?P<name>.+)\[(?P<start>\d+)-(?P<end>\d+)\]")
+    m = p.match(grp)
+    if m is not None:
+        s = int(m.group("start"))
+        e = int(m.group("end"))
+        n = m.group("name")
+        return list(map(lambda x: n + str(x), range(s, e + 1)))
+    else:
+        return [grp]
+
+
 def seekpath(path):
     """Seek for an enos file `path` and returns its absolute counterpart.
 
     Seeking rules are:
     - If `path` is absolute then return it
     - Otherwise, look for `path` in the current working directory
     - Otherwise, look for `path` in the resources directory
```

### Comparing `enos-7.1.1/pyproject.toml` & `enos-8.0.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 [tool.poetry]
 name = "enos"
-version = "7.1.1"
+version = "8.0.0a1"
 description = "Experimental eNvironment for OpenStack"
 authors = ["Didier Iscovery <discovery-dev@inria.fr>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/BeyondTheClouds/enos"
 documentation = "https://beyondtheclouds.github.io/enos/"
 keywords = ["OpenStack", "Evaluation", "Grid'5000", "Chameleon", "Vagrant"]
 classifiers = [
   'Development Status :: 4 - Beta',
   'Intended Audience :: System Administrators',
   'Intended Audience :: Science/Research',
   'Operating System :: POSIX :: Linux',
-  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
+  'Programming Language :: Python :: 3.10',
+  'Programming Language :: Python :: 3.11',
 ]
 include = [
   'README.rst',
   'LICENSE',
   'enos/ansible/**/*',
   'enos/ansible.cfg',
   'enos/provider/openstack.sh',
   'enos/resources/**/*',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-enoslib = { version = "~5.6", extras = [ "chameleon" ] }
+python = "^3.8"
 # enoslib = { path = '../enoslib', develop = true, extras = [ "chameleon" ]  }
+enoslib = { version = "^8.1.2", extras = [ "chameleon" ] }
+# Our ansible_filter_loader hack (to load Jinja context filters from Kolla)
+# no longer works with recent versions of Ansible, so let's stick to 2.9 for now.
+ansible = { version = "~2.9" }
 docopt = ">=0.6.2,<0.7.0"
 virtualenv = "^20.4.3"
-python-openstackclient = "^5.5.0"
-python-heatclient = "^2.3.0"
+python-openstackclient = "^6.0.0"
+python-heatclient = "^2.5.0"
 influxdb = { version = "4.0.0", optional = true }
 
 [tool.poetry.extras]
 # poetry install -E annotations
 annotations = ["influxdb"]
 
 [tool.poetry.scripts]
```

### Comparing `enos-7.1.1/PKG-INFO` & `enos-8.0.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: enos
-Version: 7.1.1
+Version: 8.0.0a1
 Summary: Experimental eNvironment for OpenStack
 Home-page: https://github.com/BeyondTheClouds/enos
 License: GPL-3.0-or-later
 Keywords: OpenStack,Evaluation,Grid'5000,Chameleon,Vagrant
 Author: Didier Iscovery
 Author-email: discovery-dev@inria.fr
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: annotations
+Requires-Dist: ansible (>=2.9,<2.10)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: enoslib[chameleon] (>=5.6,<5.7)
-Requires-Dist: influxdb (==4.0.0); extra == "annotations"
-Requires-Dist: python-heatclient (>=2.3.0,<3.0.0)
-Requires-Dist: python-openstackclient (>=5.5.0,<6.0.0)
+Requires-Dist: enoslib[chameleon] (>=8.1.2,<9.0.0)
+Requires-Dist: influxdb (==4.0.0) ; extra == "annotations"
+Requires-Dist: python-heatclient (>=2.5.0,<3.0.0)
+Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0)
 Requires-Dist: virtualenv (>=20.4.3,<21.0.0)
 Project-URL: Documentation, https://beyondtheclouds.github.io/enos/
 Description-Content-Type: text/x-rst
 
-|Build Status| |Doc Status| |Pypi| |Code style| |License|
+|Doc Status| |Pypi| |Code style| |License|
 
 Join us on gitter :  |Join the chat at
 https://gitter.im/BeyondTheClouds/enos|
 
 About Enos
 ==========
 
@@ -95,16 +100,14 @@
 Links
 =====
 
 -  Docs - https://beyondtheclouds.github.io/enos/
 -  Discovery - https://beyondtheclouds.github.io/
 -  Docker - https://hub.docker.com/r/beyondtheclouds/
 
-.. |Build Status| image:: https://travis-ci.org/BeyondTheClouds/enos.svg?branch=master
-   :target: https://travis-ci.org/BeyondTheClouds/enos
 .. |Join the chat at https://gitter.im/BeyondTheClouds/enos| image:: https://badges.gitter.im/BeyondTheClouds/enos.svg
    :target: https://gitter.im/BeyondTheClouds/enos?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
 .. |Code style| image:: https://api.codacy.com/project/badge/Grade/87536e9c0f0d47e08d1b9e0950c9d14b
    :target: https://www.codacy.com/app/msimonin/enos?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=BeyondTheClouds/enos&amp;utm_campaign=Badge_Grade
 .. |License| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
 .. |Pypi| image:: https://badge.fury.io/py/enos.svg
```


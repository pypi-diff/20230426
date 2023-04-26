# Comparing `tmp/ifrappe_bench-5.16.5.tar.gz` & `tmp/ifrappe_bench-5.16.6.tar.gz`

## Comparing `ifrappe_bench-5.16.5.tar` & `ifrappe_bench-5.16.6.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/__init__.pyr
--rwxr-xr-x   0        0        0    20065 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/app.py
--rw-r--r--   0        0        0    13384 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/bench.py
--rwxr-xr-x   0        0        0     5807 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/cli.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/exceptions.py
--rwxr-xr-x   0        0        0     2897 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/config.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/git.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/install.py
--rwxr-xr-x   0        0        0     6221 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/make.py
--rwxr-xr-x   0        0        0    12647 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/setup.py
--rwxr-xr-x   0        0        0     2824 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/update.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/commands/utils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/__init__.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/common_site_config.py
--rwxr-xr-x   0        0        0     5423 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/lets_encrypt.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/nginx.py
--rwxr-xr-x   0        0        0      885 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/procfile.py
--rwxr-xr-x   0        0        0     5574 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/production_setup.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/redis.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/site_config.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/supervisor.py
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/systemd.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/502.html
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/Procfile
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/bench_manager_nginx.conf
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/frappe_sudoers
--rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/letsencrypt.cfg
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/nginx.conf
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/nginx_default.conf
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/redis_cache.conf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/redis_queue.conf
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/redis_socketio.conf
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/supervisor.conf
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-schedule.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-web.service
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-node-socketio.service
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-redis-cache.service
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-redis-queue.service
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-redis-socketio.service
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-redis.target
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-web.target
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-workers.target
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench.target
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/patches.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/v5/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/v5/fix_backup_cronjob.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/v5/fix_user_permissions.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/v5/set_live_reload_config.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/patches/v5/update_archived_sites.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/create_user.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/macosx.yml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/site.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/vm_build.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bash_screen_wall/tasks/main.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/change_ssh_port.yml
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/main.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_bench_production.yml
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_erpnext.yml
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_firewall.yml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_inputrc.yml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/debian.yml
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/debian_family.yml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/macos.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/main.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/redhat_family.yml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/ubuntu.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/dns_caching/handlers/main.yml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/dns_caching/tasks/main.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/defaults/main.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/handlers/main.yml
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/tasks/main.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/frappe_selinux/tasks/main.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/locale/defaults/main.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/locale/tasks/main.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/logwatch/defaults/main.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/logwatch/tasks/main.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/README.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/defaults/main.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/files/mariadb_config.cnf
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/handlers/main.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/centos.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/debian.yml
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/main.yml
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/templates/my.cnf.j2
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/vars/main.yml
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/README.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/defaults/main.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/handlers/main.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/meta/main.yml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/main.yml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/setup-Debian.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/vhosts.yml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/templates/nginx.conf.j2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/templates/nginx.repo.j2
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/templates/vhosts.j2
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tests/inventory
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tests/test.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/vars/Debian.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/vars/RedHat.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nodejs/defaults/main.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nodejs/tasks/debian_family.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nodejs/tasks/main.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/nodejs/tasks/redhat_family.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/ntpd/tasks/main.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/packer/tasks/debian_family.yml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/packer/tasks/main.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/packer/tasks/redhat_family.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/psutil/tasks/main.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/redis/tasks/main.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/supervisor/tasks/main.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/swap/defaults/main.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/swap/tasks/main.yml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/defaults/main.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/tasks/debian_family.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/tasks/main.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/tests/__init__.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/tests/test_base.py
--rwxr-xr-x   0        0        0     6695 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/tests/test_init.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/tests/test_setup_production.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/tests/test_utils.py
--rw-r--r--   0        0        0    13783 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/__init__.py
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/app.py
--rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/bench.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/cli.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/render.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/system.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/bench/utils/translation.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/.gitignore
--rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/LICENSE
--rwxr-xr-x   0        0        0    11041 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/README.md
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/pyproject.toml
--rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.5/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/__init__.pyr
+-rwxr-xr-x   0        0        0    20065 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/app.py
+-rw-r--r--   0        0        0    13384 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/bench.py
+-rwxr-xr-x   0        0        0     5807 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/cli.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/exceptions.py
+-rwxr-xr-x   0        0        0     2897 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/__init__.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/config.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/git.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/install.py
+-rwxr-xr-x   0        0        0     6221 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/make.py
+-rwxr-xr-x   0        0        0    12647 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/setup.py
+-rwxr-xr-x   0        0        0     2824 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/update.py
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/commands/utils.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/__init__.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/common_site_config.py
+-rwxr-xr-x   0        0        0     5423 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/lets_encrypt.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/nginx.py
+-rwxr-xr-x   0        0        0      885 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/procfile.py
+-rwxr-xr-x   0        0        0     5574 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/production_setup.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/redis.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/site_config.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/supervisor.py
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/systemd.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/502.html
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/Procfile
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/bench_manager_nginx.conf
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/frappe_sudoers
+-rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/letsencrypt.cfg
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/nginx.conf
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/nginx_default.conf
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/redis_cache.conf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/redis_queue.conf
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/redis_socketio.conf
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/supervisor.conf
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-schedule.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-web.service
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-node-socketio.service
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-redis-cache.service
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-redis-queue.service
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-redis-socketio.service
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-redis.target
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-web.target
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-workers.target
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench.target
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/patches.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/v5/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/v5/fix_backup_cronjob.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/v5/fix_user_permissions.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/v5/set_live_reload_config.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/patches/v5/update_archived_sites.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/create_user.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/macosx.yml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/site.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/vm_build.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bash_screen_wall/tasks/main.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/change_ssh_port.yml
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/main.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_bench_production.yml
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_erpnext.yml
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_firewall.yml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_inputrc.yml
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/debian.yml
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/debian_family.yml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/macos.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/main.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/ubuntu.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/dns_caching/handlers/main.yml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/dns_caching/tasks/main.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/defaults/main.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/handlers/main.yml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/tasks/main.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/frappe_selinux/tasks/main.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/locale/defaults/main.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/locale/tasks/main.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/logwatch/defaults/main.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/logwatch/tasks/main.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/README.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/defaults/main.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/files/mariadb_config.cnf
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/handlers/main.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/centos.yml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/debian.yml
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/main.yml
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/templates/my.cnf.j2
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/vars/main.yml
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/defaults/main.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/handlers/main.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/meta/main.yml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/main.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/setup-Debian.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/vhosts.yml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/templates/nginx.conf.j2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/templates/nginx.repo.j2
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/templates/vhosts.j2
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tests/inventory
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tests/test.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/vars/Debian.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/vars/RedHat.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nodejs/defaults/main.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nodejs/tasks/debian_family.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nodejs/tasks/main.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/nodejs/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/ntpd/tasks/main.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/packer/tasks/debian_family.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/packer/tasks/main.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/packer/tasks/redhat_family.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/psutil/tasks/main.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/redis/tasks/main.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/supervisor/tasks/main.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/swap/defaults/main.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/swap/tasks/main.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/defaults/main.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/tasks/debian_family.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/tasks/main.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/tests/__init__.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/tests/test_base.py
+-rwxr-xr-x   0        0        0     6695 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/tests/test_init.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/tests/test_setup_production.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/tests/test_utils.py
+-rw-r--r--   0        0        0    13783 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/__init__.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/app.py
+-rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/bench.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/cli.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/render.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/system.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/bench/utils/translation.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/.gitignore
+-rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/LICENSE
+-rwxr-xr-x   0        0        0    11041 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/README.md
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/pyproject.toml
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 ifrappe_bench-5.16.6/PKG-INFO
```

### Comparing `ifrappe_bench-5.16.5/bench/app.py` & `ifrappe_bench-5.16.6/bench/app.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/bench.py` & `ifrappe_bench-5.16.6/bench/bench.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/cli.py` & `ifrappe_bench-5.16.6/bench/cli.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/exceptions.py` & `ifrappe_bench-5.16.6/bench/exceptions.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/__init__.py` & `ifrappe_bench-5.16.6/bench/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/config.py` & `ifrappe_bench-5.16.6/bench/commands/config.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/git.py` & `ifrappe_bench-5.16.6/bench/commands/git.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/install.py` & `ifrappe_bench-5.16.6/bench/commands/install.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/make.py` & `ifrappe_bench-5.16.6/bench/commands/make.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/setup.py` & `ifrappe_bench-5.16.6/bench/commands/setup.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/update.py` & `ifrappe_bench-5.16.6/bench/commands/update.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/commands/utils.py` & `ifrappe_bench-5.16.6/bench/commands/utils.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/common_site_config.py` & `ifrappe_bench-5.16.6/bench/config/common_site_config.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/lets_encrypt.py` & `ifrappe_bench-5.16.6/bench/config/lets_encrypt.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/nginx.py` & `ifrappe_bench-5.16.6/bench/config/nginx.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/procfile.py` & `ifrappe_bench-5.16.6/bench/config/procfile.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/production_setup.py` & `ifrappe_bench-5.16.6/bench/config/production_setup.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/redis.py` & `ifrappe_bench-5.16.6/bench/config/redis.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/site_config.py` & `ifrappe_bench-5.16.6/bench/config/site_config.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/supervisor.py` & `ifrappe_bench-5.16.6/bench/config/supervisor.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/systemd.py` & `ifrappe_bench-5.16.6/bench/config/systemd.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/502.html` & `ifrappe_bench-5.16.6/bench/config/templates/502.html`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/Procfile` & `ifrappe_bench-5.16.6/bench/config/templates/Procfile`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/bench_manager_nginx.conf` & `ifrappe_bench-5.16.6/bench/config/templates/bench_manager_nginx.conf`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/letsencrypt.cfg` & `ifrappe_bench-5.16.6/bench/config/templates/letsencrypt.cfg`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/nginx.conf` & `ifrappe_bench-5.16.6/bench/config/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/nginx_default.conf` & `ifrappe_bench-5.16.6/bench/config/templates/nginx_default.conf`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/supervisor.conf` & `ifrappe_bench-5.16.6/bench/config/templates/supervisor.conf`

 * *Files 9% similar despite different names*

```diff
@@ -178,20 +178,20 @@
 
 [group:{{ bench_name }}-web]
 programs={{ bench_name }}-frappe-web {%- if node -%} ,{{ bench_name }}-node-socketio {%- endif%}
 
 {% if use_rq %}
 
 [group:{{ bench_name }}-workers]
-programs={{ bench_name }}-frappe-schedule,{{ bench_name }}-frappe-default-worker,{{ bench_name }}-frappe-short-worker,{{ bench_name }}-frappe-long-worker{%- for worker_name in workers -%},{{ bench_name }}-frappe-{{ worker_name }}-worker{%- endfor %}
+programs={{ bench_name }}-frappe-schedule,{{ bench_name }}-frappe-default-worker,{{ bench_name }}-frappe-short-worker,{{ bench_name }}-frappe-long-worker
 
 {% else %}
 
 [group:{{ bench_name }}-workers]
-programs={{ bench_name }}-frappe-workerbeat,{{ bench_name }}-frappe-worker,{{ bench_name }}-frappe-longjob-worker,{{ bench_name }}-frappe-async-worker{%- for worker_name in workers -%},{{ bench_name }}-frappe-{{ worker_name }}-worker{%- endfor %}
+programs={{ bench_name }}-frappe-workerbeat,{{ bench_name }}-frappe-worker,{{ bench_name }}-frappe-longjob-worker,{{ bench_name }}-frappe-async-worker
 
 {% endif %}
 
 {% if not skip_redis %}
 [group:{{ bench_name }}-redis]
 programs={{ bench_name }}-redis-cache,{{ bench_name }}-redis-queue,{{ bench_name }}-redis-socketio
 {% endif %}
```

### Comparing `ifrappe_bench-5.16.5/bench/config/templates/systemd/frappe-bench-frappe-web.service` & `ifrappe_bench-5.16.6/bench/config/templates/systemd/frappe-bench-frappe-web.service`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/patches/__init__.py` & `ifrappe_bench-5.16.6/bench/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/patches/v5/fix_user_permissions.py` & `ifrappe_bench-5.16.6/bench/patches/v5/fix_user_permissions.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/patches/v5/update_archived_sites.py` & `ifrappe_bench-5.16.6/bench/patches/v5/update_archived_sites.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/create_user.yml` & `ifrappe_bench-5.16.6/bench/playbooks/create_user.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/macosx.yml` & `ifrappe_bench-5.16.6/bench/playbooks/macosx.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/site.yml` & `ifrappe_bench-5.16.6/bench/playbooks/site.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_bench_production.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_bench_production.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_erpnext.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_erpnext.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/bench/tasks/setup_firewall.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/bench/tasks/setup_firewall.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/debian.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/debian_family.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/macos.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/macos.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/redhat_family.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/redhat_family.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/common/tasks/ubuntu.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/common/tasks/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2` & `ifrappe_bench-5.16.6/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te` & `ifrappe_bench-5.16.6/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/frappe_selinux/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/frappe_selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/locale/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/locale/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/README.md` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/README.md`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/files/mariadb_config.cnf` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/files/mariadb_config.cnf`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/debian.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/README.md` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/README.md`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/defaults/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/setup-Debian.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/setup-Debian.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/tasks/vhosts.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/tasks/vhosts.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/templates/nginx.conf.j2` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/nginx/templates/vhosts.j2` & `ifrappe_bench-5.16.6/bench/playbooks/roles/nginx/templates/vhosts.j2`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/ntpd/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/ntpd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/packer/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/packer/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/redis/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/redis/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/swap/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/swap/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/virtualbox/tasks/debian_family.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/virtualbox/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml` & `ifrappe_bench-5.16.6/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/tests/test_base.py` & `ifrappe_bench-5.16.6/bench/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/tests/test_init.py` & `ifrappe_bench-5.16.6/bench/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/tests/test_setup_production.py` & `ifrappe_bench-5.16.6/bench/tests/test_setup_production.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/tests/test_utils.py` & `ifrappe_bench-5.16.6/bench/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/__init__.py` & `ifrappe_bench-5.16.6/bench/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/app.py` & `ifrappe_bench-5.16.6/bench/utils/app.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/bench.py` & `ifrappe_bench-5.16.6/bench/utils/bench.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/cli.py` & `ifrappe_bench-5.16.6/bench/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/render.py` & `ifrappe_bench-5.16.6/bench/utils/render.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/system.py` & `ifrappe_bench-5.16.6/bench/utils/system.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/bench/utils/translation.py` & `ifrappe_bench-5.16.6/bench/utils/translation.py`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/.gitignore` & `ifrappe_bench-5.16.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/LICENSE` & `ifrappe_bench-5.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/README.md` & `ifrappe_bench-5.16.6/README.md`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/pyproject.toml` & `ifrappe_bench-5.16.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ifrappe_bench-5.16.5/PKG-INFO` & `ifrappe_bench-5.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifrappe-bench
-Version: 5.16.5
+Version: 5.16.6
 Summary: CLI to manage Multi-tenant deployments for Frappe apps
 Project-URL: Changelog, https://github.com/frappe/bench/releases
 Project-URL: Documentation, https://frappeframework.com/docs/user/en/bench
 Project-URL: Homepage, https://frappe.io/bench
 Project-URL: Source, https://github.com/frappe/bench
 Author-email: Frappe Technologies Pvt Ltd <developers@frappe.io>
 License-Expression: GPL-3.0-only
```


# Comparing `tmp/bbot-1.0.5.1625rc0.tar.gz` & `tmp/bbot-1.0.5.1654rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1625rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1654rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1625rc0.tar` & `bbot-1.0.5.1654rc0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/README.md
--rw-r--r--   0        0        0      211 2023-04-19 17:33:47.795802 bbot-1.0.5.1625rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6478 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13430 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8920 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30113 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     7432 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29289 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4261 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    28275 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9530 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-04-19 17:33:24.599915 bbot-1.0.5.1625rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3731 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25113 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     5001 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10060 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5491 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      311 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    15770 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4481 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10976 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    13620 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4257 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0     5745 2023-04-19 17:33:24.603915 bbot-1.0.5.1625rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     1839 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1787 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1007 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3609 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1606 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8304 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2255 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26114 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3251 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4038 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2591 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    74367 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5859 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4678 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-04-19 17:33:24.607915 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11616 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      476 2023-04-19 17:33:24.611914 bbot-1.0.5.1625rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-04-19 17:33:24.615915 bbot-1.0.5.1625rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-04-19 17:33:24.615915 bbot-1.0.5.1625rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-04-19 17:33:24.615915 bbot-1.0.5.1625rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-04-19 17:33:24.615915 bbot-1.0.5.1625rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-04-19 17:33:47.795802 bbot-1.0.5.1625rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1625rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/LICENSE
+-rw-r--r--   0        0        0    51011 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/README.md
+-rw-r--r--   0        0        0      211 2023-04-26 14:47:36.705750 bbot-1.0.5.1654rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6536 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13693 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8920 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    30371 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     6940 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29460 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4286 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    29037 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9574 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-04-26 14:47:03.869335 bbot-1.0.5.1654rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25359 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     5001 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10060 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5546 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16263 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4481 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11237 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13620 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4245 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:47:03.873335 bbot-1.0.5.1654rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0     9307 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2546 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1787 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1007 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3609 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1606 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8304 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2255 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3251 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4038 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2545 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/helpers.py
+-rw-r--r--   0        0        0    74299 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5859 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4739 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-04-26 14:47:03.877335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11616 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      476 2023-04-26 14:47:03.881335 bbot-1.0.5.1654rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-04-26 14:47:03.885335 bbot-1.0.5.1654rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-04-26 14:47:03.885335 bbot-1.0.5.1654rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-04-26 14:47:03.885335 bbot-1.0.5.1654rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-04-26 14:47:03.889335 bbot-1.0.5.1654rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1338 2023-04-26 14:47:36.701749 bbot-1.0.5.1654rc0/pyproject.toml
+-rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1654rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1625rc0/LICENSE` & `bbot-1.0.5.1654rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/README.md` & `bbot-1.0.5.1654rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/agent/agent.py` & `bbot-1.0.5.1654rc0/bbot/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,19 @@
 
     def send(self, message):
         while 1:
             try:
                 self.ws.send(json.dumps(message))
                 break
             except Exception as e:
+                if getattr(self.scan, "stopping", True):
+                    break
                 log.warning(f"Error sending message: {e}, retrying")
                 log.trace(traceback.format_exc())
                 sleep(1)
-                continue
 
     def on_message(self, ws, message):
         try:
             message = json.loads(message)
         except Exception as e:
             log.warning(f'Failed to JSON-decode message "{message}": {e}')
             return
```

### Comparing `bbot-1.0.5.1625rc0/bbot/cli.py` & `bbot-1.0.5.1654rc0/bbot/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -262,20 +262,26 @@
 
                 if not options.dry_run:
                     if not options.agent_mode and not options.yes and sys.stdin.isatty():
                         log.hugesuccess(f"Scan ready. Press enter to execute {scanner.name}")
                         input()
 
                     def keyboard_listen():
+                        allowed_errors = 10
                         while 1:
                             keyboard_input = "a"
-                            with suppress(Exception):
+                            try:
                                 keyboard_input = input()
+                                allowed_errors = 10
+                            except Exception:
+                                allowed_errors -= 1
                             if not keyboard_input:
                                 toggle_log_level(logger=log)
+                            if allowed_errors <= 0:
+                                break
 
                     keyboard_listen_thread = threading.Thread(target=keyboard_listen, daemon=True)
                     keyboard_listen_thread.start()
 
                     scanner.start_without_generator()
 
             except bbot.core.errors.ScanError as e:
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1654rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1654rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1654rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1654rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/errors.py` & `bbot-1.0.5.1654rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/event/base.py` & `bbot-1.0.5.1654rc0/bbot/core/event/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,23 +418,26 @@
                 return True
             # hostnames and IPs
             return host_in_host(other.host, self.host)
         return False
 
     def json(self, mode="json"):
         j = dict()
-        for i in ("type", "id", "web_spider_distance"):
+        for i in ("type", "id"):
             v = getattr(self, i, "")
             if v:
                 j.update({i: v})
         data_attr = getattr(self, f"data_{mode}", None)
         if data_attr is not None:
             j["data"] = data_attr
         else:
             j["data"] = smart_decode(self.data)
+        web_spider_distance = getattr(self, "web_spider_distance", None)
+        if web_spider_distance is not None:
+            j["web_spider_distance"] = web_spider_distance
         j["scope_distance"] = self.scope_distance
         if self.scan:
             j["scan"] = self.scan.id
         j["timestamp"] = self.timestamp.timestamp()
         if self.host:
             j["resolved_hosts"] = [str(h) for h in self.resolved_hosts]
         source_id = self.source_id
@@ -677,15 +680,16 @@
         return set()
 
 
 class URL_UNVERIFIED(BaseEvent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.web_spider_distance = getattr(self.source, "web_spider_distance", 0)
-        if self.type == "URL_UNVERIFIED":
+        # increment the web spider distance
+        if self.type == "URL_UNVERIFIED" and getattr(self.module, "name", "") != "TARGET":
             self.web_spider_distance += 1
         self.num_redirects = getattr(self.source, "num_redirects", 0)
 
     def sanitize_data(self, data):
         self.parsed = validators.validate_url_parsed(data)
 
         # tag as dir or endpoint
@@ -800,18 +804,16 @@
         for i in data.get("raw_header", "").splitlines():
             if len(i) > 0 and ":" in i:
                 k, v = i.split(":", 1)
                 k = k.strip().lower()
                 v = v.lstrip()
                 header_dict[k] = v
         data["header-dict"] = header_dict
-        return data
-
-    def _data_human(self):
-        data = dict(self.data)
+        # move URL to the front of the dictionary for visibility
+        data = dict(data)
         new_data = {"url": data.pop("url")}
         new_data.update(data)
         return new_data
 
     def _words(self):
         return set()
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1654rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,45 +24,28 @@
 
         - The above is roughly equivalent to:
             ls /etc | grep conf
 
     NOTE: STDERR is logged after the process exits, if its exit code is non-zero
         If you want to see it immediately, pass stderr=None
     """
-
-    if not "stdout" in kwargs:
-        kwargs["stdout"] = subprocess.PIPE
-    if not "stderr" in kwargs:
-        kwargs["stderr"] = subprocess.PIPE
+    command, kwargs = self._prepare_command_kwargs(command, kwargs)
     _input = kwargs.pop("input", "")
-    sudo = kwargs.pop("sudo", False)
     input_msg = ""
     if _input:
         kwargs["stdin"] = subprocess.PIPE
         input_msg = " (with stdin)"
-
-    command = [str(s) for s in command]
-    env = kwargs.get("env", os.environ)
-    if sudo and os.geteuid() != 0:
-        self.depsinstaller.ensure_root()
-        env["SUDO_ASKPASS"] = str((self.tools_dir / self.depsinstaller.askpass_filename).resolve())
-        env["BBOT_SUDO_PASS"] = self.depsinstaller._sudo_password
-        kwargs["env"] = env
-
-        PATH = os.environ.get("PATH", "")
-        LD_LIBRARY_PATH = os.environ.get("LD_LIBRARY_PATH", "")
-        command = ["sudo", "-E", "-A", f"LD_LIBRARY_PATH={LD_LIBRARY_PATH}", f"PATH={PATH}"] + command
     log.hugeverbose(f"run_live{input_msg}: {' '.join(command)}")
     try:
         with catch(subprocess.Popen, command, *args, **kwargs) as process:
             if _input:
                 if type(_input) in (str, bytes):
                     _input = (_input,)
                 self.feed_pipe(process.stdin, _input, text=False)
-            for line in io.TextIOWrapper(process.stdout, encoding="utf-8", errors="ignore"):
+            for line in io.TextIOWrapper(process.stdout, encoding="utf-8", errors="ignore", line_buffering=True):
                 yield line
 
             # surface stderr
             process.wait()
             if process.stderr and process.returncode != 0:
                 stderr = smart_decode(process.stderr.read())
                 if stderr:
@@ -78,44 +61,49 @@
     Simple helper for running a command, and getting its output as a string
         process = run(["ls", "/tmp"])
         process.stdout --> "file1.txt\nfile2.txt"
 
     NOTE: STDERR is captured (not displayed) by default.
         If you want to see it, self.debug(process.stderr) or pass stderr=None
     """
+    command, kwargs = self._prepare_command_kwargs(command, kwargs)
+    if not "text" in kwargs:
+        kwargs["text"] = True
+    log.hugeverbose(f"run: {' '.join(command)}")
+    result = catch(subprocess.run, command, *args, **kwargs)
+
+    # surface stderr
+    if result.stderr and result.returncode != 0:
+        stderr = smart_decode(result.stderr)
+        if stderr:
+            command_str = " ".join(command)
+            log.warning(f"Stderr for {command_str}:\n\t{stderr}")
+
+    return result
+
+
+def _prepare_command_kwargs(self, command, kwargs):
     if not "stdout" in kwargs:
         kwargs["stdout"] = subprocess.PIPE
     if not "stderr" in kwargs:
         kwargs["stderr"] = subprocess.PIPE
-    if not "text" in kwargs:
-        kwargs["text"] = True
     sudo = kwargs.pop("sudo", False)
 
     command = [str(s) for s in command]
     env = kwargs.get("env", os.environ)
     if sudo and os.geteuid() != 0:
         self.depsinstaller.ensure_root()
         env["SUDO_ASKPASS"] = str((self.tools_dir / self.depsinstaller.askpass_filename).resolve())
         env["BBOT_SUDO_PASS"] = self.depsinstaller._sudo_password
         kwargs["env"] = env
 
         PATH = os.environ.get("PATH", "")
         LD_LIBRARY_PATH = os.environ.get("LD_LIBRARY_PATH", "")
         command = ["sudo", "-E", "-A", f"LD_LIBRARY_PATH={LD_LIBRARY_PATH}", f"PATH={PATH}"] + command
-    log.hugeverbose(f"run: {' '.join(command)}")
-    result = catch(subprocess.run, command, *args, **kwargs)
-
-    # surface stderr
-    if result.stderr and result.returncode != 0:
-        stderr = smart_decode(result.stderr)
-        if stderr:
-            command_str = " ".join(command)
-            log.warning(f"Stderr for {command_str}:\n\t{stderr}")
-
-    return result
+    return command, kwargs
 
 
 def catch(callback, *args, **kwargs):
     try:
         return callback(*args, **kwargs)
     except FileNotFoundError as e:
         log.warning(f"{e} - missing executable?")
@@ -204,14 +192,14 @@
         log.trace(traceback.format_exc())
         return
     return filename
 
 
 def tail(filename, callback):
     try:
-        with open(filename) as f:
+        with open(filename, errors="ignore") as f:
             for line in f:
                 line = line.rstrip("\r\n")
                 callback(line)
     except Exception as e:
         log.error(f"Error tailing file {filename}: {e}")
         log.trace(traceback.format_exc())
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import json
 import logging
 import ipaddress
 import traceback
-import cloudcheck
 import dns.resolver
 import dns.exception
 from threading import Lock
 from contextlib import suppress
 
 from .regexes import dns_name_regex
 from bbot.core.errors import ValidationError, DNSError
 from .threadpool import NamedLock, PatchedThreadPoolExecutor
-from .misc import is_ip, is_domain, domain_parents, parent_domain, rand_string
+from .misc import is_ip, is_domain, domain_parents, parent_domain, rand_string, cloudcheck
 
 log = logging.getLogger("bbot.core.helpers.dns")
 
 
 class DNSHelper:
     """
     For automatic wildcard detection, nameserver validation, etc.
@@ -308,19 +307,21 @@
                     if future is None:
                         break
                     futures[future] = t
 
                 for future in self.parent_helper.as_completed(futures):
                     resolved_raw, errors = future.result()
                     for rdtype, e in errors:
-                        event_tags.add(f"{rdtype.lower()}-error")
+                        if rdtype not in resolved_raw:
+                            event_tags.add(f"{rdtype.lower()}-error")
                     for rdtype, records in resolved_raw:
-                        event_tags.add("resolved")
                         rdtype = str(rdtype).upper()
-                        event_tags.add(f"{rdtype.lower()}-record")
+                        if records:
+                            event_tags.add("resolved")
+                            event_tags.add(f"{rdtype.lower()}-record")
 
                         # whitelisting and blacklisting of IPs
                         for r in records:
                             for _, t in self.extract_targets(r):
                                 if t:
                                     ip = self.parent_helper.make_ip_type(t)
 
@@ -352,17 +353,18 @@
                             for ip in ips:
                                 to_check.add(ip)
                     for ip in to_check:
                         provider, provider_type, subnet = cloudcheck.check(ip)
                         if provider:
                             event_tags.add(f"{provider_type}-{provider}")
 
-                # check for private IPs
-                if "resolved" not in event_tags:
+                # if needed, mark as unresolved
+                if not is_ip(event_host) and "resolved" not in event_tags:
                     event_tags.add("unresolved")
+                # check for private IPs
                 for rdtype, ips in dns_children.items():
                     for ip in ips:
                         try:
                             ip = ipaddress.ip_address(ip)
                             if ip.is_private:
                                 event_tags.add("private-ip")
                         except ValueError:
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 log = logging.getLogger("bbot.core.helpers")
 
 
 class ConfigAwareHelper:
     from .web import wordlist, request, download, api_page_iter, curl
     from .cache import cache_get, cache_put, cache_filename, is_cached, CacheDict
-    from .command import run, run_live, tempfile, feed_pipe, _feed_pipe, tempfile_tail
+    from .command import run, run_live, _prepare_command_kwargs, tempfile, feed_pipe, _feed_pipe, tempfile_tail
     from . import ntlm
     from . import regexes
     from . import validators
 
     def __init__(self, config, scan=None):
         self.config = config
         self._scan = scan
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import signal
 import string
 import difflib
 import inspect
 import logging
 import platform
 import ipaddress
-
 import traceback
 import subprocess as sp
 from pathlib import Path
 from itertools import islice
 from datetime import datetime
 from tabulate import tabulate
 import wordninja as _wordninja
 from contextlib import suppress
+import cloudcheck as _cloudcheck
 import tldextract as _tldextract
 from hashlib import sha1 as hashlib_sha1
 from urllib.parse import urlparse, quote, unquote, urlunparse  # noqa F401
 
 from .url import *  # noqa F401
 from . import regexes
 from .. import errors
@@ -199,14 +199,19 @@
     "192.168.1.1" --> [192.168.1.0/31, 192.168.1.0/30 ... 128.0.0.0/1, 0.0.0.0/0]
     """
     net = ipaddress.ip_network(i, strict=False)
     for i in range(net.prefixlen - (0 if include_self else 1), -1, -1):
         yield ipaddress.ip_network(f"{net.network_address}/{i}", strict=False)
 
 
+def is_port(p):
+    p = str(p)
+    return p and p.isdigit() and 0 <= int(p) <= 65535
+
+
 def is_ip(d, version=None):
     """
     "192.168.1.1" --> True
     "bad::c0de" --> True
     "evilcorp.com" --> False
     """
     if type(d) in (ipaddress.IPv4Address, ipaddress.IPv6Address):
@@ -447,15 +452,15 @@
         with open(s, errors="ignore") as f:
             for line in f:
                 yield line.rstrip("\r\n")
     except OSError:
         yield s
 
 
-def chain_lists(l, try_files=False, msg=None):
+def chain_lists(l, try_files=False, msg=None, remove_blank=True):
     """
     Chain together list, splitting entries on comma
         - Optionally try to open entries as files and add their contents to the list
         - Used for parsing a list of arguments that may include space and/or comma-separated values
         - ["a", "b,c,d"] --> ["a", "b", "c", "d"]
         - try_files=True:
             - ["a,file.txt", "c,d"] --> ["a", "f_line1", "f_line2", "f_line3", "c", "d"]
@@ -470,15 +475,18 @@
                     new_msg = str(msg).format(filename=f_path)
                     log.info(new_msg)
                 for line in str_or_file(f):
                     final_list[line] = None
             else:
                 final_list[f] = None
 
-    return list(final_list)
+    ret = list(final_list)
+    if remove_blank:
+        ret = [r for r in ret if r]
+    return ret
 
 
 def list_files(directory, filter=lambda x: True):
     """
     "/tmp/test" --> ["file1.txt", "file2.txt"]
     """
     directory = Path(directory).resolve()
@@ -989,7 +997,26 @@
     return size
 
 
 def is_file(f):
     with suppress(Exception):
         return Path(f).is_file()
     return False
+
+
+provider_map = {"amazon": "aws", "google": "gcp"}
+
+
+def cloudcheck(ip):
+    """
+    Check whether an IP address belongs to a cloud provider
+
+        provider, provider_type, subnet = cloudcheck("168.62.20.37")
+        print(provider) # "Azure"
+        print(provider_type) # "cloud"
+        print(subnet) # IPv4Network('168.62.0.0/19')
+    """
+    provider, provider_type, subnet = _cloudcheck.check(ip)
+    if provider:
+        with suppress(KeyError):
+            provider = provider_map[provider.lower()]
+    return provider, provider_type, subnet
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/names_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     "puffy",
     "pure",
     "queer",
     "questionable",
     "rabid",
     "raging",
     "rambunctious",
+    "rapid_unscheduled",
     "raving",
     "reckless",
     "ripped",
     "sadistic",
     "satanic",
     "savvy",
     "scheming",
@@ -236,14 +237,15 @@
     "unholy",
     "unleashed",
     "unmedicated",
     "unmelted",
     "unmitigated",
     "unrelenting",
     "unrestrained",
+    "unscheduled",
     "unworthy",
     "utmost",
     "vehement",
     "vicious",
     "vigorous",
     "vile",
     "violent",
```

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1654rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1654rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1654rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/defaults.yml` & `bbot-1.0.5.1654rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1654rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1654rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1654rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/base.py` & `bbot-1.0.5.1654rc0/bbot/modules/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
 
     def _postcheck_and_run(self, callback, event):
         acceptable, reason = self._event_postcheck(event)
         if not acceptable:
             if reason:
                 self.debug(f"Not accepting {event} because {reason}")
             return
+        self.scan.stats.event_consumed(event, self)
         return callback(event)
 
     def _register_running(self, callback, *args, **kwargs):
         with self._running_counter:
             return callback(*args, **kwargs)
 
     def _handle_batch(self, force=False):
@@ -416,14 +417,17 @@
             return False, f"module is in error state"
         # exclude non-watched types
         if not any(t in self.get_watched_events() for t in ("*", event.type)):
             return False, "its type is not in watched_events"
         if self.target_only:
             if "target" not in event.tags:
                 return False, "it did not meet target_only filter criteria"
+        # exclude certain URLs (e.g. javascript):
+        if event.type.startswith("URL") and self.name != "httpx" and "httpx-only" in event.tags:
+            return False, "its extension was listed in url_extension_httpx_only"
         # if event is an IP address that was speculated from a CIDR
         source_is_range = getattr(event.source, "type", "") == "IP_RANGE"
         if (
             source_is_range
             and event.type == "IP_ADDRESS"
             and str(event.module) == "speculate"
             and self.name != "speculate"
@@ -492,15 +496,14 @@
             self.debug(f"Not in an acceptable state to queue event")
             return
         acceptable, reason = self._event_precheck(event)
         if not acceptable:
             if reason and reason != "its type is not in watched_events":
                 self.debug(f"Not accepting {event} because {reason}")
             return
-        self.scan.stats.event_consumed(event, self)
         try:
             self.incoming_event_queue.put(event)
         except AttributeError:
             self.debug(f"Not in an acceptable state to queue event")
         with self.event_received:
             self.event_received.notify()
 
@@ -565,18 +568,18 @@
             self._request_failures += 1
         else:
             self._request_failures = 0
         if self._request_failures >= self.failed_request_abort_threshold:
             self.set_error_state(f"Setting error state due to {self._request_failures:,} failed HTTP requests")
         return r
 
-    def is_spider_danger(self, event, url):
+    def is_spider_danger(self, source_event, url):
         url_depth = self.helpers.url_depth(url)
         web_spider_depth = self.scan.config.get("web_spider_depth", 1)
-        spider_distance = getattr(event, "web_spider_distance", 0)
+        spider_distance = getattr(source_event, "web_spider_distance", 0) + 1
         web_spider_distance = self.scan.config.get("web_spider_distance", 0)
         if (url_depth > web_spider_depth) or (spider_distance > web_spider_distance):
             return True
         return False
 
     @property
     def config(self):
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1654rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1654rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1654rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1654rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1654rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1654rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1654rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1654rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1654rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/c99.py` & `bbot-1.0.5.1654rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/censys.py` & `bbot-1.0.5.1654rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1654rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1654rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/crt.py` & `bbot-1.0.5.1654rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1654rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1654rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1654rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1654rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1654rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1654rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1654rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1654rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1654rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1654rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1654rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/github.py` & `bbot-1.0.5.1654rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1654rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1654rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1654rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1654rc0/bbot/modules/httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         if event.module == self:
             return False, "event is from self"
 
         if "spider-danger" in event.tags:
             return False, "event has spider danger"
 
         # scope filtering
-
         in_scope_only = self.config.get("in_scope_only", True)
         safe_to_visit = "httpx-safe" in event.tags
         if not safe_to_visit and (in_scope_only and not self.scan.in_scope(event)):
             return False, "event is not in scope"
         # reject base URLs to avoid visiting a resource twice
         # note: speculate makes open ports from
         return True
@@ -133,19 +132,19 @@
 
             # main URL
             httpx_ip = j.get("host", "unknown")
             tags = [f"status-{status_code}", f"ip-{httpx_ip}"]
             title = self.helpers.tagify(j.get("title", ""))
             if title:
                 tags.append(f"http-title-{title}")
-            url_event = self.make_event(url, "URL", source_event, tags=tags)
+            url_event = self.make_event(url, "URL", source_event, module=source_event.module, tags=tags)
             if url_event:
                 if url_event != source_event:
                     self.emit_event(url_event)
                 else:
                     url_event._resolved.set()
                 # HTTP response
-                self.emit_event(j, "HTTP_RESPONSE", url_event, internal=True)
+                self.emit_event(j, "HTTP_RESPONSE", url_event, module=source_event.module, internal=True)
 
     def cleanup(self):
         resume_file = self.helpers.current_dir / "resume.cfg"
         resume_file.unlink(missing_ok=True)
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1654rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1654rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1654rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1654rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1654rc0/bbot/modules/internal/excavate.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,15 @@
                     else:
                         result = path
 
                 yield result, name
 
     def report(self, result, name, event, **kwargs):
         consider_spider_danger = kwargs.get("consider_spider_danger", True)
+        web_spider_distance = getattr(event, "web_spider_distance", 0)
         exceeded_max_links = kwargs.get("exceeded_max_links", False)
 
         tags = []
 
         parsed_uri = self.excavate.helpers.urlparse(result)
         host, port = self.excavate.helpers.split_host_port(parsed_uri.netloc)
         # Handle non-HTTP URIs (ftp, s3, etc.)
@@ -133,15 +134,21 @@
                 {"protocol": parsed_uri.scheme, "host": str(host)},
                 "PROTOCOL",
                 source=event,
             )
             return
 
         is_spider_danger = self.excavate.is_spider_danger(event, result)
-        if exceeded_max_links or (consider_spider_danger and is_spider_danger):
+        if (
+            exceeded_max_links  # if we exceeded the max number of links
+            or (consider_spider_danger and is_spider_danger)  # or if there's spider danger
+            or (
+                (not consider_spider_danger) and (web_spider_distance > self.excavate.max_redirects)
+            )  # or if the spider distance is way out of control (greater than max_redirects)
+        ):
             tags.append("spider-danger")
 
         self.excavate.debug(f"Found URL [{result}] from parsing [{event.data.get('url')}] with regex [{name}]")
         self.excavate.emit_event(result, "URL_UNVERIFIED", source=event, tags=tags)
 
 
 class EmailExtractor(BaseExtractor):
@@ -311,15 +318,16 @@
 
     def handle_event(self, event):
         data = event.data
 
         # HTTP_RESPONSE is a special case
         if event.type == "HTTP_RESPONSE":
             # handle redirects
-            num_redirects = getattr(event, "num_redirects", 0)
+            web_spider_distance = getattr(event, "web_spider_distance", 0)
+            num_redirects = max(getattr(event, "num_redirects", 0), web_spider_distance)
             location = event.data.get("location", "")
             host = event.host
             if location:
                 scheme = self.helpers.is_uri(location, return_scheme=True)
                 if not scheme:
                     location_parsed = event.parsed._replace(path=location)
                     host, _ = self.helpers.split_host_port(location_parsed.netloc)
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1654rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1654rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1654rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1654rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1654rc0/bbot/modules/masscan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import functools
 import subprocess
 from contextlib import suppress
 
 from bbot.modules.base import BaseModule
 
 
 class masscan(BaseModule):
@@ -134,24 +133,29 @@
         # config file
         masscan_config = self.masscan_config.replace(self._target_findkey, targets)
         self.debug("Masscan config:")
         for line in masscan_config.splitlines():
             self.debug(line)
         config_file = self.helpers.tempfile(masscan_config)
         # output file
-        process_output = functools.partial(self.process_output, result_callback=result_callback)
-        json_output_file = self.helpers.tempfile_tail(process_output)
+        # process_output = functools.partial(self.process_output, result_callback=result_callback)
+        # json_output_file = self.helpers.tempfile_tail(process_output)
         # command
         command = self._build_masscan_command(config=config_file, exclude=exclude, ping=ping)
-        command += ("-oJ", json_output_file)
         # execute
-        self.helpers.run(command, sudo=True)
+        stats_file = self.helpers.tempfile_tail(callback=self.verbose)
+        try:
+            with open(stats_file, "w") as stats_fh:
+                for line in self.helpers.run_live(command, sudo=True, stderr=stats_fh):
+                    self.process_output(line, result_callback=result_callback)
+        finally:
+            stats_file.unlink()
 
     def _build_masscan_command(self, targets=None, config=None, exclude=None, dry_run=False, ping=False):
-        command = ("masscan", "--rate", self.rate, "--wait", self.wait, "--open-only")
+        command = ("masscan", "--rate", self.rate, "--wait", self.wait, "--open-only", "-oJ", "-")
         if targets is not None:
             command += (targets,)
         if config is not None:
             command += ("-c", config)
         if ping:
             command += ("--ping",)
         elif not dry_run:
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1654rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1654rc0/bbot/modules/naabu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import subprocess
 from bbot.modules.base import BaseModule
 
 
 class naabu(BaseModule):
-    watched_events = ["IP_ADDRESS", "DNS_NAME", "IP_RANGE"]
+    watched_events = ["IP_ADDRESS", "DNS_NAME"]
     produced_events = ["OPEN_TCP_PORT"]
     flags = ["active", "portscan", "aggressive", "web-thorough"]
     meta = {"description": "Execute port scans with naabu"}
     options = {
         "ports": "",
         "top_ports": 100,
         "skip_host_discovery": True,
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1654rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/otx.py` & `bbot-1.0.5.1654rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,50 +10,67 @@
     options = {"output_file": ""}
     options_desc = {"output_file": "Output to CSV file"}
 
     header_row = ["Event type", "Event data", "IP Address", "Source Module", "Scope Distance", "Event Tags"]
     filename = "output.csv"
 
     def setup(self):
+        self.custom_headers = []
+        self._headers_set = set()
         self._writer = None
         self._prep_output_dir(self.filename)
         return True
 
     @property
     def writer(self):
         if self._writer is None:
-            self._writer = csv.writer(self.file)
-            self._writer.writerow(self.header_row)
+            self._writer = csv.DictWriter(self.file, fieldnames=self.fieldnames)
+            self._writer.writeheader()
         return self._writer
 
     @property
     def file(self):
         if self._file is None:
             if self.output_file.is_file():
                 self.helpers.backup_file(self.output_file)
             self._file = open(self.output_file, mode="a", newline="")
         return self._file
 
+    @property
+    def fieldnames(self):
+        return self.header_row + list(self.custom_headers)
+
     def writerow(self, row):
         self.writer.writerow(row)
         self.file.flush()
 
     def handle_event(self, event):
+        # ["Event type", "Event data", "IP Address", "Source Module", "Scope Distance", "Event Tags"]
         self.writerow(
-            [
-                getattr(event, "type", ""),
-                getattr(event, "data", ""),
-                ",".join(str(x) for x in getattr(event, "resolved_hosts", set()) if self.helpers.is_ip(x)),
-                str(getattr(event, "module", "")),
-                str(getattr(event, "scope_distance", "")),
-                ",".join(sorted(list(getattr(event, "tags", [])))),
-            ]
+            {
+                "Event type": getattr(event, "type", ""),
+                "Event data": getattr(event, "data", ""),
+                "IP Address": ",".join(
+                    str(x) for x in getattr(event, "resolved_hosts", set()) if self.helpers.is_ip(x)
+                ),
+                "Source Module": str(getattr(event, "module", "")),
+                "Scope Distance": str(getattr(event, "scope_distance", "")),
+                "Event Tags": ",".join(sorted(list(getattr(event, "tags", [])))),
+            }
         )
 
     def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
     def report(self):
         if self._file is not None:
             self.info(f"Saved CSV output to {self.output_file}")
+
+    def add_custom_headers(self, headers):
+        if isinstance(headers, str):
+            headers = [headers]
+        for header in headers:
+            if header not in self._headers_set:
+                self._headers_set.add(header)
+                self.custom_headers.append(header)
```

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1654rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1654rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1654rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1654rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1654rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1654rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1654rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1654rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1654rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1654rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/robots.py` & `bbot-1.0.5.1654rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1654rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1654rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1654rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1654rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1654rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/social.py` & `bbot-1.0.5.1654rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1654rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1654rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1654rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1654rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1654rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1654rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1654rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1654rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1654rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1654rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1654rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1654rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1654rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1654rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1654rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/scanner/target.py` & `bbot-1.0.5.1654rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1654rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/conftest.py` & `bbot-1.0.5.1654rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/helpers.py` & `bbot-1.0.5.1654rc0/bbot/test/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
         return
 
     def setup(self):
         pass
 
     def run(self):
         events = list(self.scan.start())
-        for e in events:
-            print(e)
         events = [e for e in events if e.module == self.module]
         assert self.check_events(events)
 
     @abstractmethod
     def check_events(self, events):
         raise NotImplementedError
```

### Comparing `bbot-1.0.5.1625rc0/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1654rc0/bbot/test/modules_test_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class Httpx(HttpxMockHelper):
     def mock_args(self):
         request_args = dict(headers={"test": "header"})
         respond_args = dict(response_data=json.dumps({"foo": "bar"}))
         self.set_expect_requests(request_args, respond_args)
 
+    def run(self):
+        events = list(self.scan.start())
+        assert self.check_events(events)
+
     def check_events(self, events):
         for e in events:
             if e.type == "HTTP_RESPONSE":
                 j = json.loads(e.data["body"])
                 if j.get("foo", "") == "bar":
                     return True
         return False
@@ -749,23 +753,21 @@
             self.scan2.modules["masscan"].masscan_config = self.masscan_config
 
         self.setup_scan_2 = setup_scan_2
         self.masscan_run = False
 
     def run_masscan(self, command, *args, **kwargs):
         if "masscan" in command[0]:
-            json_output_file = command[-1]
-            with open(json_output_file, "w") as f:
-                f.write(self.masscan_output)
+            yield from self.masscan_output.splitlines()
             self.masscan_run = True
         else:
-            return self.scan.helpers.run(command, *args, **kwargs)
+            yield from self.scan.helpers.run_live(command, *args, **kwargs)
 
     def patch_scan(self, scan):
-        scan.helpers.run = self.run_masscan
+        scan.helpers.run_live = self.run_masscan
 
     def run(self):
         super().run()
         self.setup_scan_2()
         assert self.masscan_run == True, "masscan didn't run when it was supposed to"
         self.masscan_run = False
         events = list(self.scan2.start())
@@ -877,16 +879,14 @@
         )
 
     def run(self):
         with requests_mock.Mocker() as m:
             self.m = m
             self.mock_args_requests()
             events = list(self.scan.start())
-            for e in events:
-                print(e)
             self.check_events(events)
 
     def check_events(self, events):
         for provider in self.providers:
             # make sure buckets were excavated
             assert any(
                 e.type == "STORAGE_BUCKET" and str(e.module) == f"{provider}_cloud" for e in events
@@ -1266,15 +1266,14 @@
         basic_detection = False
         mutaton_of_detected = False
         basehost_mutation = False
         special_vhost_list = False
         wordcloud_detection = False
 
         for e in events:
-            print(e)
             if e.type == "VHOST":
                 if e.data["vhost"] == "admin":
                     basic_detection = True
                 if e.data["vhost"] == "cloud":
                     mutaton_of_detected = True
                 if e.data["vhost"] == "q-cloud":
                     basehost_mutation = True
@@ -1597,15 +1596,14 @@
         respond_args = {"response_data": "<html>Copyright 1984</html>"}
         self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
     def check_events(self, events):
         first_run_detect = False
         second_run_detect = False
         for e in events:
-            print(e.type)
             if e.type == "FINDING":
                 if "Directory listing enabled" in e.data["description"]:
                     first_run_detect = True
                 elif "Copyright" in e.data["description"]:
                     second_run_detect = True
         if first_run_detect and second_run_detect:
             return True
```

### Comparing `bbot-1.0.5.1625rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1654rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test.conf` & `bbot-1.0.5.1654rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_1/test_modules_full.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 from ..bbot_fixtures import *
 
 
-def test_cli(monkeypatch, caplog, bbot_config):
+def test_cli(monkeypatch, bbot_config):
     from bbot import cli
 
     monkeypatch.setattr(sys, "exit", lambda *args, **kwargs: True)
     monkeypatch.setattr(os, "_exit", lambda *args, **kwargs: True)
     monkeypatch.setattr(cli, "config", bbot_config)
 
     old_sys_argv = sys.argv
 
-    # basic scan
     home_dir = Path(bbot_config["home"])
+    scans_home = home_dir / "scans"
+
+    # basic scan
     monkeypatch.setattr(
         sys,
         "argv",
         [
             "bbot",
             "-y",
             "-t",
             "127.0.0.1",
             "www.example.com",
             "-om",
             "human",
             "csv",
             "json",
             "-n",
-            "test_scan",
+            "test_cli_scan",
             "-c",
             "dns_resolution=False",
+            "-o",
+            "/tmp",
         ],
     )
-    caplog.set_level(0, logger="bbot")
     cli.main()
-    caplog.set_level(9999, logger="bbot")
+
+    scan_home = scans_home / "test_cli_scan"
+    assert (scan_home / "wordcloud.tsv").is_file()
+    assert (scan_home / "output.txt").is_file()
+    assert (scan_home / "output.csv").is_file()
+    assert (scan_home / "output.json").is_file()
+    with open(scan_home / "output.csv") as f:
+        lines = f.readlines()
+        assert lines[0] == "Event type,Event data,IP Address,Source Module,Scope Distance,Event Tags\n"
+        assert len(lines) > 1
+
     ip_success = False
     dns_success = False
-    for r in caplog.records:
-        if r.levelname == "STDOUT":
-            if "[IP_ADDRESS]        \t127.0.0.1\tTARGET" in r.message:
+    output_filename = scan_home / "output.txt"
+    with open(output_filename) as f:
+        lines = f.read().splitlines()
+        for line in lines:
+            if "[IP_ADDRESS]        \t127.0.0.1\tTARGET" in line:
                 ip_success = True
-            if "[DNS_NAME]          \twww.example.com\tTARGET" in r.message:
+            if "[DNS_NAME]          \twww.example.com\tTARGET" in line:
                 dns_success = True
     assert ip_success and dns_success
 
     # show version
     monkeypatch.setattr("sys.argv", ["bbot", "--version"])
     cli.main()
 
@@ -59,24 +74,14 @@
     # list module options
     monkeypatch.setattr("sys.argv", ["bbot", "--help-all"])
     cli.main()
 
     # unpatch sys.argv
     monkeypatch.setattr("sys.argv", old_sys_argv)
 
-    scan_home = home_dir / "scans" / "test_scan"
-    assert (scan_home / "wordcloud.tsv").is_file()
-    assert (scan_home / "output.txt").is_file()
-    assert (scan_home / "output.csv").is_file()
-    assert (scan_home / "output.json").is_file()
-    with open(scan_home / "output.csv") as f:
-        lines = f.readlines()
-        assert lines[0] == "Event type,Event data,IP Address,Source Module,Scope Distance,Event Tags\n"
-        assert len(lines) > 1
-
 
 def test_config_validation(monkeypatch, capsys, bbot_config):
     from bbot import cli
     from bbot.core.configurator import args
 
     monkeypatch.setattr(sys, "exit", lambda *args, **kwargs: True)
     monkeypatch.setattr(os, "_exit", lambda *args, **kwargs: True)
```

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1654rc0/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1654rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1654rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1654rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1654rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1625rc0/pyproject.toml` & `bbot-1.0.5.1654rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1625rc"
+version = "v1.0.5.1654rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1625rc0/PKG-INFO` & `bbot-1.0.5.1654rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1625rc0
+Version: 1.0.5.1654rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


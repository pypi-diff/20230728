# Comparing `tmp/bbot-1.1.0.1958rc0.tar.gz` & `tmp/bbot-1.1.0.2024rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.0.1958rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.0.2024rc0.tar", max compression
```

## Comparing `bbot-1.1.0.1958rc0.tar` & `bbot-1.1.0.2024rc0.tar`

### file list

```diff
@@ -1,290 +1,293 @@
--rw-r--r--   0        0        0    32473 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/LICENSE
--rw-r--r--   0        0        0     6679 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-17 21:39:01.010223 bbot-1.1.0.1958rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14945 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9721 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5290 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1314 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1115 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       61 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-17 21:38:38.789515 bbot-1.1.0.1958rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9315 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    28361 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4281 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    36996 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    17481 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2282 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13681 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8020 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4094 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1202 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     3505 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    26361 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4851 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5922 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      908 2023-07-17 21:38:38.793515 bbot-1.1.0.1958rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5718 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13949 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11600 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7138 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5795 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9382 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16428 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5280 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15129 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5163 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      728 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11378 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1845 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     8861 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2007 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1398 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11061 2023-07-17 21:38:38.797515 bbot-1.1.0.1958rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1397 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27985 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     4763 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10464 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     3987 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1103 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    15109 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    27583 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7957 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     9758 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     8916 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     2757 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     1949 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-17 21:38:38.801515 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9253 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10661 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     6024 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-17 21:38:38.805516 bbot-1.1.0.1958rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-17 21:38:38.813516 bbot-1.1.0.1958rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1576 2023-07-17 21:39:01.010223 bbot-1.1.0.1958rc0/pyproject.toml
--rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 bbot-1.1.0.1958rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/LICENSE
+-rw-r--r--   0        0        0     6611 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-28 21:18:32.019552 bbot-1.1.0.2024rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14945 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9721 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5290 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1314 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1182 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1115 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       61 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     2985 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5271 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9315 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    28343 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4281 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-28 21:18:13.571636 bbot-1.1.0.2024rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    37365 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    17480 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1491 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2661 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3123 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    14658 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8020 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4097 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1344 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     3505 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2768 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    26642 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5441 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5922 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      689 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5718 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13946 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15894 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0      884 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     2539 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11597 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1313 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      856 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7138 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5795 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9362 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16428 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5279 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1519 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-28 21:18:13.575636 bbot-1.1.0.2024rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    16018 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     5248 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     5006 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5620 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      728 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11404 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1845 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9436 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8373 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2007 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1398 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8151 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0     1249 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      507 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11098 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4010 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1397 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2307 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    25632 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27991 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     4763 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10464 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1103 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-28 21:18:13.579636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    15109 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    28277 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7957 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     9758 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7135 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2664 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     8916 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     2757 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     1949 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      564 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     1613 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0      972 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      659 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-28 21:18:13.583636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9356 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      610 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0      611 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     6024 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2374 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-28 21:18:13.587636 bbot-1.1.0.2024rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-28 21:18:13.595636 bbot-1.1.0.2024rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1595 2023-07-28 21:18:32.019552 bbot-1.1.0.2024rc0/pyproject.toml
+-rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 bbot-1.1.0.2024rc0/PKG-INFO
```

### Comparing `bbot-1.1.0.1958rc0/LICENSE` & `bbot-1.1.0.2024rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/README.md` & `bbot-1.1.0.2024rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,23 @@
+![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
+
 # BEE·bot
 
 ### OSINT automation for hackers.
 
 [![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot) [![Pypi Downloads](https://img.shields.io/pypi/dm/bbot)](https://pypi.org/project/bbot) [![Discord](https://img.shields.io/discord/859164869970362439)](https://discord.com/invite/PZqkgxu5SA)
 
 BBOT is a modular, recursive OSINT framework that can execute the entire OSINT workflow in a single command.
 
-![bbot_banner](https://github.com/blacklanternsecurity/bbot/assets/20261699/af2e822c-d7d6-40e7-bcba-2ce52faa6c4c)
-
 BBOT is inspired by [Spiderfoot](https://github.com/smicallef/spiderfoot) but takes it to the next level with features like multi-target scans, lightning-fast asyncio performance, and NLP-powered subdomain mutations. It offers a wide range of functionality, including subdomain enumeration, port scanning, web screenshots, vulnerability scanning, and much more. 
 
 ![subdomain-stats-boeing](https://github.com/blacklanternsecurity/bbot/assets/20261699/de0154c1-476e-4337-9599-45a1c5e0e78b)
 
 BBOT typically outperforms other subdomain enumeration tools by 20-25%. To learn how this is possible, see [How It Works](https://www.blacklanternsecurity.com/bbot/how_it_works/).
 
-## Consider checking out our [Documentation](https://www.blacklanternsecurity.com/bbot):
-
-<!-- BBOT DOCS TOC -->
-- **Basics**
-    - [Getting Started](https://www.blacklanternsecurity.com/bbot/)
-    - [How it Works](https://www.blacklanternsecurity.com/bbot/how_it_works)
-    - [Comparison to Other Tools](https://www.blacklanternsecurity.com/bbot/comparison)
-- **Scanning**
-    - [Scanning Overview](https://www.blacklanternsecurity.com/bbot/scanning/)
-    - [Events](https://www.blacklanternsecurity.com/bbot/scanning/events)
-    - [Output](https://www.blacklanternsecurity.com/bbot/scanning/output)
-    - [Tips and Tricks](https://www.blacklanternsecurity.com/bbot/scanning/tips_and_tricks)
-    - [Advanced Usage](https://www.blacklanternsecurity.com/bbot/scanning/advanced)
-    - [Configuration](https://www.blacklanternsecurity.com/bbot/scanning/configuration)
-    - [List of Modules](https://www.blacklanternsecurity.com/bbot/scanning/list_of_modules)
-- **Contribution**
-    - [How to Write a Module](https://www.blacklanternsecurity.com/bbot/contribution)
-- **Misc**
-    - [Release History](https://www.blacklanternsecurity.com/bbot/release_history)
-<!-- END BBOT DOCS TOC -->
-
 ## Installation ([pip](https://pypi.org/project/bbot/))
 
 For more installation methods including [Docker](https://hub.docker.com/r/blacklanternsecurity/bbot), see [Installation](https://www.blacklanternsecurity.com/bbot/#installation).
 
 ```bash
 # Prerequisites:
 # - Linux (Windows and macOS are *not* supported)
@@ -135,14 +114,35 @@
     async for event in scan.async_start():
         print(event.json())
 
 import asyncio
 asyncio.run(main())
 ```
 
+## Documentation
+
+<!-- BBOT DOCS TOC -->
+- **Basics**
+    - [Getting Started](https://www.blacklanternsecurity.com/bbot/)
+    - [How it Works](https://www.blacklanternsecurity.com/bbot/how_it_works)
+    - [Comparison to Other Tools](https://www.blacklanternsecurity.com/bbot/comparison)
+- **Scanning**
+    - [Scanning Overview](https://www.blacklanternsecurity.com/bbot/scanning/)
+    - [Events](https://www.blacklanternsecurity.com/bbot/scanning/events)
+    - [Output](https://www.blacklanternsecurity.com/bbot/scanning/output)
+    - [Tips and Tricks](https://www.blacklanternsecurity.com/bbot/scanning/tips_and_tricks)
+    - [Advanced Usage](https://www.blacklanternsecurity.com/bbot/scanning/advanced)
+    - [Configuration](https://www.blacklanternsecurity.com/bbot/scanning/configuration)
+    - [List of Modules](https://www.blacklanternsecurity.com/bbot/scanning/list_of_modules)
+- **Contribution**
+    - [How to Write a Module](https://www.blacklanternsecurity.com/bbot/contribution)
+- **Misc**
+    - [Release History](https://www.blacklanternsecurity.com/bbot/release_history)
+<!-- END BBOT DOCS TOC -->
+
 ## Acknowledgements
 
 Thanks to these amazing people for contributing to BBOT! :heart:
 
 If you're interested in contributing to BBOT, or just curious how it works under the hood, see [Contribution](https://www.blacklanternsecurity.com/bbot/contribution/).
 
 <p align="center">
```

### Comparing `bbot-1.1.0.1958rc0/bbot/agent/agent.py` & `bbot-1.1.0.2024rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/cli.py` & `bbot-1.1.0.2024rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.0.2024rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/configurator/args.py` & `bbot-1.1.0.2024rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/configurator/environ.py` & `bbot-1.1.0.2024rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/configurator/files.py` & `bbot-1.1.0.2024rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/errors.py` & `bbot-1.1.0.2024rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/event/base.py` & `bbot-1.1.0.2024rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/flags.py` & `bbot-1.1.0.2024rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/async_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import uuid
 import asyncio
 import logging
 import threading
+from datetime import datetime
 from queue import Queue, Empty
+from .misc import human_timedelta
 from contextlib import asynccontextmanager
 
 log = logging.getLogger("bbot.core.helpers.async_helpers")
 
 from .cache import CacheDict
 
 
@@ -35,21 +38,44 @@
             self._cache.put(name, lock)
         async with lock:
             yield
 
 
 class TaskCounter:
     def __init__(self):
-        self.value = 0
+        self.tasks = {}
 
-    def __enter__(self):
-        self.value += 1
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.value -= 1
+    @property
+    def value(self):
+        return len(self.tasks)
+
+    def count(self, task_name):
+        if callable(task_name):
+            task_name = f"{task_name.__qualname__}()"
+        return self.Task(self, task_name)
+
+    class Task:
+        def __init__(self, manager, task_name):
+            self.manager = manager
+            self.task_name = task_name
+            self.task_id = None
+            self.start_time = None
+
+        async def __aenter__(self):
+            self.task_id = uuid.uuid4()  # generate a unique ID for the task
+            self.start_time = datetime.now()
+            self.manager.tasks[self.task_id] = self
+            return self.task_id  # this will be passed as 'task_id' to __aexit__
+
+        async def __aexit__(self, exc_type, exc_val, exc_tb):
+            self.manager.tasks.pop(self.task_id, None)  # remove only current task
+
+        def __str__(self):
+            running_for = human_timedelta(datetime.now() - self.start_time)
+            return f"{self.task_name} running for {running_for}"
 
 
 def async_to_sync_gen(async_gen):
     # Queue to hold generated values
     queue = Queue()
 
     # Flag to indicate if the async generator is done
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/cache.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/command.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,18 @@
                 _input = b"\n".join(smart_encode(i) for i in _input) + b"\n"
             else:
                 _input = smart_encode(_input)
         stdout, stderr = await proc.communicate(_input)
 
         # surface stderr
         if text:
-            stderr = smart_decode(stderr)
-            stdout = smart_decode(stdout)
+            if stderr is not None:
+                stderr = smart_decode(stderr)
+            if stdout is not None:
+                stdout = smart_decode(stdout)
         if proc.returncode:
             if check:
                 raise CalledProcessError(proc.returncode, command, output=stdout, stderr=stderr)
             if stderr:
                 command_str = " ".join(command)
                 log.warning(f"Stderr for run({command_str}):\n\t{stderr}")
 
@@ -59,23 +61,26 @@
             else:
                 line = line.rstrip(b"\r\n")
             yield line
 
         if input_task is not None:
             try:
                 await input_task
-            except BrokenPipeError:
+            except ConnectionError:
+                log.trace(f"ConnectionError in command: {command}, kwargs={kwargs}")
                 log.trace(traceback.format_exc())
         await proc.wait()
 
         if proc.returncode:
             stdout, stderr = await proc.communicate()
             if text:
-                stderr = smart_decode(stderr)
-                stdout = smart_decode(stdout)
+                if stderr is not None:
+                    stderr = smart_decode(stderr)
+                if stdout is not None:
+                    stdout = smart_decode(stdout)
             if check:
                 raise CalledProcessError(proc.returncode, command, output=stdout, stderr=stderr)
             # surface stderr
             if stderr:
                 command_str = " ".join(command)
                 log.warning(f"Stderr for run_live({command_str}):\n\t{stderr}")
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/diff.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/dns.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import asyncio
 import logging
 import ipaddress
 import traceback
 import contextlib
 import dns.exception
 import dns.asyncresolver
 
 from .regexes import dns_name_regex
 from bbot.core.helpers.ratelimiter import RateLimiter
 from bbot.core.helpers.async_helpers import NamedLock
 from bbot.core.errors import ValidationError, DNSError
-from .misc import is_ip, is_domain, is_dns_name, domain_parents, parent_domain, rand_string, cloudcheck
+from .misc import is_ip, is_domain, is_dns_name, domain_parents, parent_domain, rand_string, cloudcheck, as_completed
 
 log = logging.getLogger("bbot.core.helpers.dns")
 
 
 class DNSHelper:
     """
     For automatic wildcard detection, nameserver validation, etc.
@@ -303,16 +302,16 @@
             else:
                 if event.type == "DNS_NAME" and not minimal:
                     types = self.all_rdtypes
                 else:
                     types = ("A", "AAAA")
 
             if types:
-                tasks = [asyncio.create_task(self.resolve_raw(event_host, type=t, cache_result=True)) for t in types]
-                for task in asyncio.as_completed(tasks):
+                tasks = [self.resolve_raw(event_host, type=t, cache_result=True) for t in types]
+                async for task in as_completed(tasks):
                     resolved_raw, errors = await task
                     for rdtype, e in errors:
                         if rdtype not in resolved_raw:
                             event_tags.add(f"{rdtype.lower()}-error")
                     for rdtype, records in resolved_raw:
                         rdtype = str(rdtype).upper()
                         if records:
@@ -390,19 +389,21 @@
     async def resolve_batch(self, queries, **kwargs):
         """
         await resolve_batch(["www.evilcorp.com", "evilcorp.com"]) --> [
             ("www.evilcorp.com", {"1.1.1.1"}),
             ("evilcorp.com", {"2.2.2.2"})
         ]
         """
-
-        for task in asyncio.as_completed(
-            [asyncio.create_task(self._resolve_batch_coro_wrapper(q, **kwargs)) for q in queries]
-        ):
-            yield await task
+        queries = list(queries)
+        batch_size = 250
+        for i in range(0, len(queries), batch_size):
+            batch = queries[i : i + batch_size]
+            tasks = [self._resolve_batch_coro_wrapper(q, **kwargs) for q in batch]
+            async for task in as_completed(tasks):
+                yield await task
 
     def extract_targets(self, record):
         """
         Extract whatever hostnames/IPs a DNS records points to
         """
         results = set()
         rdtype = str(record.rdtype.name).upper()
@@ -491,20 +492,18 @@
         wildcard_tasks = {t: [] for t in self.all_rdtypes}
         base_query_ips = dict()
         # if the caller hasn't already done the work of resolving the IPs
         if ips is None:
             # then resolve the query for all rdtypes
             for _rdtype in self.all_rdtypes:
                 # resolve the base query
-                wildcard_tasks[_rdtype].append(
-                    asyncio.create_task(self.resolve_raw(query, type=_rdtype, cache_result=True))
-                )
+                wildcard_tasks[_rdtype].append(self.resolve_raw(query, type=_rdtype, cache_result=True))
 
             for _rdtype, tasks in wildcard_tasks.items():
-                for task in asyncio.as_completed(tasks):
+                async for task in as_completed(tasks):
                     raw_results, errors = await task
                     if errors and not raw_results:
                         self.debug(f"Failed to resolve {query} ({_rdtype}) during wildcard detection")
                         result[_rdtype] = (None, parent)
                         continue
                     for __rdtype, answers in raw_results:
                         base_query_ips[__rdtype] = set()
@@ -580,23 +579,21 @@
                 # resolve a bunch of random subdomains of the same parent
                 for rdtype in self.all_rdtypes:
                     # continue if a wildcard was already found for this rdtype
                     # if rdtype in self._wildcard_cache[host_hash]:
                     #     continue
                     for _ in range(self.wildcard_tests):
                         rand_query = f"{rand_string(digits=False, length=10)}.{host}"
-                        wildcard_tasks[rdtype].append(
-                            asyncio.create_task(self.resolve(rand_query, type=rdtype, cache_result=False))
-                        )
+                        wildcard_tasks[rdtype].append(self.resolve(rand_query, type=rdtype, cache_result=False))
 
                 # combine the random results
                 is_wildcard = False
                 wildcard_results = dict()
                 for rdtype, tasks in wildcard_tasks.items():
-                    for task in asyncio.as_completed(tasks):
+                    async for task in as_completed(tasks):
                         results = await task
                         if results:
                             is_wildcard = True
                             if not rdtype in wildcard_results:
                                 wildcard_results[rdtype] = set()
                             wildcard_results[rdtype].update(results)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/files.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/helper.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/logger.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/misc.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 import wordninja as _wordninja
 from contextlib import suppress
 import cloudcheck as _cloudcheck
 import tldextract as _tldextract
 import xml.etree.ElementTree as ET
 from collections.abc import Mapping
 from hashlib import sha1 as hashlib_sha1
+from asyncio import create_task, sleep, wait_for  # noqa
 from urllib.parse import urlparse, quote, unquote, urlunparse  # noqa F401
-from asyncio import as_completed, create_task, sleep, wait_for  # noqa
 
 from .url import *  # noqa F401
 from .. import errors
 from .punycode import *  # noqa F401
 from .logger import log_to_stderr
 from . import regexes as bbot_regexes
 from .names_generator import random_name, names, adjectives  # noqa F401
@@ -235,15 +235,15 @@
 
 def is_ip(d, version=None):
     """
     "192.168.1.1" --> True
     "bad::c0de" --> True
     "evilcorp.com" --> False
     """
-    if type(d) in (ipaddress.IPv4Address, ipaddress.IPv6Address):
+    if isinstance(d, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
         if version is None or version == d.version:
             return True
     try:
         ip = ipaddress.ip_address(d)
         if version is None or ip.version == version:
             return True
     except Exception:
@@ -973,15 +973,18 @@
     result = []
     if hours:
         result.append(f"{hours:,} hour" + ("s" if hours > 1 else ""))
     if minutes:
         result.append(f"{minutes:,} minute" + ("s" if minutes > 1 else ""))
     if seconds:
         result.append(f"{seconds:,} second" + ("s" if seconds > 1 else ""))
-    return ", ".join(result)
+    ret = ", ".join(result)
+    if not ret:
+        ret = "0 seconds"
+    return ret
 
 
 def bytes_to_human(_bytes):
     """
     Converts bytes to human-readable filesize
         bytes_to_human(1234129384) --> "1.15GB"
     """
@@ -1271,7 +1274,16 @@
     result = []
 
     for element in elements:
         if any((c in '<>:"/\\|?*') or (ord(c) < 32 and c != " ") for c in element):
             raise ValueError(f"Invalid character in string: {element}")
         result.append(element)
     return result
+
+
+async def as_completed(coros):
+    tasks = {coro if isinstance(coro, asyncio.Task) else asyncio.create_task(coro): coro for coro in coros}
+    while tasks:
+        done, _ = await asyncio.wait(tasks.keys(), return_when=asyncio.FIRST_COMPLETED)
+        for task in done:
+            tasks.pop(task)
+            yield task
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/modules.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
     def recommend_dependencies(self, modules):
         """
         Returns a dictionary containing missing dependencies and their suggested resolutions
         """
         resolve_choices = {}
         # step 1: build a dictionary containing event types and their associated modules
-        # {"IP_ADDRESS": set("naabu", "ipneighbor", ...)}
+        # {"IP_ADDRESS": set("nmap", "ipneighbor", ...)}
         watched = {}
         produced = {}
         for modname in modules:
             preloaded = self._preloaded.get(modname)
             if preloaded:
                 for event_type in preloaded.get("watched_events", []):
                     self.add_or_create(watched, event_type, modname)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/regexes.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,56 +17,67 @@
 ]
 
 word_regex = re.compile(r"[^\d\W_]+")
 word_num_regex = re.compile(r"[^\W_]+")
 num_regex = re.compile(r"\d+")
 _ipv6_regex = r"[A-F0-9:]*:[A-F0-9:]*:[A-F0-9:]*"
 ipv6_regex = re.compile(_ipv6_regex, re.I)
-_dns_name_regex = r"(?:(?:[\w-]+)\.)+(?:[^\W_0-9]{2,20})"
-_hostname_regex = r"^[\w-]+$"
-_email_regex = r"(?:[^\W_][\w\-\.\+]{,100})@(?:\w[\w\-\._]{,100})\.(?:[^\W_0-9]{2,8})"
+# dns names with periods
+_dns_name_regex = r"(?:\w(?:[\w-]{0,100}\w)?\.)+[^\W_]{1,63}"
+# dns names without periods
+_hostname_regex = r"(?!\w*\.\w+)\w(?:[\w-]{0,100}\w)?"
+_email_regex = r"(?:[^\W_][\w\-\.\+]{,100})@" + _dns_name_regex
 email_regex = re.compile(_email_regex, re.I)
 _ptr_regex = r"(?:[0-9]{1,3}[-_\.]){3}[0-9]{1,3}"
 ptr_regex = re.compile(_ptr_regex)
+
+_open_port_regexes = (
+    _dns_name_regex + r":[0-9]{1,5}",
+    _hostname_regex + r":[0-9]{1,5}",
+    r"\[" + _ipv6_regex + r"\]:[0-9]{1,5}",
+)
+open_port_regexes = list(re.compile(r, re.I) for r in _open_port_regexes)
+
 _url_regexes = (
-    r"https?://((?:\w|\w[\w\-]*\w)[\.]?)+(?:\w[\w\-]*\w|\w)(?::[0-9]{1,5})?.*$",
-    r"https?://\[" + _ipv6_regex + r"\](?::[0-9]{1,5})?.*$",
+    r"https?://" + _dns_name_regex + r"(?::[0-9]{1,5})?(?:(?:/|\?).*)?",
+    r"https?://" + _hostname_regex + r"(?::[0-9]{1,5})?(?:(?:/|\?).*)?",
+    r"https?://\[" + _ipv6_regex + r"\](?::[0-9]{1,5})?(?:(?:/|\?).*)?",
 )
 url_regexes = list(re.compile(r, re.I) for r in _url_regexes)
 
 event_type_regexes = OrderedDict(
     (
         (k, tuple(re.compile(r, re.I) for r in regexes))
         for k, regexes in (
             (
                 "DNS_NAME",
-                (r"^" + _dns_name_regex + r"$",),
+                (
+                    r"^" + _dns_name_regex + r"$",
+                    r"^" + _hostname_regex + r"$",
+                ),
             ),
             (
                 "EMAIL_ADDRESS",
                 (r"^" + _email_regex + r"$",),
             ),
             (
                 "OPEN_TCP_PORT",
-                (
-                    r"^((?:\w|\w[\w\-]*\w)[\.]?)+(?:\w[\w\-]*\w|\w):[0-9]{1,5}$",
-                    r"^\[" + _ipv6_regex + r"\]:[0-9]{1,5}$",
-                ),
+                tuple(r"^" + r + r"$" for r in _open_port_regexes),
             ),
             (
                 "URL",
-                _url_regexes,
+                tuple(r"^" + r + r"$" for r in _url_regexes),
             ),
         )
     )
 )
 
 event_id_regex = re.compile(r"[0-9a-f]{40}:[A-Z0-9_]+")
 dns_name_regex = re.compile(_dns_name_regex, re.I)
 scan_name_regex = re.compile(r"[a-z]{3,20}_[a-z]{3,20}")
-hostname_regex = re.compile(_hostname_regex, re.I)
+hostname_regex = re.compile(r"^" + _hostname_regex + r"$", re.I)
 
 # For use with extract_params_html helper
 input_tag_regex = re.compile(r"<input[^>]+?name=[\"\'](\w+)[\"\']")
 jquery_get_regex = re.compile(r"url:\s?[\"\'].+?\?(\w+)=")
 jquery_post_regex = re.compile(r"\$.post\([\'\"].+[\'\"].+\{(.+)\}")
 a_tag_regex = re.compile(r"<a[^>]*href=[\"\'][^\"\'?>]*\?([^&\"\'=]+)")
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/url.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/validators.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import ipaddress
 
 from bbot.core.helpers import regexes
 from bbot.core.helpers.url import clean_url
 from bbot.core.helpers.punycode import smart_decode_punycode
 from bbot.core.helpers.misc import split_host_port, make_netloc
 
-log = logging.getLogger("bbot.core.helpers.")
+log = logging.getLogger("bbot.core.helpers.validators")
 
 
 def validator(func):
     """
     Decorator for squashing all errors into ValueError
     """
 
@@ -58,16 +58,14 @@
             # finally, try DNS_NAME
             host = smart_decode_punycode(host)
             # clean asterisks and clinging dashes
             host = host.strip("*.-").replace("*", "")
             for r in regexes.event_type_regexes["DNS_NAME"]:
                 if r.match(host):
                     return host
-            if regexes.hostname_regex.match(host):
-                return host
     assert False, f'Invalid hostname: "{host}"'
 
 
 @validator
 def validate_url(url):
     return validate_url_parsed(url).geturl()
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/web.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import ssl
+import anyio
 import httpx
 import logging
 import traceback
 from pathlib import Path
 from bs4 import BeautifulSoup
 
 from bbot.core.errors import WordlistError, CurlError
@@ -93,14 +94,16 @@
             kwargs["follow_redirects"] = allow_redirects
 
         # in case of URL only, assume GET request
         if len(args) == 1:
             kwargs["url"] = args[0]
             args = []
 
+        url = kwargs.get("url", "")
+
         if not args and "method" not in kwargs:
             kwargs["method"] = "GET"
 
         client_kwargs = {}
         for k in list(kwargs):
             if k in self.client_options:
                 v = kwargs.pop(k)
@@ -113,22 +116,43 @@
                 async with self.web_rate_limiter:
                     response = await client.request(*args, **kwargs)
                 if self.http_debug:
                     log.debug(
                         f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}"
                     )
                 return response
+            except httpx.TimeoutException:
+                log.verbose(f"HTTP timeout to URL: {url}")
+                if raise_error:
+                    raise
+            except httpx.ConnectError:
+                log.verbose(f"HTTP connect failed to URL: {url}")
+                if raise_error:
+                    raise
             except httpx.RequestError as e:
-                log.debug(f"Error with request: {e}")
+                log.trace(f"Error with request to URL: {url}: {e}")
                 log.trace(traceback.format_exc())
                 if raise_error:
                     raise
             except ssl.SSLError as e:
-                log.debug(f"SSL error with request: {e}")
+                msg = f"SSL error with request to URL: {url}: {e}"
+                log.trace(msg)
+                log.trace(traceback.format_exc())
+                if raise_error:
+                    raise httpx.RequestError(msg)
+            except anyio.EndOfStream as e:
+                msg = f"AnyIO error with request to URL: {url}: {e}"
+                log.trace(msg)
+                log.trace(traceback.format_exc())
+                if raise_error:
+                    raise httpx.RequestError(msg)
+            except BaseException as e:
+                log.trace(f"Unhandled exception with request to URL: {url}: {e}")
                 log.trace(traceback.format_exc())
+                raise
 
     async def download(self, url, **kwargs):
         """
         Downloads file, returns full path of filename
         If download failed, returns None
 
         Caching supported via "cache_hrs"
```

### Comparing `bbot-1.1.0.1958rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.0.2024rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/core/logger/logger.py` & `bbot-1.1.0.2024rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/db/neo4j.py` & `bbot-1.1.0.2024rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/defaults.yml` & `bbot-1.1.0.2024rc0/bbot/defaults.yml`

 * *Files 0% similar despite different names*

```diff
@@ -128,12 +128,12 @@
 
 # Custom interactsh server settings
 interactsh_server: null
 interactsh_token: null
 interactsh_disable: false
 
 # For performance reasons, always skip these DNS queries
-# Microsoft's DNS infrastructure is misconfigured so that some queries to mail.protection.outlook.com always time out
+# Microsoft's DNS infrastructure is misconfigured so that certain queries to mail.protection.outlook.com always time out
 dns_omit_queries:
   - SRV:mail.protection.outlook.com
   - CNAME:mail.protection.outlook.com
   - TXT:mail.protection.outlook.com
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/anubisdb.py` & `bbot-1.1.0.2024rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/azure_realm.py` & `bbot-1.1.0.2024rc0/bbot/modules/azure_realm.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,19 @@
     async def handle_event(self, event):
         _, domain = self.helpers.split_domain(event.data)
         domain_hash = hash(domain)
         if domain_hash not in self.processed:
             self.processed.add(domain_hash)
             auth_url = await self.getuserrealm(domain)
             if auth_url:
-                self.emit_event(auth_url, "URL_UNVERIFIED", source=event, tags=["affiliate", "ms-auth-url"])
+                url_event = self.make_event(
+                    auth_url, "URL_UNVERIFIED", source=event, tags=["affiliate", "ms-auth-url"]
+                )
+                url_event.source_domain = domain
+                self.emit_event(url_event)
 
     async def getuserrealm(self, domain):
         url = f"https://login.microsoftonline.com/getuserrealm.srf?login=test@{domain}"
         r = await self.helpers.request(url)
         if r is None:
             return
         try:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.0.2024rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/badsecrets.py` & `bbot-1.1.0.2024rc0/bbot/modules/badsecrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class badsecrets(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
     meta = {"description": "Library for detecting known or weak secrets across many web frameworks"}
     max_event_handlers = 2
-    deps_pip = ["badsecrets~=0.3.351"]
+    deps_pip = ["badsecrets~=0.4"]
 
     @property
     def _max_event_handlers(self):
         return multiprocessing.cpu_count()
 
     async def handle_event(self, event):
         resp_body = event.data.get("body", None)
@@ -29,22 +29,26 @@
                 else:
                     resp_cookies_list = [resp_cookies_raw]
                 for c in resp_cookies_list:
                     c2 = c.lstrip(";").strip().split(";")[0].split("=")
                     if len(c2) == 2:
                         resp_cookies[c2[0]] = c2[1]
         if resp_body or resp_cookies:
-            r_list = await self.scan.run_in_executor_mp(
-                carve_all_modules, body=resp_body, cookies=resp_cookies, url=event.data.get("url", None)
-            )
+            try:
+                r_list = await self.scan.run_in_executor_mp(
+                    carve_all_modules, body=resp_body, cookies=resp_cookies, url=event.data.get("url", None)
+                )
+            except Exception as e:
+                self.warning(f"Error processing {event}: {e}")
+                return
             if r_list:
                 for r in r_list:
                     if r["type"] == "SecretFound":
                         data = {
-                            "severity": "HIGH",
+                            "severity": r["description"]["severity"],
                             "description": f"Known Secret Found. Secret Type: [{r['description']['secret']}] Secret: [{r['secret']}] Product Type: [{r['description']['product']}] Product: [{r['product']}] Detecting Module: [{r['detecting_module']}] Details: [{r['details']}]",
                             "url": event.data["url"],
                             "host": str(event.host),
                         }
                         self.emit_event(data, "VULNERABILITY", event)
                     elif r["type"] == "IdentifyOnly":
                         data = {
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/base.py` & `bbot-1.1.0.2024rc0/bbot/modules/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -210,28 +210,26 @@
         return self._watched_events
 
     async def _handle_batch(self):
         submitted = False
         if self.batch_size <= 1:
             return
         if self.num_incoming_events > 0:
-            events, finish, report = await self.events_waiting()
+            events, finish = await self.events_waiting()
             if not self.errored:
                 self.debug(f"Handling batch of {len(events):,} events")
                 if events:
                     submitted = True
-                    async with self.scan.acatch(context=f"{self.name}.handle_batch"):
-                        with self._task_counter:
-                            await self.handle_batch(*events)
+                    context = "handle_batch()"
+                    async with self.scan.acatch(context), self._task_counter.count(context):
+                        await self.handle_batch(*events)
                 if finish:
-                    async with self.scan.acatch(context=f"{self.name}.finish"):
+                    context = "finish()"
+                    async with self.scan.acatch(context), self._task_counter.count(context):
                         await self.finish()
-                elif report:
-                    async with self.scan.acatch(context=f"{self.name}.report"):
-                        await self.report()
         return submitted
 
     def make_event(self, *args, **kwargs):
         raise_error = kwargs.pop("raise_error", False)
         try:
             event = self.scan.make_event(*args, **kwargs)
         except ValidationError as e:
@@ -256,15 +254,14 @@
 
     async def events_waiting(self):
         """
         yields all events in queue, up to maximum batch size
         """
         events = []
         finish = False
-        report = False
         while self.incoming_event_queue:
             if len(events) > self.batch_size:
                 break
             try:
                 event = self.incoming_event_queue.get_nowait()
                 self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
                 acceptable, reason = await self._event_postcheck(event)
@@ -274,20 +271,20 @@
                     else:
                         events.append(event)
                         self.scan.stats.event_consumed(event, self)
                 elif reason:
                     self.debug(f"Not accepting {event} because {reason}")
             except asyncio.queues.QueueEmpty:
                 break
-        return events, finish, report
+        return events, finish
 
     @property
     def num_incoming_events(self):
         ret = 0
-        if self.incoming_event_queue:
+        if self.incoming_event_queue is not False:
             ret = self.incoming_event_queue.qsize()
         return ret
 
     @property
     def _max_event_handlers(self):
         return self.max_event_handlers
 
@@ -314,49 +311,55 @@
                 status = None
             msg = f"{e}"
             self.trace()
         return self.name, status, str(msg)
 
     async def _worker(self):
         async with self.scan.acatch(context=self._worker):
-            while not self.scan.stopping:
-                # hold the reigns if our outgoing queue is full
-                if self._qsize > 0 and self.outgoing_event_queue.qsize() >= self._qsize:
-                    await asyncio.sleep(0.1)
-                    continue
-
-                if self.batch_size > 1:
-                    submitted = await self._handle_batch()
-                    if not submitted:
-                        async with self._event_received:
-                            await self._event_received.wait()
-
-                else:
-                    try:
-                        if self.incoming_event_queue:
-                            event = await self.incoming_event_queue.get()
-                        else:
-                            self.debug(f"Event queue is in bad state")
-                            return
-                    except asyncio.queues.QueueEmpty:
+            try:
+                while not self.scan.stopping:
+                    # hold the reigns if our outgoing queue is full
+                    if self._qsize > 0 and self.outgoing_event_queue.qsize() >= self._qsize:
+                        await asyncio.sleep(0.1)
                         continue
-                    self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
-                    acceptable, reason = await self._event_postcheck(event)
-                    if not acceptable:
-                        self.debug(f"Not accepting {event} because {reason}")
-                    if acceptable:
-                        if event.type == "FINISHED":
-                            async with self.scan.acatch(context=f"{self.name}.finish"):
-                                with self._task_counter:
+
+                    if self.batch_size > 1:
+                        submitted = await self._handle_batch()
+                        if not submitted:
+                            async with self._event_received:
+                                await self._event_received.wait()
+
+                    else:
+                        try:
+                            if self.incoming_event_queue is not False:
+                                event = await self.incoming_event_queue.get()
+                            else:
+                                self.debug(f"Event queue is in bad state")
+                                break
+                        except asyncio.queues.QueueEmpty:
+                            continue
+                        self.debug(f"Got {event} from {getattr(event, 'module', 'unknown_module')}")
+                        acceptable, reason = await self._event_postcheck(event)
+                        if not acceptable:
+                            self.debug(f"Not accepting {event} because {reason}")
+                        if acceptable:
+                            if event.type == "FINISHED":
+                                context = "finish()"
+                                async with self.scan.acatch(context), self._task_counter.count(context):
                                     await self.finish()
-                        else:
-                            self.scan.stats.event_consumed(event, self)
-                            async with self.scan.acatch(context=f"{self.name}.handle_event"):
-                                with self._task_counter:
+                            else:
+                                context = f"handle_event({event})"
+                                self.scan.stats.event_consumed(event, self)
+                                async with self.scan.acatch(context), self._task_counter.count(context):
                                     await self.handle_event(event)
+            except asyncio.CancelledError:
+                self.log.trace("Worker cancelled")
+                self.trace()
+                raise
+        self.log.trace(f"Worker stopped")
 
     @property
     def max_scope_distance(self):
         if self.in_scope_only or self.target_only:
             return 0
         return max(0, self.scan.scope_search_distance + self.scope_distance_modifier)
 
@@ -445,24 +448,24 @@
         self.debug(f"{event} passed post-check")
         return True, ""
 
     async def _cleanup(self):
         if not self._cleanedup:
             self._cleanedup = True
             for callback in [self.cleanup] + self.cleanup_callbacks:
+                context = f"cleanup()"
                 if callable(callback):
-                    async with self.scan.acatch(context=self.name):
-                        with self._task_counter:
-                            await self.helpers.execute_sync_or_async(callback)
+                    async with self.scan.acatch(context), self._task_counter.count(context):
+                        await self.helpers.execute_sync_or_async(callback)
 
     async def queue_event(self, event):
         """
         Queue (incoming) event with module
         """
-        if self.incoming_event_queue in (None, False):
+        if self.incoming_event_queue is False:
             self.debug(f"Not in an acceptable state to queue incoming event")
             return
         acceptable, reason = self._event_precheck(event)
         if not acceptable:
             if reason and reason != "its type is not in watched_events":
                 self.debug(f"Not accepting {event} because {reason}")
             return
@@ -494,20 +497,21 @@
     def dequeue_outgoing_event_nowait(self):
         return self.outgoing_event_queue.get_nowait()
         with self._event_dequeued:
             self._event_dequeued.notify()
 
     def set_error_state(self, message=None):
         if not self.errored:
+            log_msg = f"Setting error state for module {self.name}"
             if message is not None:
-                self.warning(str(message))
-            self.debug(f"Setting error state for module {self.name}")
+                log_msg += f": {message}"
+            self.warning(log_msg)
             self.errored = True
             # clear incoming queue
-            if self.incoming_event_queue:
+            if self.incoming_event_queue is not False:
                 self.debug(f"Emptying event_queue")
                 with suppress(asyncio.queues.QueueEmpty):
                     while 1:
                         self.incoming_event_queue.get_nowait()
                 # set queue to None to prevent its use
                 # if there are leftover objects in the queue, the scan will hang.
                 self._incoming_event_queue = False
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bevigil.py` & `bbot-1.1.0.2024rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/binaryedge.py` & `bbot-1.1.0.2024rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bucket_aws.py` & `bbot-1.1.0.2024rc0/bbot/modules/bucket_aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             new_buckets = new_buckets - buckets
         new_buckets = [b for b in new_buckets if self.valid_bucket_name(b)]
         tasks = []
         for base_domain in self.base_domains:
             for region in self.regions:
                 for bucket_name in new_buckets:
                     url = self.build_url(bucket_name, base_domain, region)
-                    tasks.append(self.helpers.create_task(self._check_bucket_exists(bucket_name, url)))
-        for task in self.helpers.as_completed(tasks):
+                    tasks.append(self._check_bucket_exists(bucket_name, url))
+        async for task in self.helpers.as_completed(tasks):
             existent_bucket, tags, bucket_name, url = await task
             if existent_bucket:
                 yield bucket_name, url, tags
 
     async def _check_bucket_exists(self, bucket_name, url):
         self.debug(f'Checking if bucket exists: "{bucket_name}"')
         return await self.check_bucket_exists(bucket_name, url)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.0.2024rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.0.2024rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.0.2024rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bucket_gcp.py` & `bbot-1.1.0.2024rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/builtwith.py` & `bbot-1.1.0.2024rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/bypass403.py` & `bbot-1.1.0.2024rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/c99.py` & `bbot-1.1.0.2024rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/censys.py` & `bbot-1.1.0.2024rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/certspotter.py` & `bbot-1.1.0.2024rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/columbus.py` & `bbot-1.1.0.2024rc0/bbot/modules/columbus.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,20 @@
 
 
 class columbus(crobat):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     meta = {"description": "Query the Columbus Project API for subdomains"}
-    options = {"limit": 500}
-    options_desc = {"limit": "Max number of subdomains to retrieve"}
 
     base_url = "https://columbus.elmasy.com/api/lookup"
 
-    async def setup(self):
-        self.limit = self.config.get("limit", 500)
-        return await super().setup()
-
     async def request_url(self, query):
-        url = f"{self.base_url}/{self.helpers.quote(query)}"
+        url = f"{self.base_url}/{self.helpers.quote(query)}?days=365"
         return await self.request_with_fail_count(url)
 
     def parse_results(self, r, query):
         results = set()
         json = r.json()
         if json and isinstance(json, list):
-            return set([f"{s.lower()}.{query}" for s in json[: self.limit]])
+            return set([f"{s.lower()}.{query}" for s in json])
         return results
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/crobat.py` & `bbot-1.1.0.2024rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/crt.py` & `bbot-1.1.0.2024rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.0.2024rc0/bbot/modules/deadly/ffuf.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.debug(f"Using wordlist [{wordlist_url}]")
         self.wordlist = await self.helpers.wordlist(wordlist_url)
         self.wordlist_lines = list(self.helpers.read_file(self.wordlist))
         self.tempfile, tempfile_len = self.generate_templist()
         self.verbose(f"Generated dynamic wordlist with length [{str(tempfile_len)}]")
         try:
             self.extensions = parse_list_string(self.config.get("extensions", ""))
-            self.critical(f"Using custom extensions: [{','.join(self.extensions)}]")
+            self.debug(f"Using custom extensions: [{','.join(self.extensions)}]")
         except ValueError as e:
             self.warning(f"Error parsing extensions: {e}")
             return False
         return True
 
     async def handle_event(self, event):
         if self.helpers.url_depth(event.data) > self.config.get("max_depth"):
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.0.2024rc0/bbot/modules/deadly/nuclei.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "aggressive"]
     meta = {"description": "Fast and customisable vulnerability scanner"}
 
     batch_size = 25
 
     options = {
-        "version": "2.9.4",
+        "version": "2.9.9",
         "tags": "",
         "templates": "",
         "severity": "",
         "ratelimit": 150,
         "concurrency": 25,
         "mode": "manual",
         "etags": "",
@@ -111,15 +111,15 @@
         if self.mode == "budget":
             self.info(
                 f"Running nuclei in BUDGET mode. This mode calculates which nuclei templates can be used, constrained by your 'budget' of number of requests. Current budget is set to: {self.budget}"
             )
 
             self.info("Processing nuclei templates to perform budget calculations...")
 
-            self.nucleibudget = NucleiBudget(self.budget, self.nuclei_templates_dir)
+            self.nucleibudget = NucleiBudget(self)
             self.budget_templates_file = self.helpers.tempfile(self.nucleibudget.collapsable_templates, pipe=False)
 
             self.info(
                 f"Loaded [{str(sum(self.nucleibudget.severity_stats.values()))}] templates based on a budget of [{str(self.budget)}] request(s)"
             )
             self.info(
                 f"Template Severity: Critical [{self.nucleibudget.severity_stats['critical']}] High [{self.nucleibudget.severity_stats['high']}] Medium [{self.nucleibudget.severity_stats['medium']}] Low [{self.nucleibudget.severity_stats['low']}] Info [{self.nucleibudget.severity_stats['info']}] Unknown [{self.nucleibudget.severity_stats['unknown']}]"
@@ -269,19 +269,20 @@
                     f"rejecting URL [{str(event.data)}] because directory_only is true and event has endpoint tag"
                 )
                 return False
         return True
 
 
 class NucleiBudget:
-    def __init__(self, budget, templates_dir):
+    def __init__(self, nuclei_module):
+        self.parent = nuclei_module
         self._yaml_files = {}
-        self.templates_dir = templates_dir
+        self.templates_dir = nuclei_module.nuclei_templates_dir
         self.yaml_list = self.get_yaml_list()
-        self.budget_paths = self.find_budget_paths(budget)
+        self.budget_paths = self.find_budget_paths(nuclei_module.budget)
         self.collapsable_templates, self.severity_stats = self.find_collapsable_templates()
 
     def get_yaml_list(self):
         return list(self.templates_dir.rglob("*.yaml"))
 
     # Given the current budget setting, scan all of the templates for paths, sort them by frequency and select the first N (budget) items
     def find_budget_paths(self, budget):
@@ -360,10 +361,10 @@
     def parse_yaml(self, yamlfile):
         if yamlfile not in self._yaml_files:
             with open(yamlfile, "r") as stream:
                 try:
                     y = yaml.safe_load(stream)
                     self._yaml_files[yamlfile] = y
                 except yaml.YAMLError as e:
-                    self.warning(f"failed to load yaml file: {e}")
+                    self.parent.warning(f"failed to load yaml file: {e}")
                     return {}
         return self._yaml_files[yamlfile]
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.0.2024rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.0.2024rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.0.2024rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.1.0.2024rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/emailformat.py` & `bbot-1.1.0.2024rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.0.2024rc0/bbot/modules/ffuf_shortnames.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if not wordlist_extensions:
             wordlist_extensions = f"{self.helpers.wordlist_dir}/raft-small-extensions-lowercase_CLEANED.txt"
         self.debug(f"Using [{wordlist_extensions}] for shortname candidate extension list")
         self.wordlist_extensions = await self.helpers.wordlist(wordlist_extensions)
 
         try:
             self.extensions = parse_list_string(self.config.get("extensions", ""))
-            self.critical(f"Using custom extensions: [{','.join(self.extensions)}]")
+            self.debug(f"Using custom extensions: [{','.join(self.extensions)}]")
         except ValueError as e:
             self.warning(f"Error parsing extensions: {e}")
             return False
 
         self.ignore_redirects = self.config.get("ignore_redirects")
 
         self.per_host_collection = {}
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.0.2024rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/fullhunt.py` & `bbot-1.1.0.2024rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.0.2024rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/git.py` & `bbot-1.1.0.2024rc0/bbot/modules/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         base_url = event.data.rstrip("/")
         urls = {
             # git config
             urljoin(base_url, ".git/config"),
             urljoin(f"{base_url}/", ".git/config"),
         }
         tasks = [self.get_url(u) for u in urls]
-        for task in self.helpers.as_completed(tasks):
+        async for task in self.helpers.as_completed(tasks):
             result, url = await task
             text = getattr(result, "text", "")
             if not text:
                 text = ""
             if text:
                 if getattr(result, "status_code", 0) == 200 and "[core]" in text and not self.fp_regex.match(text):
                     self.emit_event(
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/github.py` & `bbot-1.1.0.2024rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/gowitness.py` & `bbot-1.1.0.2024rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/hackertarget.py` & `bbot-1.1.0.2024rc0/bbot/modules/hackertarget.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,9 @@
     def parse_results(self, r, query):
         for line in r.text.splitlines():
             host = line.split(",")[0]
             try:
                 self.helpers.validators.validate_host(host)
                 yield host
             except ValueError:
-                self.set_error_state(host)
+                self.debug(f"Error validating API result: {line}")
+                continue
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/host_header.py` & `bbot-1.1.0.2024rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/httpx.py` & `bbot-1.1.0.2024rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/hunt.py` & `bbot-1.1.0.2024rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/hunterio.py` & `bbot-1.1.0.2024rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.0.2024rc0/bbot/modules/iis_shortnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,18 +105,18 @@
 
         tasks = []
         for c in valid_chars:
             suffix = "/a.aspx"
             wildcard = "*" if extension_mode else "*~1*"
             payload = encode_all(f"{prefix}{c}{wildcard}")
             url = f"{target}{payload}{suffix}"
-            task = self.helpers.create_task(self.threaded_request(method, url, affirmative_status_code, c))
+            task = self.threaded_request(method, url, affirmative_status_code, c)
             tasks.append(task)
 
-        for task in self.helpers.as_completed(tasks):
+        async for task in self.helpers.as_completed(tasks):
             result, c = await task
             if result:
                 found_results = True
                 node_count += 1
                 self.verbose(f"node_count: {str(node_count)} for node: {target}")
                 if node_count > self.config.get("max_node_count"):
                     self.warning(
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/internal/base.py` & `bbot-1.1.0.2024rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.0.2024rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.0.2024rc0/bbot/modules/internal/speculate.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         target_len = len(self.scan.target)
         if target_len > self.config.get("max_hosts", 65536):
             if not self.portscanner_enabled:
                 self.hugewarning(
                     f"Selected target ({target_len:,} hosts) is too large, skipping IP_RANGE --> IP_ADDRESS speculation"
                 )
-                self.hugewarning(f"Enabling a port scanner (naabu or masscan) module is highly recommended")
+                self.hugewarning(f"Enabling a port scanner (nmap or masscan) module is highly recommended")
             self.range_to_ip = False
 
         return True
 
     async def handle_event(self, event):
         # generate individual IP addresses from IP range
         if event.type == "IP_RANGE" and self.range_to_ip:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.0.2024rc0/bbot/modules/ipneighbor.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,8 +28,11 @@
         netmask = main_ip.max_prefixlen - min(main_ip.max_prefixlen, self.num_bits)
         network = ipaddress.ip_network(f"{main_ip}/{netmask}", strict=False)
         subnet_hash = hash(network)
         if not subnet_hash in self.processed:
             self.processed.add(subnet_hash)
             for ip in network:
                 if ip != main_ip:
-                    self.emit_event(str(ip), "IP_ADDRESS", event, internal=True)
+                    ip_event = self.make_event(str(ip), "IP_ADDRESS", event, internal=True)
+                    # keep the scope distance low to give it one more hop for DNS resolution
+                    # ip_event.scope_distance = max(1, event.scope_distance)
+                    self.emit_event(ip_event)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/ipstack.py` & `bbot-1.1.0.2024rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/leakix.py` & `bbot-1.1.0.2024rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/masscan.py` & `bbot-1.1.0.2024rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/massdns.py` & `bbot-1.1.0.2024rc0/bbot/modules/massdns.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,42 +115,59 @@
 
     def already_processed(self, hostname):
         if hash(hostname) in self.processed:
             return True
         return False
 
     async def massdns(self, domain, subdomains):
-        abort_msg = f"Aborting massdns on {domain} due to false positives"
-        if await self._canary_check(domain):
-            self.info(abort_msg)
+        subdomains = list(subdomains)
+
+        # before we start, do a canary check for wildcards
+        abort_msg = f"Aborting massdns on {domain} due to false positive"
+        canary_result = await self._canary_check(domain)
+        if canary_result:
+            self.info(abort_msg + f": {canary_result}")
             return []
+
         results = [l async for l in self._massdns(domain, subdomains)]
+
+        # do another canary check for good measure
         if len(results) > 50:
-            if await self._canary_check(domain):
-                self.info(abort_msg)
+            canary_result = await self._canary_check(domain)
+            if canary_result:
+                self.info(abort_msg + f": {canary_result}")
                 return []
+
+        # abort if there are a suspiciously high number of results
+        # (the results are over 2000, and this is more than 20 percent of the input size)
+        if len(results) > 2000 and len(results) / len(subdomains) > 0.2:
+            self.info(
+                f"Aborting because the number of results ({len(results):,}) is suspiciously high for the length of the wordlist ({len(subdomains):,})"
+            )
+            return []
+
+        # everything checks out
         self.verbose(f"Resolving batch of {len(results):,} results")
-        resolved = dict(
-            [l async for l in self.helpers.resolve_batch(results, type=("A", "AAAA", "CNAME"), cache_result=True)]
-        )
+        resolved = dict([l async for l in self.helpers.resolve_batch(results, type=("A", "CNAME"), cache_result=True)])
         resolved = {k: v for k, v in resolved.items() if v}
         for hostname in resolved:
             self.add_found(hostname)
         return list(resolved)
 
-    async def _canary_check(self, domain, num_checks=50):
+    async def _canary_check(self, domain, num_checks=100):
         random_subdomains = list(self.gen_random_subdomains(num_checks))
         self.verbose(f"Testing {len(random_subdomains):,} canaries against {domain}")
         canary_results = [l async for l in self._massdns(domain, random_subdomains)]
-        async for result in self.helpers.resolve_batch(canary_results):
+        resolved_canaries = self.helpers.resolve_batch(canary_results)
+        async for query, result in resolved_canaries:
             if result:
-                return True
-        # for result in canary_results:
-        #     if await self.helpers.resolve(result):
-        #         return True
+                await resolved_canaries.aclose()
+                result = f"{query}:{result}"
+                self.log.trace(f"Found false positive: {result}")
+                return result
         return False
 
     async def _massdns(self, domain, subdomains):
         """
         {
           "name": "www.blacklanternsecurity.com.",
           "type": "A",
@@ -345,16 +362,17 @@
     def gen_random_subdomains(self, n=50):
         delimeters = (".", "-")
         lengths = list(range(10, 20))
         for i in range(0, n):
             d = delimeters[i % len(delimeters)]
             l = lengths[i % len(lengths)]
             segments = list(random.choice(self.devops_mutations) for _ in range(l))
-            subdomains = d.join(segments)
-            yield subdomains
+            segments.append(self.helpers.rand_string(length=8, digits=False))
+            subdomain = d.join(segments)
+            yield subdomain
 
     def get_source_event(self, hostname):
         for p in self.helpers.domain_parents(hostname):
             try:
                 return self.source_events[hash(p)]
             except KeyError:
                 continue
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/myssl.py` & `bbot-1.1.0.2024rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/nmap.py` & `bbot-1.1.0.2024rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/nsec.py` & `bbot-1.1.0.2024rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/ntlm.py` & `bbot-1.1.0.2024rc0/bbot/modules/ntlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,29 +119,29 @@
 
         tasks = []
         for url in urls:
             url_hash = hash(url)
             if url_hash in self.processed:
                 continue
             self.processed.add(url_hash)
-            task = self.helpers.create_task(self.check_ntlm(url))
-            tasks.append(task)
+            tasks.append(self.helpers.create_task(self.check_ntlm(url)))
 
-        for task in self.helpers.as_completed(tasks):
+        gen = self.helpers.as_completed(tasks)
+        async for task in gen:
             try:
                 result, url = await task
                 if result:
                     await self.helpers.cancel_tasks(tasks)
                     return result, url
             except (RequestError, ReadTimeout) as e:
                 if str(e):
                     self.warning(str(e))
                 # cancel all the tasks if there's an error
                 await self.helpers.cancel_tasks(tasks)
-                break
+                await gen.aclose()
 
         return None, None
 
     async def check_ntlm(self, test_url):
         # use lower timeout value
         http_timeout = self.config.get("httpx_timeout", 5)
         r = await self.helpers.request(
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/oauth.py` & `bbot-1.1.0.2024rc0/bbot/modules/oauth.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,46 +45,54 @@
         oauth_tasks = []
         if self.try_all or any(t in event.tags for t in ("oauth-token-endpoint",)):
             oauth_tasks.append(self.helpers.create_task(self.getoauth(url)))
         if self.try_all or any(t in event.tags for t in ("ms-auth-url",)):
             for u in self.url_and_base(url):
                 oidc_tasks.append(self.helpers.create_task(self.getoidc(u)))
 
+        source_domain = getattr(event, "source_domain", domain)
+
         for oidc_task in oidc_tasks:
             url, token_endpoint, oidc_results = await oidc_task
             if token_endpoint:
-                self.emit_event(
+                finding_event = self.make_event(
                     {
-                        "description": f"OpenID Connect Endpoint found at {url}",
+                        "description": f"OpenID Connect Endpoint (domain: {source_domain}) found at {url}",
                         "host": event.host,
                         "url": url,
                     },
                     "FINDING",
                     source=event,
                 )
-                self.emit_event(
+                finding_event.source_domain = source_domain
+                self.emit_event(finding_event)
+                url_event = self.make_event(
                     token_endpoint, "URL_UNVERIFIED", source=event, tags=["affiliate", "oauth-token-endpoint"]
                 )
+                url_event.source_domain = source_domain
+                self.emit_event(url_event)
             for result in oidc_results:
                 if result not in (domain, event.data):
                     event_type = "URL_UNVERIFIED" if self.helpers.is_url(result) else "DNS_NAME"
                     self.emit_event(result, event_type, source=event, tags=["affiliate"])
 
         for oauth_task in oauth_tasks:
             url = await oauth_task
             if url:
-                self.emit_event(
+                oauth_finding = self.make_event(
                     {
-                        "description": f"Potentially Sprayable OAUTH Endpoint at {url}",
+                        "description": f"Potentially Sprayable OAUTH Endpoint (domain: {source_domain}) at {url}",
                         "host": event.host,
                         "url": url,
                     },
                     "FINDING",
                     source=event,
                 )
+                oauth_finding.source_domain = source_domain
+                self.emit_event(oauth_finding)
 
     def url_and_base(self, url):
         yield url
         parsed = self.helpers.urlparse(url)
         baseurl = f"{parsed.scheme}://{parsed.netloc}/"
         if baseurl != url:
             yield baseurl
@@ -111,15 +119,15 @@
         results -= {token_endpoint}
         return url, token_endpoint, results
 
     async def getoauth(self, url):
         data = {
             "grant_type": "authorization_code",
             "client_id": "xxx",
-            "redirect_uri": "https://www.blacklanternsecurity.com",
+            "redirect_uri": "https://example.com",
             "code": "xxx",
             "client_secret": "xxx",
         }
         url_hash = hash("OAUTH:" + url)
         if url_hash not in self.processed:
             self.processed.add(url_hash)
             r = await self.helpers.request(url, method="POST", data=data)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/otx.py` & `bbot-1.1.0.2024rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/asset_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         for asset in sorted(self.assets.values(), key=sort_key):
             findings_and_vulns = asset.findings.union(asset.vulnerabilities)
             ports = getattr(asset, "ports", set())
             ports = [str(p) for p in sorted([int(p) for p in asset.ports])]
             ips = sorted([str(i) for i in getattr(asset, "ip_addresses", [])])
             host = getattr(asset, "host", "")
-            if host:
+            if host and isinstance(host, str):
                 _, domain = self.helpers.split_domain(host)
                 if domain:
                     increment_stat("Domains", domain)
             for ip in ips:
                 net = ipaddress.ip_network(f"{ip}/{self.summary_netmask}", strict=False)
                 increment_stat("IP Addresses", str(net))
             for port in ports:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/base.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/csv.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/http.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/human.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/json.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/web_report.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/output/websocket.py` & `bbot-1.1.0.2024rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.0.2024rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.0.2024rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.0.2024rc0/bbot/modules/paramminer_headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,35 +72,41 @@
     max_event_handlers = 12
     in_scope_only = True
     compare_mode = "header"
     default_wordlist = "paramminer_headers.txt"
 
     async def setup(self):
         self.event_dict = {}
+        self.already_checked = set()
         wordlist = self.config.get("wordlist", "")
         if not wordlist:
             wordlist = f"{self.helpers.wordlist_dir}/{self.default_wordlist}"
         self.debug(f"Using wordlist: [{wordlist}]")
         self.wl = set(
             h.strip().lower()
             for h in self.helpers.read_file(await self.helpers.wordlist(wordlist))
             if len(h) > 0 and "%" not in h
         )
 
         # check against the boring list (if the option is set)
 
         if self.config.get("skip_boring_words", True):
             self.wl -= self.boring_words
-        self.matched_words = {}
+        self.extracted_words_master = set()
         return True
 
     def rand_string(self, *args, **kwargs):
         return self.helpers.rand_string(*args, **kwargs)
 
     async def do_mining(self, wl, url, batch_size, compare_helper):
+        for i in wl:
+            if i not in self.wl:
+                h = hash(i + url)
+                self.already_checked.add(h)
+
         results = set()
         abort_threshold = 15
         try:
             for group in self.helpers.grouper(wl, batch_size):
                 async for result, reasons, reflection in self.binary_search(compare_helper, url, group):
                     results.add((result, ",".join(reasons), reflection))
                     if len(results) >= abort_threshold:
@@ -151,19 +157,24 @@
             return
 
         wl = set(self.wl)
         if self.config.get("http_extract"):
             extracted_words = self.load_extracted_words(event.data.get("body"), event.data.get("content_type"))
             if extracted_words:
                 self.debug(f"Extracted {str(len(extracted_words))} words from {url}")
-                self.matched_words[url] = extracted_words
+                self.extracted_words_master.update(extracted_words - wl)
                 wl |= extracted_words
+
         if self.config.get("skip_boring_words", True):
             wl -= self.boring_words
-        results = await self.do_mining(wl, url, batch_size, compare_helper)
+
+        try:
+            results = await self.do_mining(wl, url, batch_size, compare_helper)
+        except HttpCompareError as e:
+            self.debug(f"Encountered HttpCompareError: [{e}] for URL [{event.data}]")
         self.process_results(event, results)
 
     async def count_test(self, url):
         baseline = await self.helpers.request(url)
         if baseline is None:
             return
         if str(baseline.status_code)[0] in ("4", "5"):
@@ -213,25 +224,27 @@
         rand = self.rand_string()
         test_headers = {}
         for header in header_list:
             test_headers[header] = rand
         return await compare_helper.compare(url, headers=test_headers, check_reflection=(len(header_list) == 1))
 
     async def finish(self):
-        for url, (event, batch_size) in self.event_dict.items():
+        untested_matches = self.extracted_words_master.copy()
+        if self.config.get("skip_boring_words", True):
+            untested_matches -= self.boring_words
+
+        for url, (event, batch_size) in list(self.event_dict.items()):
             try:
                 compare_helper = self.helpers.http_compare(url)
             except HttpCompareError as e:
                 self.debug(f"Error initializing compare helper: {e}")
                 return
-            untested_matches = set()
-            for k, s in self.matched_words.items():
-                if k != url:
-                    untested_matches.update(s)
-
-            untested_matches -= self.wl
-
-            if self.config.get("skip_boring_words", True):
-                untested_matches -= self.boring_words
-
-            results = await self.do_mining(untested_matches, url, batch_size, compare_helper)
+            untested_matches_copy = untested_matches.copy()
+            for i in untested_matches:
+                h = hash(i + url)
+                if h in self.already_checked:
+                    untested_matches_copy.remove(i)
+            try:
+                results = await self.do_mining(untested_matches_copy, url, batch_size, compare_helper)
+            except HttpCompareError as e:
+                self.debug(f"Encountered HttpCompareError: [{e}] for URL [{url}]")
             self.process_results(event, results)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/passivetotal.py` & `bbot-1.1.0.2024rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/pgp.py` & `bbot-1.1.0.2024rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/rapiddns.py` & `bbot-1.1.0.2024rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.0.2024rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/report/asn.py` & `bbot-1.1.0.2024rc0/bbot/modules/report/asn.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
             "name": "unknown",
             "description": "unknown",
             "country": "",
         }
         return True
 
     async def filter_event(self, event):
+        if str(event.module) == "ipneighbor":
+            return False
         if getattr(event.host, "is_private", False):
             return False
         return True
 
     async def handle_event(self, event):
         host = event.host
         if self.cache_get(host) == False:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/riddler.py` & `bbot-1.1.0.2024rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/robots.py` & `bbot-1.1.0.2024rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/secretsdb.py` & `bbot-1.1.0.2024rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/securitytrails.py` & `bbot-1.1.0.2024rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.0.2024rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/skymem.py` & `bbot-1.1.0.2024rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/smuggler.py` & `bbot-1.1.0.2024rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/social.py` & `bbot-1.1.0.2024rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/sslcert.py` & `bbot-1.1.0.2024rc0/bbot/modules/sslcert.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,20 +59,16 @@
         if event.scope_distance == 0:
             abort_threshold = self.in_scope_abort_threshold
             log_fn = self.info
         else:
             abort_threshold = self.out_of_scope_abort_threshold
             log_fn = self.verbose
 
-        tasks = []
-        for host in hosts:
-            task = self.helpers.create_task(self.visit_host(host, port))
-            tasks.append(task)
-
-        for task in self.helpers.as_completed(tasks):
+        tasks = [self.visit_host(host, port) for host in hosts]
+        async for task in self.helpers.as_completed(tasks):
             result = await task
             if not isinstance(result, tuple) or not len(result) == 3:
                 continue
             dns_names, emails, (host, port) = result
             if len(dns_names) > abort_threshold:
                 netloc = self.helpers.make_netloc(host, port)
                 log_fn(
@@ -146,16 +142,24 @@
             try:
                 ssl_object = transport.get_extra_info("ssl_object")
             except Exception as e:
                 self.verbose(f"Error getting ssl_object: {e}", trace=True)
                 return [], [], (host, port)
 
             # Get the certificate
-            der = ssl_object.getpeercert(binary_form=True)
-            cert = crypto.load_certificate(crypto.FILETYPE_ASN1, der)
+            try:
+                der = ssl_object.getpeercert(binary_form=True)
+            except Exception as e:
+                self.verbose(f"Error getting peer cert: {e}", trace=True)
+                return [], [], (host, port)
+            try:
+                cert = crypto.load_certificate(crypto.FILETYPE_ASN1, der)
+            except Exception as e:
+                self.verbose(f"Error loading certificate: {e}", trace=True)
+                return [], [], (host, port)
             issuer = cert.get_issuer()
             if issuer.emailAddress and self.helpers.regexes.email_regex.match(issuer.emailAddress):
                 emails.add(issuer.emailAddress)
             subject = cert.get_subject()
             if subject.emailAddress and self.helpers.regexes.email_regex.match(subject.emailAddress):
                 emails.add(subject.emailAddress)
             common_name = str(subject.commonName).lstrip("*.").lower()
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.1.0.2024rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/telerik.py` & `bbot-1.1.0.2024rc0/bbot/modules/telerik.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,16 @@
                                 break
 
         tasks = []
         for dh in self.DialogHandlerUrls:
             tasks.append(self.helpers.create_task(self.test_detector(event.data, f"{dh}?dp=1")))
 
         fail_count = 0
-        for task in self.helpers.as_completed(tasks):
+        gen = self.helpers.as_completed(tasks)
+        async for task in gen:
             try:
                 result, dh = await task
             except asyncio.CancelledError:
                 continue
 
             # cancel if we run into timeouts etc.
             if result is None:
@@ -236,15 +237,15 @@
                     description = f"Telerik DialogHandler detected"
                     self.emit_event(
                         {"host": str(event.host), "url": f"{event.data}{dh}", "description": description},
                         "FINDING",
                         event,
                     )
                     # Once we have a match we need to stop, because the basic handler (Telerik.Web.UI.DialogHandler.aspx) usually works with a path wildcard
-                    break
+                    await gen.aclose()
 
         await self.helpers.cancel_tasks(tasks)
 
         spellcheckhandler = "Telerik.Web.UI.SpellCheckHandler.axd"
         result, _ = await self.test_detector(event.data, spellcheckhandler)
         try:
             # The standard behavior for the spellcheck handler without parameters is a 500
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/threatminer.py` & `bbot-1.1.0.2024rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.0.2024rc0/bbot/modules/url_manipulation.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,23 +43,26 @@
             compare_helper = self.helpers.http_compare(
                 event.data, allow_redirects=self.allow_redirects, include_cache_buster=False
             )
         except HttpCompareError as e:
             self.debug(e)
             return
 
-        if compare_helper.canary_check(event.data, mode="getparam") == False:
+        if await compare_helper.canary_check(event.data, mode="getparam") == False:
             self.verbose(f'Aborting "{event.data}" due to failed canary check')
             return
 
         for sig in self.signatures:
             sig = self.format_signature(sig, event)
-            match, reasons, reflection, subject_response = await compare_helper.compare(
-                sig[1], method=sig[0], allow_redirects=self.allow_redirects
-            )
+            try:
+                match, reasons, reflection, subject_response = await compare_helper.compare(
+                    sig[1], method=sig[0], allow_redirects=self.allow_redirects
+                )
+            except HttpCompareError as e:
+                self.debug(f"Encountered HttpCompareError: [{e}] for URL [{event.data}]")
 
             if subject_response:
                 subject_content = "".join([str(x) for x in subject_response.headers])
                 if subject_response.text != None:
                     subject_content += subject_response.text
 
                 if self.rand_string not in subject_content:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/urlscan.py` & `bbot-1.1.0.2024rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/viewdns.py` & `bbot-1.1.0.2024rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/virustotal.py` & `bbot-1.1.0.2024rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/wafw00f.py` & `bbot-1.1.0.2024rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.0.2024rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/wayback.py` & `bbot-1.1.0.2024rc0/bbot/modules/wayback.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 
     async def query(self, query):
         results = set()
         waybackurl = f"{self.base_url}/cdx/search/cdx?url={self.helpers.quote(query)}&matchType=domain&output=json&fl=original&collapse=original"
         r = await self.helpers.request(waybackurl, timeout=self.http_timeout + 10)
         if not r:
             self.warning(f'Error connecting to archive.org for query "{query}"')
-            return
+            return results
         try:
             j = r.json()
             assert type(j) == list
         except Exception:
             self.warning(f'Error JSON-decoding archive.org response for query "{query}"')
-            return
+            return results
 
         urls = []
         for result in j[1:]:
             try:
                 url = result[0]
                 urls.append(url)
             except KeyError:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/modules/zoomeye.py` & `bbot-1.1.0.2024rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.0.2024rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/scanner/manager.py` & `bbot-1.1.0.2024rc0/bbot/scanner/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,32 +30,32 @@
         self._incoming_queues = None
         self._module_priority_weights = None
 
     async def init_events(self):
         """
         seed scanner with target events
         """
-        async with self.scan.acatch(context=self.init_events):
-            with self._task_counter:
-                await self.distribute_event(self.scan.root_event)
-                sorted_events = sorted(self.scan.target.events, key=lambda e: len(e.data))
-                for event in sorted_events:
-                    self.scan.verbose(f"Target: {event}")
-                    self.queue_event(event)
-                await asyncio.sleep(0.1)
-                self.scan._finished_init = True
+        context = f"manager.init_events()"
+        async with self.scan.acatch(context), self._task_counter.count(context):
+            await self.distribute_event(self.scan.root_event)
+            sorted_events = sorted(self.scan.target.events, key=lambda e: len(e.data))
+            for event in sorted_events:
+                self.scan.verbose(f"Target: {event}")
+                self.queue_event(event)
+            await asyncio.sleep(0.1)
+            self.scan._finished_init = True
 
     async def emit_event(self, event, *args, **kwargs):
         """
         TODO: Register + kill duplicate events immediately?
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         bbot.scanner: scan._event_thread_pool: running for 0 seconds: ScanManager._emit_event(DNS_NAME("sipfed.online.lync.com"))
         """
-        with self._task_counter:
+        async with self._task_counter.count(f"emit_event({event})"):
             # skip event if it fails precheck
             if not self._event_precheck(event):
                 event._resolved.set()
                 return
 
             log.debug(f'Module "{event.module}" raised {event}')
 
@@ -78,15 +78,15 @@
         """
         if event._dummy:
             log.warning(f"Cannot emit dummy event: {event}")
             return False
         if event == event.get_source():
             log.debug(f"Skipping event with self as source: {event}")
             return False
-        if not event._force_output and self.is_duplicate_event(event):
+        if self.is_duplicate_event(event) and not event._force_output:
             log.debug(f"Skipping {event} because it is a duplicate")
             return False
         return True
 
     async def _emit_event(self, event, *args, **kwargs):
         log.debug(f"Emitting {event}")
         distribute_event = True
@@ -157,15 +157,15 @@
             # Cloud tagging
             for provider in self.scan.helpers.cloud.providers.values():
                 provider.tag_event(event)
 
             event_is_duplicate = self.is_duplicate_event(event)
 
             # Scope shepherding
-            # here, we buff or nerf an event based on its attributes and certain scan settings
+            # here, we buff or nerf the scope distance of an event based on its attributes and certain scan settings
             event_is_duplicate = self.is_duplicate_event(event)
             event_in_report_distance = event.scope_distance <= self.scan.scope_report_distance
             set_scope_distance = event.scope_distance
             if event_whitelisted:
                 set_scope_distance = 0
             if event.host:
                 # here, we evaluate some weird logic
@@ -175,15 +175,15 @@
                 event_is_duplicate = event_is_duplicate and not event._force_output
                 if event_will_be_output and not event_is_duplicate:
                     if set_scope_distance == 0:
                         log.debug(f"Making {event} in-scope")
                     source_trail = event.set_scope_distance(set_scope_distance)
                     # force re-emit internal source events
                     for s in source_trail:
-                        await self.emit_event(s, _block=False, _force_submit=True)
+                        self.queue_event(s)
                 else:
                     if event.scope_distance > self.scan.scope_report_distance:
                         log.debug(
                             f"Making {event} internal because its scope_distance ({event.scope_distance}) > scope_report_distance ({self.scan.scope_report_distance})"
                         )
                         event.make_internal()
 
@@ -311,18 +311,14 @@
     def accept_event(self, event):
         is_duplicate = self.is_duplicate_event(event, add=True)
         if is_duplicate and not event._force_output:
             log.debug(f"{event.module}: not raising duplicate event {event}")
             return False
         return True
 
-    async def _register_running(self, callback, *args, **kwargs):
-        with self._task_counter:
-            return await callback(*args, **kwargs)
-
     async def distribute_event(self, *args, **kwargs):
         """
         Queue event with modules
         """
         async with self.scan.acatch(context=self.distribute_event):
             event = self.scan.make_event(*args, **kwargs)
 
@@ -437,14 +433,23 @@
                 with suppress(Exception):
                     mod.set_error_state()
 
         status["finished"] = finished
 
         modules_errored = [m for m, s in status["modules"].items() if s["errored"]]
 
+        max_mem_percent = 90
+        mem_status = self.scan.helpers.memory_status()
+        # abort if we don't have the memory
+        mem_percent = mem_status.percent
+        if mem_percent > max_mem_percent:
+            free_memory = mem_status.available
+            free_memory_human = self.scan.helpers.bytes_to_human(free_memory)
+            self.scan.warning(f"System memory is at {mem_percent:.1f}% ({free_memory_human} remaining)")
+
         if _log:
             modules_status = []
             for m, s in status["modules"].items():
                 running = s["running"]
                 incoming = s["events"]["incoming"]
                 outgoing = s["events"]["outgoing"]
                 tasks = s["tasks"]
@@ -452,14 +457,16 @@
                 if running or total > 0:
                     modules_status.append((m, running, incoming, outgoing, tasks, total))
             modules_status.sort(key=lambda x: x[-1], reverse=True)
 
             if modules_status:
                 modules_status_str = ", ".join([f"{m}({i:,}:{t:,}:{o:,})" for m, r, i, o, t, _ in modules_status])
                 running_modules_str = ", ".join([m[0] for m in modules_status if m[1]])
+                if not running_modules_str:
+                    running_modules_str = "None"
                 self.scan.info(f"{self.scan.name}: Modules running: {running_modules_str}")
                 self.scan.verbose(
                     f"{self.scan.name}: Modules status (incoming:processing:outgoing) {modules_status_str}"
                 )
             event_type_summary = sorted(
                 self.scan.stats.events_emitted_by_type.items(), key=lambda x: x[-1], reverse=True
             )
@@ -489,24 +496,32 @@
             if self.scan.log_level <= logging.DEBUG:
                 # status debugging
                 scan_active_status = []
                 scan_active_status.append(f"scan._finished_init: {self.scan._finished_init}")
                 scan_active_status.append(f"manager.active: {self.active}")
                 scan_active_status.append(f"    manager.running: {self.running}")
                 scan_active_status.append(f"        manager._task_counter.value: {self._task_counter.value}")
+                scan_active_status.append(f"        manager._task_counter.tasks:")
+                for task in self._task_counter.tasks.values():
+                    scan_active_status.append(f"            - {task}:")
                 scan_active_status.append(
-                    f"        manager.incoming_event_queue.qsize(): {self.incoming_event_queue.qsize()}"
+                    f"        manager.incoming_event_queue.qsize: {self.incoming_event_queue.qsize()}"
                 )
                 scan_active_status.append(f"    manager.modules_finished: {self.modules_finished}")
-                for m in self.scan.modules.values():
+                for m in sorted(self.scan.modules.values(), key=lambda m: m.name):
+                    running = m.running
                     scan_active_status.append(f"        {m}.finished: {m.finished}")
-                    scan_active_status.append(f"            running: {m.running}")
+                    scan_active_status.append(f"            running: {running}")
+                    if running:
+                        scan_active_status.append(f"            tasks:")
+                        for task in m._task_counter.tasks.values():
+                            scan_active_status.append(f"                - {task}:")
                     scan_active_status.append(f"            num_incoming_events: {m.num_incoming_events}")
                     scan_active_status.append(
-                        f"            outgoing_event_queue.qsize(): {m.outgoing_event_queue.qsize()}"
+                        f"            outgoing_event_queue.qsize: {m.outgoing_event_queue.qsize()}"
                     )
                 for line in scan_active_status:
                     self.scan.debug(line)
 
                 # log module memory usage
                 module_memory_usage = []
                 for module in self.scan.modules.values():
```

### Comparing `bbot-1.1.0.1958rc0/bbot/scanner/scanner.py` & `bbot-1.1.0.2024rc0/bbot/scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             while 1:
                 # abort if we're aborting
                 if self.aborting:
                     self.drain_queues()
                     break
 
                 if "python" in self.modules:
-                    events, finish, report = await self.modules["python"].events_waiting()
+                    events, finish = await self.modules["python"].events_waiting()
                     for e in events:
                         yield e
 
                 # if initialization finished and the scan is no longer active
                 if self._finished_init and not self.manager.active:
                     new_activity = await self.finish()
                     if not new_activity:
@@ -323,15 +323,15 @@
 
     async def setup_modules(self, remove_failed=True):
         await self.load_modules()
         self.verbose(f"Setting up modules")
         hard_failed = []
         soft_failed = []
 
-        for task in asyncio.as_completed([asyncio.create_task(m._setup()) for m in self.modules.values()]):
+        async for task in self.helpers.as_completed([m._setup() for m in self.modules.values()]):
             module_name, status, msg = await task
             if status == True:
                 self.debug(f"Setup succeeded for {module_name} ({msg})")
             elif status == False:
                 self.error(f"Setup hard-failed for {module_name}: {msg}")
                 self.modules[module_name].set_error_state()
                 hard_failed.append(module_name)
@@ -413,17 +413,17 @@
         tasks += self.manager_worker_loop_tasks
         self.helpers.cancel_tasks_sync(tasks)
         # process pool
         self.process_pool.shutdown(cancel_futures=True)
 
     async def report(self):
         for mod in self.modules.values():
-            async with self.acatch(context=mod.report):
-                with mod._task_counter:
-                    await mod.report()
+            context = f"{mod.name}.report()"
+            async with self.acatch(context), mod._task_counter.count(context):
+                await mod.report()
 
     async def cleanup(self):
         # clean up modules
         self.status = "CLEANING_UP"
         for mod in self.modules.values():
             await mod._cleanup()
         if not self._cleanedup:
```

### Comparing `bbot-1.1.0.1958rc0/bbot/scanner/stats.py` & `bbot-1.1.0.2024rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/scanner/target.py` & `bbot-1.1.0.2024rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/scripts/docs.py` & `bbot-1.1.0.2024rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.0.2024rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/conftest.py` & `bbot-1.1.0.2024rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/run_tests.sh` & `bbot-1.1.0.2024rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test.conf` & `bbot-1.1.0.2024rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_events.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -245,24 +245,24 @@
 
     # punycode
     assert scan.make_event("ドメイン.テスト", dummy=True).type == "DNS_NAME"
     assert scan.make_event("bob@ドメイン.テスト", dummy=True).type == "EMAIL_ADDRESS"
     assert scan.make_event("ドメイン.テスト:80", dummy=True).type == "OPEN_TCP_PORT"
     assert scan.make_event("http://ドメイン.テスト:80", dummy=True).type == "URL_UNVERIFIED"
 
-    assert scan.make_event("xn--eckwd4c7c.xn--zckzah", dummy=True).type == "DNS_NAME"
-    assert scan.make_event("bob@xn--eckwd4c7c.xn--zckzah", dummy=True).type == "EMAIL_ADDRESS"
-    assert scan.make_event("xn--eckwd4c7c.xn--zckzah:80", dummy=True).type == "OPEN_TCP_PORT"
-    assert scan.make_event("http://xn--eckwd4c7c.xn--zckzah:80", dummy=True).type == "URL_UNVERIFIED"
-
     assert scan.make_event("xn--eckwd4c7c.xn--zckzah", dummy=True).data == "ドメイン.テスト"
     assert scan.make_event("bob@xn--eckwd4c7c.xn--zckzah", dummy=True).data == "bob@ドメイン.テスト"
     assert scan.make_event("xn--eckwd4c7c.xn--zckzah:80", dummy=True).data == "ドメイン.テスト:80"
     assert scan.make_event("http://xn--eckwd4c7c.xn--zckzah:80", dummy=True).data == "http://ドメイン.テスト/"
 
+    assert scan.make_event("xn--eckwd4c7c.xn--zckzah", dummy=True).type == "DNS_NAME"
+    assert scan.make_event("bob@xn--eckwd4c7c.xn--zckzah", dummy=True).type == "EMAIL_ADDRESS"
+    assert scan.make_event("xn--eckwd4c7c.xn--zckzah:80", dummy=True).type == "OPEN_TCP_PORT"
+    assert scan.make_event("http://xn--eckwd4c7c.xn--zckzah:80", dummy=True).type == "URL_UNVERIFIED"
+
     # test event serialization
     from bbot.core.event import event_from_json
 
     db_event = scan.make_event("127.0.0.1", dummy=True)
     db_event.scope_distance = 1
     timestamp = db_event.timestamp.timestamp()
     json_event = db_event.json()
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import datetime
 import ipaddress
 
 from ..bbot_fixtures import *
 
 
 @pytest.mark.asyncio
@@ -336,16 +337,18 @@
     assert type(helpers.make_date()) == str
 
     # punycode
     assert helpers.smart_encode_punycode("ドメイン.テスト") == "xn--eckwd4c7c.xn--zckzah"
     assert helpers.smart_decode_punycode("xn--eckwd4c7c.xn--zckzah") == "ドメイン.テスト"
     assert helpers.smart_encode_punycode("evilcorp.com") == "evilcorp.com"
     assert helpers.smart_decode_punycode("evilcorp.com") == "evilcorp.com"
-    assert helpers.smart_encode_punycode("bob@ドメイン.テスト") == "bob@xn--eckwd4c7c.xn--zckzah"
-    assert helpers.smart_decode_punycode("bob@xn--eckwd4c7c.xn--zckzah") == "bob@ドメイン.テスト"
+    assert helpers.smart_encode_punycode("bob_smith@ドメイン.テスト") == "bob_smith@xn--eckwd4c7c.xn--zckzah"
+    assert helpers.smart_decode_punycode("bob_smith@xn--eckwd4c7c.xn--zckzah") == "bob_smith@ドメイン.テスト"
+    assert helpers.smart_encode_punycode("ドメイン.テスト:80") == "xn--eckwd4c7c.xn--zckzah:80"
+    assert helpers.smart_decode_punycode("xn--eckwd4c7c.xn--zckzah:80") == "ドメイン.テスト:80"
     with pytest.raises(ValueError):
         helpers.smart_decode_punycode(b"asdf")
     with pytest.raises(ValueError):
         helpers.smart_encode_punycode(b"asdf")
 
     assert helpers.recursive_decode("Hello%20world%21") == "Hello world!"
     assert helpers.recursive_decode("Hello%20%5Cu041f%5Cu0440%5Cu0438%5Cu0432%5Cu0435%5Cu0442") == "Hello Привет"
@@ -578,16 +581,19 @@
     # sleep for 5 seconds
     await asyncio.sleep(5)
     await helpers.cancel_tasks(tasks)
     # 5 seconds * 10 requests per second == 50
     assert 45 <= len(results) <= 55
 
 
-def test_async_helpers():
+@pytest.mark.asyncio
+async def test_async_helpers():
+    import random
     from bbot.core.helpers.async_helpers import async_to_sync_gen
+    from bbot.core.helpers.misc import as_completed
 
     # async to sync generator converter
     async def async_gen():
         for i in range(5):
             yield i
 
     sync_gen = async_to_sync_gen(async_gen())
@@ -596,14 +602,26 @@
     while 1:
         try:
             l.append(next(sync_gen))
         except StopIteration:
             break
     assert l == [0, 1, 2, 3, 4]
 
+    async def do_stuff(r):
+        await asyncio.sleep(r)
+        return r
+
+    random_ints = [random.random() for _ in range(1000)]
+    tasks = [do_stuff(r) for r in random_ints]
+    results = set()
+    async for t in as_completed(tasks):
+        results.add(await t)
+    assert len(results) == 1000
+    assert sorted(random_ints) == sorted(results)
+
 
 # test parse_port_string helper
 
 
 def test_portparse_singleports(helpers):
     assert helpers.parse_port_string("80,443,22") == [80, 443, 22]
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .base import ModuleTestBase
 
 
 class TestColumbus(ModuleTestBase):
     async def setup_after_prep(self, module_test):
         module_test.httpx_mock.add_response(
-            url=f"https://columbus.elmasy.com/api/lookup/blacklanternsecurity.com",
+            url=f"https://columbus.elmasy.com/api/lookup/blacklanternsecurity.com?days=365",
             json=["asdf", "zzzz"],
         )
 
     def check(self, module_test, events):
         assert any(e.data == "asdf.blacklanternsecurity.com" for e in events), "Failed to detect subdomain"
         assert any(e.data == "zzzz.blacklanternsecurity.com" for e in events), "Failed to detect subdomain"
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base import ModuleTestBase
 
-from .test_module_azure_realm import TestAzure_Realm
+from .test_module_azure_realm import TestAzure_Realm as Azure_Realm
 
 
 class TestOAUTH(ModuleTestBase):
     targets = ["evilcorp.com"]
     config_overrides = {"scope_report_distance": 1, "omit_event_types": []}
     modules_overrides = ["azure_realm", "oauth"]
     openid_config_azure = {
@@ -163,15 +163,15 @@
             "ES512",
         ],
     }
 
     async def setup_after_prep(self, module_test):
         module_test.httpx_mock.add_response(
             url=f"https://login.microsoftonline.com/getuserrealm.srf?login=test@evilcorp.com",
-            json=TestAzure_Realm.response_json,
+            json=Azure_Realm.response_json,
         )
         module_test.httpx_mock.add_response(
             url="https://login.windows.net/evilcorp.com/.well-known/openid-configuration",
             json=self.openid_config_azure,
         )
         module_test.httpx_mock.add_response(
             url="https://evilcorp.okta.com/.well-known/openid-configuration",
@@ -202,29 +202,29 @@
             status_code=400,
         )
 
     def check(self, module_test, events):
         assert any(
             e.type == "FINDING"
             and e.data["description"]
-            == "OpenID Connect Endpoint found at https://login.windows.net/evilcorp.com/.well-known/openid-configuration"
+            == "OpenID Connect Endpoint (domain: evilcorp.com) found at https://login.windows.net/evilcorp.com/.well-known/openid-configuration"
             for e in events
         )
         assert any(
             e.type == "FINDING"
             and e.data["description"]
-            == "OpenID Connect Endpoint found at https://evilcorp.okta.com/.well-known/openid-configuration"
+            == "OpenID Connect Endpoint (domain: evilcorp.com) found at https://evilcorp.okta.com/.well-known/openid-configuration"
             for e in events
         )
         assert any(
             e.type == "FINDING"
             and e.data["description"]
-            == "Potentially Sprayable OAUTH Endpoint at https://login.windows.net/cc74fc12-4142-400e-a653-f98bdeadbeef/oauth2/token"
+            == "Potentially Sprayable OAUTH Endpoint (domain: evilcorp.com) at https://login.windows.net/cc74fc12-4142-400e-a653-f98bdeadbeef/oauth2/token"
             for e in events
         )
         assert any(
             e.type == "FINDING"
             and e.data["description"]
-            == "Potentially Sprayable OAUTH Endpoint at https://evilcorp.okta.com/oauth2/v1/token"
+            == "Potentially Sprayable OAUTH Endpoint (domain: evilcorp.com) at https://evilcorp.okta.com/oauth2/v1/token"
             for e in events
         )
         assert any(e.data == "sts.windows.net" for e in events)
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .test_module_paramminer_headers import *
+from .test_module_paramminer_headers import Paramminer_Headers, tempwordlist, helper
 
 
-class TestParamminer_Cookies(TestParamminer_Headers):
+class TestParamminer_Cookies(Paramminer_Headers):
     modules_overrides = ["httpx", "paramminer_cookies"]
     config_overrides = {"modules": {"paramminer_cookies": {"wordlist": tempwordlist(["junkcookie", "admincookie"])}}}
 
     cookies_body = """
     <html>
     <title>the title</title>
     <body>
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .test_module_paramminer_headers import *
+from .test_module_paramminer_headers import Paramminer_Headers, tempwordlist, helper
 
 
-class TestParamminer_Getparams(TestParamminer_Headers):
+class TestParamminer_Getparams(Paramminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
     config_overrides = {"modules": {"paramminer_getparams": {"wordlist": tempwordlist(["canary", "id"])}}}
 
     getparam_body = """
     <html>
     <title>the title</title>
     <body>
@@ -106,15 +106,15 @@
     def check(self, module_test, events):
         assert not any(
             e.type == "FINDING" and "[Paramminer] Getparam: [boring] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
-class TestParamminer_Getparams_Extract_Json(TestParamminer_Headers):
+class TestParamminer_Getparams_Extract_Json(Paramminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
     config_overrides = {"modules": {"paramminer_getparams": {"wordlist": tempwordlist([]), "http_extract": True}}}
 
     getparam_extract_json = """
     {
   "obscureParameter": 1,
   "common": 1
@@ -148,15 +148,15 @@
         assert any(
             e.type == "FINDING"
             and "[Paramminer] Getparam: [obscureParameter] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
-class TestParamminer_Getparams_Extract_Xml(TestParamminer_Headers):
+class TestParamminer_Getparams_Extract_Xml(Paramminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
     config_overrides = {
         "modules": {
             "paramminer_getparams": {"wordlist": tempwordlist([]), "http_extract": True, "skip_boring_words": True}
         }
     }
 
@@ -195,15 +195,15 @@
         assert any(
             e.type == "FINDING"
             and "[Paramminer] Getparam: [obscureParameter] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
-class TestParamminer_Getparams_Extract_Html(TestParamminer_Headers):
+class TestParamminer_Getparams_Extract_Html(Paramminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
     config_overrides = {
         "modules": {"paramminer_getparams": {"wordlist": tempwordlist(["canary"]), "http_extract": True}}
     }
 
     getparam_extract_html = """
 <html><a href="/?hack=1">ping</a></html>
@@ -233,15 +233,15 @@
     def check(self, module_test, events):
         assert any(
             e.type == "FINDING" and "[Paramminer] Getparam: [hack] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
-class TestParamminer_Getparams_finish(TestParamminer_Headers):
+class TestParamminer_Getparams_finish(Paramminer_Headers):
     modules_overrides = ["httpx", "excavate", "paramminer_getparams"]
     config_overrides = {
         "modules": {"paramminer_getparams": {"wordlist": tempwordlist(["canary", "canary2"]), "http_extract": True}}
     }
 
     targets = ["http://127.0.0.1:8888/test1.php", "http://127.0.0.1:8888/test2.php"]
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bbot.core.helpers import helper
 
 from .base import ModuleTestBase, tempwordlist
 
 
-class TestParamminer_Headers(ModuleTestBase):
+class Paramminer_Headers(ModuleTestBase):
     targets = ["http://127.0.0.1:8888"]
     modules_overrides = ["httpx", "paramminer_headers"]
     config_overrides = {"modules": {"paramminer_headers": {"wordlist": tempwordlist(["junkword1", "tracestate"])}}}
 
     headers_body = """
     <html>
     <title>the title</title>
@@ -45,15 +45,19 @@
             for e in events
         )
         assert not any(
             e.type == "FINDING" and "[Paramminer] Header: [junkword1]" in e.data["description"] for e in events
         )
 
 
-class TestParamminer_Headers(TestParamminer_Headers):
+class TestParamminer_Headers(Paramminer_Headers):
+    pass
+
+
+class TestParamminer_Headers_noreflection(Paramminer_Headers):
     headers_body_match = """
     <html>
     <title>the title</title>
     <body>
     <p>Hello Administrator!</p>';
     </body>
     </html>
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         respond_args = {"response_data": web_body}
         module_test.set_expect_requests(respond_args=respond_args)
 
     def check(self, module_test, events):
         report_file = module_test.scan.home / "web_report.html"
         with open(report_file) as f:
             report_content = f.read()
-        assert "<li>[HIGH] Known Secret Found" in report_content
+        assert "<li>[CRITICAL] Known Secret Found" in report_content
         assert (
             """<h3>URL</h3>
 <ul>
 <li><strong>http://127.0.0.1:8888/</strong>"""
             in report_content
         )
         assert (
```

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.0.2024rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/testsslcert.pem` & `bbot-1.1.0.2024rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/test/testsslkey.pem` & `bbot-1.1.0.2024rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.0.2024rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.0.2024rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.0.2024rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.0.2024rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.0.2024rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.0.2024rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.0.1958rc0/pyproject.toml` & `bbot-1.1.0.2024rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.0.1958rc"
+version = "v1.1.0.2024rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
 
@@ -28,14 +28,15 @@
 tabulate = "0.8.10"
 cloudcheck = "^2.0.0.34"
 websockets = "^11.0.2"
 pyjwt = "^2.7.0"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
 httpx = {extras = ["http2"], version = "^0.24.1"}
+anyio = "4.0.0rc1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 pytest-cov = "^4.0.0"
 poetry-dynamic-versioning = "^0.21.4"
```

### Comparing `bbot-1.1.0.1958rc0/PKG-INFO` & `bbot-1.1.0.2024rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.0.1958rc0
+Version: 1.1.0.2024rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansible (>=7.3.0,<8.0.0)
 Requires-Dist: ansible-runner (>=2.3.2,<3.0.0)
+Requires-Dist: anyio (==4.0.0rc1)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cloudcheck (>=2.0.0.34,<3.0.0.0)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
 Requires-Dist: httpx[http2] (>=0.24.1,<0.25.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
@@ -29,51 +30,30 @@
 Requires-Dist: tldextract (>=3.4.0,<4.0.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Requires-Dist: wordninja (>=2.0.0,<3.0.0)
 Requires-Dist: xmltojson (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/blacklanternsecurity/bbot
 Description-Content-Type: text/markdown
 
+![bbot_banner](https://user-images.githubusercontent.com/20261699/158000235-6c1ace81-a267-4f8e-90a1-f4c16884ebac.png)
+
 # BEE·bot
 
 ### OSINT automation for hackers.
 
 [![Python Version](https://img.shields.io/badge/python-3.9+-FF8400)](https://www.python.org) [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License](https://img.shields.io/badge/license-GPLv3-FF8400.svg)](https://github.com/blacklanternsecurity/bbot/blob/dev/LICENSE) [![Tests](https://github.com/blacklanternsecurity/bbot/actions/workflows/tests.yml/badge.svg?branch=stable)](https://github.com/blacklanternsecurity/bbot/actions?query=workflow%3A"tests") [![Codecov](https://codecov.io/gh/blacklanternsecurity/bbot/branch/dev/graph/badge.svg?token=IR5AZBDM5K)](https://codecov.io/gh/blacklanternsecurity/bbot) [![Pypi Downloads](https://img.shields.io/pypi/dm/bbot)](https://pypi.org/project/bbot) [![Discord](https://img.shields.io/discord/859164869970362439)](https://discord.com/invite/PZqkgxu5SA)
 
 BBOT is a modular, recursive OSINT framework that can execute the entire OSINT workflow in a single command.
 
-![bbot_banner](https://github.com/blacklanternsecurity/bbot/assets/20261699/af2e822c-d7d6-40e7-bcba-2ce52faa6c4c)
-
 BBOT is inspired by [Spiderfoot](https://github.com/smicallef/spiderfoot) but takes it to the next level with features like multi-target scans, lightning-fast asyncio performance, and NLP-powered subdomain mutations. It offers a wide range of functionality, including subdomain enumeration, port scanning, web screenshots, vulnerability scanning, and much more. 
 
 ![subdomain-stats-boeing](https://github.com/blacklanternsecurity/bbot/assets/20261699/de0154c1-476e-4337-9599-45a1c5e0e78b)
 
 BBOT typically outperforms other subdomain enumeration tools by 20-25%. To learn how this is possible, see [How It Works](https://www.blacklanternsecurity.com/bbot/how_it_works/).
 
-## Consider checking out our [Documentation](https://www.blacklanternsecurity.com/bbot):
-
-<!-- BBOT DOCS TOC -->
-- **Basics**
-    - [Getting Started](https://www.blacklanternsecurity.com/bbot/)
-    - [How it Works](https://www.blacklanternsecurity.com/bbot/how_it_works)
-    - [Comparison to Other Tools](https://www.blacklanternsecurity.com/bbot/comparison)
-- **Scanning**
-    - [Scanning Overview](https://www.blacklanternsecurity.com/bbot/scanning/)
-    - [Events](https://www.blacklanternsecurity.com/bbot/scanning/events)
-    - [Output](https://www.blacklanternsecurity.com/bbot/scanning/output)
-    - [Tips and Tricks](https://www.blacklanternsecurity.com/bbot/scanning/tips_and_tricks)
-    - [Advanced Usage](https://www.blacklanternsecurity.com/bbot/scanning/advanced)
-    - [Configuration](https://www.blacklanternsecurity.com/bbot/scanning/configuration)
-    - [List of Modules](https://www.blacklanternsecurity.com/bbot/scanning/list_of_modules)
-- **Contribution**
-    - [How to Write a Module](https://www.blacklanternsecurity.com/bbot/contribution)
-- **Misc**
-    - [Release History](https://www.blacklanternsecurity.com/bbot/release_history)
-<!-- END BBOT DOCS TOC -->
-
 ## Installation ([pip](https://pypi.org/project/bbot/))
 
 For more installation methods including [Docker](https://hub.docker.com/r/blacklanternsecurity/bbot), see [Installation](https://www.blacklanternsecurity.com/bbot/#installation).
 
 ```bash
 # Prerequisites:
 # - Linux (Windows and macOS are *not* supported)
@@ -170,14 +150,35 @@
     async for event in scan.async_start():
         print(event.json())
 
 import asyncio
 asyncio.run(main())
 ```
 
+## Documentation
+
+<!-- BBOT DOCS TOC -->
+- **Basics**
+    - [Getting Started](https://www.blacklanternsecurity.com/bbot/)
+    - [How it Works](https://www.blacklanternsecurity.com/bbot/how_it_works)
+    - [Comparison to Other Tools](https://www.blacklanternsecurity.com/bbot/comparison)
+- **Scanning**
+    - [Scanning Overview](https://www.blacklanternsecurity.com/bbot/scanning/)
+    - [Events](https://www.blacklanternsecurity.com/bbot/scanning/events)
+    - [Output](https://www.blacklanternsecurity.com/bbot/scanning/output)
+    - [Tips and Tricks](https://www.blacklanternsecurity.com/bbot/scanning/tips_and_tricks)
+    - [Advanced Usage](https://www.blacklanternsecurity.com/bbot/scanning/advanced)
+    - [Configuration](https://www.blacklanternsecurity.com/bbot/scanning/configuration)
+    - [List of Modules](https://www.blacklanternsecurity.com/bbot/scanning/list_of_modules)
+- **Contribution**
+    - [How to Write a Module](https://www.blacklanternsecurity.com/bbot/contribution)
+- **Misc**
+    - [Release History](https://www.blacklanternsecurity.com/bbot/release_history)
+<!-- END BBOT DOCS TOC -->
+
 ## Acknowledgements
 
 Thanks to these amazing people for contributing to BBOT! :heart:
 
 If you're interested in contributing to BBOT, or just curious how it works under the hood, see [Contribution](https://www.blacklanternsecurity.com/bbot/contribution/).
 
 <p align="center">
```


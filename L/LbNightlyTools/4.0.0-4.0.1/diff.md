# Comparing `tmp/LbNightlyTools-4.0.0.tar.gz` & `tmp/LbNightlyTools-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbNightlyTools-4.0.0.tar", last modified: Tue Jul 11 11:19:26 2023, max compression
+gzip compressed data, was "LbNightlyTools-4.0.1.tar", last modified: Fri Jul 28 14:48:41 2023, max compression
```

## Comparing `LbNightlyTools-4.0.0.tar` & `LbNightlyTools-4.0.1.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4932 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      487 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    15557 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35147 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-11 11:19:26.548000 LbNightlyTools-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/admin/
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/admin/LHCb_LbScripts.spectemplate
--rwxr-xr-x   0 root         (0) root         (0)     1882 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/admin/RpmHelpers.py
--rwxr-xr-x   0 root         (0) root         (0)     3688 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/admin/createLbScriptsRpm
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/.gitignore
--rw-r--r--   0 root         (0) root         (0)      982 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/Push CouchDB Nightly Builds.launch
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/auth/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/auth/validate_doc_update.js
--rw-r--r--   0 root         (0) root         (0)      486 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/build_id_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/deployment/
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/deployment/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/deployment/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/deployment/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/deployment/views/ready/
--rw-r--r--   0 root         (0) root         (0)      920 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/deployment/views/ready/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/frontend-stats/
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/.couchappignore
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/.couchapprc
--rw-r--r--   0 root         (0) root         (0)      672 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/README.md
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/_id
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/couchapp.json
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/frontend-stats/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/frontend-stats/views/byDate/
--rw-r--r--   0 root         (0) root         (0)     2483 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/frontend-stats/views/byDate/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/merge_requests/
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/merge_requests/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/merge_requests/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/merge_requests/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/merge_requests/views/mr_slots_by_ref_slot/
--rw-r--r--   0 root         (0) root         (0)      307 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/merge_requests/views/mrs/
--rw-r--r--   0 root         (0) root         (0)      756 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/merge_requests/views/mrs/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/names/
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/names/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.508000 LbNightlyTools-4.0.0/couchdb/names/views/platforms/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/platforms/map.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/platforms/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/names/views/projects/
--rw-r--r--   0 root         (0) root         (0)      142 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/projects/map.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/projects/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/names/views/slots/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/slots/map.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/names/views/slots/reduce.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/views/by_app_version/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/nightlies_summaries/views/by_app_version/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/old_dashboard/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/old_dashboard/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/old_dashboard/language
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/old_dashboard/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/views/byTime/
--rw-r--r--   0 root         (0) root         (0)       74 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/periodic_summaries/views/byTime/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/releases/
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/releases/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/releases/language
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/releases/lists/
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/releases/lists/projectBuildIds.js
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/releases/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/releases/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/releases/views/projectBuildIds/
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/releases/views/projectBuildIds/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/summaries/
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/_id
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/language
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/rewrites.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.496000 LbNightlyTools-4.0.0/couchdb/summaries/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/summaries/views/byDay/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/views/byDay/map.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/couchdb/summaries/views/lastBuildId/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/views/lastBuildId/map.js
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/summaries/views/lastBuildId/reduce.js
--rwxr-xr-x   0 root         (0) root         (0)     3600 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/couchdb/webapp_testbench.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.512000 LbNightlyTools-4.0.0/cron/
--rwxr-xr-x   0 root         (0) root         (0)     1863 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/cron/cleanup_artifacts.sh
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/cron/logrotate.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.516000 LbNightlyTools-4.0.0/docs/
--rw-r--r--   0 root         (0) root         (0)    25550 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/Interactive builds of LHCb projects.ipynb
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/LHCbPR2.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.516000 LbNightlyTools-4.0.0/docs/configuration/
--rw-r--r--   0 root         (0) root         (0)     3017 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/configuration/Example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.516000 LbNightlyTools-4.0.0/docs/examples/
--rwxr-xr-x   0 root         (0) root         (0)     1247 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/examples/lbpr-example
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/jenkins-scripts.dot
--rw-r--r--   0 root         (0) root         (0)   142880 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/jenkins-scripts.dot.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.516000 LbNightlyTools-4.0.0/docs/note/
--rw-r--r--   0 root         (0) root         (0)   946715 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/LHCb-INT-2013-006.pdf
--rw-r--r--   0 root         (0) root         (0)    24731 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/LHCb.bst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/Makefile
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/README.txt
--rw-r--r--   0 root         (0) root         (0)     3132 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/appendix.tex
--rw-r--r--   0 root         (0) root         (0)     5159 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/bibliography.bib
--rw-r--r--   0 root         (0) root         (0)    32522 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/cite.sty
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/conclusions.tex
--rw-r--r--   0 root         (0) root         (0)     5975 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/dashboard.tex
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/design.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.520000 LbNightlyTools-4.0.0/docs/note/figs/
--rw-r--r--   0 root         (0) root         (0)    60108 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/cdash-1.png
--rw-r--r--   0 root         (0) root         (0)    97134 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/cdash-2.png
--rw-r--r--   0 root         (0) root         (0)   101416 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/cdash-3.png
--rw-r--r--   0 root         (0) root         (0)   162025 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/cdash-4.png
--rw-r--r--   0 root         (0) root         (0)    91381 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/jenkins-1.png
--rw-r--r--   0 root         (0) root         (0)    81047 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/jenkins-2.png
--rw-r--r--   0 root         (0) root         (0)   173109 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/jenkins-3.png
--rw-r--r--   0 root         (0) root         (0)   160146 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/lhcb-logo.eps
--rw-r--r--   0 root         (0) root         (0)    14116 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/lhcb-logo.pdf
--rw-r--r--   0 root         (0) root         (0)   134216 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/figs/old-summary.png
--rw-r--r--   0 root         (0) root         (0)    33058 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/implementation.tex
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/introduction.tex
--rw-r--r--   0 root         (0) root         (0)     5596 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/lhcb-int-2013-006.kilepr
--rwxr-xr-x   0 root         (0) root         (0)     3645 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/listsymbols
--rw-r--r--   0 root         (0) root         (0)     1586 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/main.tex
--rw-r--r--   0 root         (0) root         (0)    61167 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/mciteplus.sty
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/preamble.tex
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/requirements.tex
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/title-LHCb-ANA.tex
--rw-r--r--   0 root         (0) root         (0)    28723 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/note/unsrturl.bst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.520000 LbNightlyTools-4.0.0/docs/operation/
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/operation/Makefile
--rw-r--r--   0 root         (0) root         (0)    26499 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/operation/NightlyBuildsOperation.html
--rw-r--r--   0 root         (0) root         (0)    11288 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/operation/NightlyBuildsOperation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.520000 LbNightlyTools-4.0.0/docs/operation/images/
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/operation/images/jenkins-jobs.dot
--rw-r--r--   0 root         (0) root         (0)    32492 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/operation/images/jenkins-jobs.dot.png
--rw-r--r--   0 root         (0) root         (0)     7965 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/docs/pylint.rc
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.520000 LbNightlyTools-4.0.0/python/LbMsg/
--rwxr-xr-x   0 root         (0) root         (0)     3452 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbMsg/BuildMsg.py
--rw-r--r--   0 root         (0) root         (0)     4609 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbMsg/Common.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbMsg/TestMsg.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbMsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.524000 LbNightlyTools-4.0.0/python/LbNightlyTools/
--rw-r--r--   0 root         (0) root         (0)     4457 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/ArtifactsServer.py
--rw-r--r--   0 root         (0) root         (0)    12315 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/BuildLogScanner.py
--rw-r--r--   0 root         (0) root         (0)    32491 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/BuildMethods.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/CheckSlotPreconditions.py
--rw-r--r--   0 root         (0) root         (0)    35063 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/CheckoutMethods.py
--rw-r--r--   0 root         (0) root         (0)    81350 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Configuration.py
--rwxr-xr-x   0 root         (0) root         (0)     5166 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/GetNightlyRefs.py
--rw-r--r--   0 root         (0) root         (0)     7547 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/GitlabUtils.py
--rw-r--r--   0 root         (0) root         (0)    18542 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/HTMLUtils.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/LbScriptsUtils.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/MergeRequestBuilds.py
--rw-r--r--   0 root         (0) root         (0)     6152 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/ProcUtils.py
--rw-r--r--   0 root         (0) root         (0)     6339 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.528000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/
--rw-r--r--   0 root         (0) root         (0)    36766 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Build.py
--rw-r--r--   0 root         (0) root         (0)    15160 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Checkout.py
--rw-r--r--   0 root         (0) root         (0)    15846 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/CollectBuildLogs.py
--rwxr-xr-x   0 root         (0) root         (0)    28229 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Common.py
--rw-r--r--   0 root         (0) root         (0)    13855 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/EnabledSlots.py
--rw-r--r--   0 root         (0) root         (0)    13783 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/GitlabMR.py
--rw-r--r--   0 root         (0) root         (0)     7665 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Index.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Install.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Preconditions.py
--rw-r--r--   0 root         (0) root         (0)    17852 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Release.py
--rw-r--r--   0 root         (0) root         (0)    14262 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Test.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26838 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/_entry_points.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/extract.php
--rw-r--r--   0 root         (0) root         (0)      999 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/listzip.php
--rw-r--r--   0 root         (0) root         (0)    45291 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/Utils.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.532000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8920 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_build.py
--rw-r--r--   0 root         (0) root         (0)    19337 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_build_script.py
--rw-r--r--   0 root         (0) root         (0)    12989 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_checkout.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_checkout_script.py
--rw-r--r--   0 root         (0) root         (0)     9317 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_config_load.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_config_pickle.py
--rw-r--r--   0 root         (0) root         (0)    15153 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_configuration_check.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_copytree.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_coverity_support.py
--rw-r--r--   0 root         (0) root         (0)    14609 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_enabled_slots_script.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_gitlab_mr_script.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_indexer.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_install.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_jobconfig.py
--rw-r--r--   0 root         (0) root         (0)     3655 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_merge_request_builds.py
--rw-r--r--   0 root         (0) root         (0)     8088 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_pack.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_precond.py
--rw-r--r--   0 root         (0) root         (0)    10940 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_rel_gen_script.py
--rw-r--r--   0 root         (0) root         (0)     8064 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_release_poll.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_repository.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_retry.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     3338 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbNightlyTools/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.524000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11506 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2664 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-11 11:19:26.000000 LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.532000 LbNightlyTools-4.0.0/python/LbPR/
--rw-r--r--   0 root         (0) root         (0)     3093 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPR/LbPRJobManager.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPR/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14057 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPR/_entry_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.532000 LbNightlyTools-4.0.0/python/LbPeriodicTools/
--rw-r--r--   0 root         (0) root         (0)     4171 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicStarter.py
--rw-r--r--   0 root         (0) root         (0)    11731 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicTest.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicTestSchedule.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/TestSchedule.xsd
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10067 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/_entry_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.532000 LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_LHCbPR.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_Starter.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_XMLParsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/python/LbRPMTools/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbCompatSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)    22912 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbExternalsSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)    10040 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbGenericSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)    16527 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)     8700 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbMetaSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)    54217 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/LHCbRPMSpecBuilder.py
--rw-r--r--   0 root         (0) root         (0)    29932 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/PackageSlot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/python/LbRPMTools/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6060 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_ExternalSpec.py
--rw-r--r--   0 root         (0) root         (0)    14756 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_PackageSlot.py
--rw-r--r--   0 root         (0) root         (0)    18876 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_Spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/python/LbTools/
--rw-r--r--   0 root         (0) root         (0)     5602 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbTools/Manifest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbTools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/python/LbTools/tests/
--rw-r--r--   0 root         (0) root         (0)     3811 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbTools/tests/test_XMLParsing.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/python/LbTools/tests/test_toolchain_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/scripts/
--rwxr-xr-x   0 root         (0) root         (0)     1053 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/scripts/lbn-get-configs
--rwxr-xr-x   0 root         (0) root         (0)     1595 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/scripts/lbn-wrapcmd
--rwxr-xr-x   0 root         (0) root         (0)     2703 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/scripts/lbpr-collect
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-11 11:19:26.548000 LbNightlyTools-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10837 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/artifacts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/artifacts/packs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/artifacts/packs/src/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/build_tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/build_tests/orig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/build_tests/orig/dummy/
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/build_tests/orig/dummy/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/build_tests/test_project/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/build_tests/test_project/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/build_tests/test_project/lhcbproject.yml
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/build_tests/test_project/main.cpp
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/ci-test-hook-content.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/BadCMT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/BadCMT/cmt/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/BadCMake/
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/Gaudi/
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/Gaudi/toolchain.cmake
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/broken/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.536000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Brunel/
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Gaudi/
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/LHCb/
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Lbcom/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/NewLHCbProj/
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/NewLHCbProj/lhcbproject.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/NewProj/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Online/
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Online/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Rec/
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/Rec/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmake/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Brunel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Brunel/cmt/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Gaudi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Gaudi/cmt/
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/LHCb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/LHCb/cmt/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Lbcom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Lbcom/cmt/
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/NewLHCbProj/
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/NewLHCbProj/lhcbproject.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/NewProj/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/NewProj/project.info
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Online/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Online/cmt/
--rw-r--r--   0 root         (0) root         (0)      115 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Online/cmt/project.cmt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.500000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Rec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Rec/cmt/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/Rec/cmt/project.cmt
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/collect_deps/cmt/conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/coverity/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/coverity/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1722 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/bin/cov-analyze
--rwxr-xr-x   0 root         (0) root         (0)     1630 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/bin/cov-build
--rwxr-xr-x   0 root         (0) root         (0)     1787 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/bin/cov-commit-defects
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/coverity/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/TEST_HEAD/
--rw-r--r--   0 root         (0) root         (0)      310 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
--rw-r--r--   0 root         (0) root         (0)      256 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/build/TEST/TEST_HEAD/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/coverity/configs/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/coverity/configs/coverity_config.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/data-packs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/fix_glimpse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/fix_glimpse/docs/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/fix_glimpse/docs/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/fix_glimpse/level1/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/fix_glimpse/level1/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/fix_glimpse/level1/level2/
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/fix_glimpse/level1/level2/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/fix_glimpse/levelA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/fix_glimpse/levelA/levelB/
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/fix_glimpse/untouched/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/fix_glimpse/untouched/.glimpse_filenames
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/indexer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/indexer/AProject/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/cmake/
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/include/
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/include/MyHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.540000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/Headers/
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.504000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/python/MyPackage/
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/scripts/
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/scripts/MyScript
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/src/
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/MyPackage/src/MySource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/indexer/AProject/build.dir/
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/periodic_tests/
--rw-r--r--   0 root         (0) root         (0)      811 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/periodic_tests/lhcbpr_schedule.xml
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/periodic_tests/schedule.xml
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/periodic_tests/scheduleIncorrect.xml
--rw-r--r--   0 root         (0) root         (0)    15858 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/periodic_tests/slotbuilds.json
--rw-r--r--   0 root         (0) root         (0)      886 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/periodic_tests/starter_schedule.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/rpm/
--rw-r--r--   0 root         (0) root         (0)     1265 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/Brunel_v46r0.spec
--rw-r--r--   0 root         (0) root         (0)     1687 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
--rw-r--r--   0 root         (0) root         (0)     7196 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/LCG_68_externalsDict.json
--rw-r--r--   0 root         (0) root         (0)     3230 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/PARAM_TMVAWeights.spec
--rw-r--r--   0 root         (0) root         (0)     3230 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/PARAM_TMVAWeights_rel5.spec
--rw-r--r--   0 root         (0) root         (0)      938 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/datapkg-slot-config.json
--rw-r--r--   0 root         (0) root         (0)     1981 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/glimpse_Brunel_v46r0.spec
--rw-r--r--   0 root         (0) root         (0)      617 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/manifest.xml
--rw-r--r--   0 root         (0) root         (0)     1273 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/manifest_do0.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/rpm/rel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
--rw-r--r--   0 root         (0) root         (0)      893 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/slot-config.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/rpm/slot-configdo0.json
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-2.json
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-2b.json
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-env.json
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-lbcore-192.json
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-lbcore-664.json
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot-with-shared.json
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/testing-slot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/testdata/tools/
--rw-r--r--   0 root         (0) root         (0)      658 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/tools/manifest.xml
--rw-r--r--   0 root         (0) root         (0)     1273 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/tools/manifest_do0.xml
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/tools/manifest_with_pkgs.xml
--rw-r--r--   0 root         (0) root         (0)     1588 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/tools/manifest_with_pkgs_new.xml
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/testdata/tools/mini_manifest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:19:26.544000 LbNightlyTools-4.0.0/utils/
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-11 11:19:25.000000 LbNightlyTools-4.0.0/utils/add_ci_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.008000 LbNightlyTools-4.0.1/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    15557 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35147 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/COPYING
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-28 14:48:41.008000 LbNightlyTools-4.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/admin/
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/admin/LHCb_LbScripts.spectemplate
+-rwxr-xr-x   0 root         (0) root         (0)     1882 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/admin/RpmHelpers.py
+-rwxr-xr-x   0 root         (0) root         (0)     3688 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/admin/createLbScriptsRpm
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/Push CouchDB Nightly Builds.launch
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/auth/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/auth/validate_doc_update.js
+-rw-r--r--   0 root         (0) root         (0)      486 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/build_id_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/deployment/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/deployment/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/deployment/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/deployment/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/deployment/views/ready/
+-rw-r--r--   0 root         (0) root         (0)      920 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/deployment/views/ready/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/frontend-stats/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/.couchappignore
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/.couchapprc
+-rw-r--r--   0 root         (0) root         (0)      672 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/README.md
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/_id
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/couchapp.json
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/frontend-stats/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/frontend-stats/views/byDate/
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/frontend-stats/views/byDate/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/merge_requests/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/merge_requests/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/merge_requests/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/merge_requests/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.964000 LbNightlyTools-4.0.1/couchdb/merge_requests/views/mr_slots_by_ref_slot/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/merge_requests/views/mr_slots_by_ref_slot/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/merge_requests/views/mrs/
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/merge_requests/views/mrs/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/names/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/names/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/names/views/platforms/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/platforms/map.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/platforms/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/names/views/projects/
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/projects/map.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/projects/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/names/views/slots/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/slots/map.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/names/views/slots/reduce.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/views/by_app_version/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/nightlies_summaries/views/by_app_version/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/old_dashboard/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/old_dashboard/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/old_dashboard/language
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/old_dashboard/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.968000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/views/byTime/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/periodic_summaries/views/byTime/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/releases/
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/releases/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/releases/language
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/releases/lists/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/releases/lists/projectBuildIds.js
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/releases/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/releases/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/releases/views/projectBuildIds/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/releases/views/projectBuildIds/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/summaries/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/_id
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/language
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/rewrites.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.948000 LbNightlyTools-4.0.1/couchdb/summaries/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/summaries/views/byDay/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/views/byDay/map.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/couchdb/summaries/views/lastBuildId/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/views/lastBuildId/map.js
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/summaries/views/lastBuildId/reduce.js
+-rwxr-xr-x   0 root         (0) root         (0)     3600 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/couchdb/webapp_testbench.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/cron/
+-rwxr-xr-x   0 root         (0) root         (0)     1863 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/cron/cleanup_artifacts.sh
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/cron/logrotate.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/docs/
+-rw-r--r--   0 root         (0) root         (0)    25550 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/Interactive builds of LHCb projects.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/LHCbPR2.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/docs/configuration/
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/configuration/Example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.972000 LbNightlyTools-4.0.1/docs/examples/
+-rwxr-xr-x   0 root         (0) root         (0)     1247 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/examples/lbpr-example
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/jenkins-scripts.dot
+-rw-r--r--   0 root         (0) root         (0)   142880 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/jenkins-scripts.dot.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.976000 LbNightlyTools-4.0.1/docs/note/
+-rw-r--r--   0 root         (0) root         (0)   946715 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/LHCb-INT-2013-006.pdf
+-rw-r--r--   0 root         (0) root         (0)    24731 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/LHCb.bst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/Makefile
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/README.txt
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/appendix.tex
+-rw-r--r--   0 root         (0) root         (0)     5159 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/bibliography.bib
+-rw-r--r--   0 root         (0) root         (0)    32522 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/cite.sty
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/conclusions.tex
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/dashboard.tex
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/design.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.980000 LbNightlyTools-4.0.1/docs/note/figs/
+-rw-r--r--   0 root         (0) root         (0)    60108 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/cdash-1.png
+-rw-r--r--   0 root         (0) root         (0)    97134 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/cdash-2.png
+-rw-r--r--   0 root         (0) root         (0)   101416 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/cdash-3.png
+-rw-r--r--   0 root         (0) root         (0)   162025 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/cdash-4.png
+-rw-r--r--   0 root         (0) root         (0)    91381 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/jenkins-1.png
+-rw-r--r--   0 root         (0) root         (0)    81047 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/jenkins-2.png
+-rw-r--r--   0 root         (0) root         (0)   173109 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/jenkins-3.png
+-rw-r--r--   0 root         (0) root         (0)   160146 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/lhcb-logo.eps
+-rw-r--r--   0 root         (0) root         (0)    14116 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/lhcb-logo.pdf
+-rw-r--r--   0 root         (0) root         (0)   134216 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/figs/old-summary.png
+-rw-r--r--   0 root         (0) root         (0)    33058 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/implementation.tex
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/introduction.tex
+-rw-r--r--   0 root         (0) root         (0)     5596 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/lhcb-int-2013-006.kilepr
+-rwxr-xr-x   0 root         (0) root         (0)     3645 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/listsymbols
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/main.tex
+-rw-r--r--   0 root         (0) root         (0)    61167 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/mciteplus.sty
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/preamble.tex
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/requirements.tex
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/title-LHCb-ANA.tex
+-rw-r--r--   0 root         (0) root         (0)    28723 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/note/unsrturl.bst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.980000 LbNightlyTools-4.0.1/docs/operation/
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/operation/Makefile
+-rw-r--r--   0 root         (0) root         (0)    26499 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/operation/NightlyBuildsOperation.html
+-rw-r--r--   0 root         (0) root         (0)    11288 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/operation/NightlyBuildsOperation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.980000 LbNightlyTools-4.0.1/docs/operation/images/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/operation/images/jenkins-jobs.dot
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/operation/images/jenkins-jobs.dot.png
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/docs/pylint.rc
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.980000 LbNightlyTools-4.0.1/python/LbMsg/
+-rwxr-xr-x   0 root         (0) root         (0)     3452 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbMsg/BuildMsg.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbMsg/Common.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbMsg/TestMsg.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbMsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.984000 LbNightlyTools-4.0.1/python/LbNightlyTools/
+-rw-r--r--   0 root         (0) root         (0)     4457 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/ArtifactsServer.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/BuildLogScanner.py
+-rw-r--r--   0 root         (0) root         (0)    32677 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/BuildMethods.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/CheckSlotPreconditions.py
+-rw-r--r--   0 root         (0) root         (0)    35063 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/CheckoutMethods.py
+-rw-r--r--   0 root         (0) root         (0)    81350 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Configuration.py
+-rwxr-xr-x   0 root         (0) root         (0)     5166 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/GetNightlyRefs.py
+-rw-r--r--   0 root         (0) root         (0)     7547 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/GitlabUtils.py
+-rw-r--r--   0 root         (0) root         (0)    18542 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/HTMLUtils.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/LbScriptsUtils.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/MergeRequestBuilds.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/ProcUtils.py
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.988000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/
+-rw-r--r--   0 root         (0) root         (0)    36766 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Build.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Checkout.py
+-rw-r--r--   0 root         (0) root         (0)    15846 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/CollectBuildLogs.py
+-rwxr-xr-x   0 root         (0) root         (0)    28293 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Common.py
+-rw-r--r--   0 root         (0) root         (0)    13855 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/EnabledSlots.py
+-rw-r--r--   0 root         (0) root         (0)    13783 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/GitlabMR.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Index.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Install.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Preconditions.py
+-rw-r--r--   0 root         (0) root         (0)    17852 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Release.py
+-rw-r--r--   0 root         (0) root         (0)    14262 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Test.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26838 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/_entry_points.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/extract.php
+-rw-r--r--   0 root         (0) root         (0)      999 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/listzip.php
+-rw-r--r--   0 root         (0) root         (0)    45291 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/Utils.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.988000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_build.py
+-rw-r--r--   0 root         (0) root         (0)    19337 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_build_script.py
+-rw-r--r--   0 root         (0) root         (0)    12989 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_checkout.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_checkout_script.py
+-rw-r--r--   0 root         (0) root         (0)     9317 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_config_load.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_config_pickle.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_configuration_check.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_copytree.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_coverity_support.py
+-rw-r--r--   0 root         (0) root         (0)    14609 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_enabled_slots_script.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_gitlab_mr_script.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_indexer.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_install.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_jobconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3655 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_merge_request_builds.py
+-rw-r--r--   0 root         (0) root         (0)     8088 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_pack.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_precond.py
+-rw-r--r--   0 root         (0) root         (0)    10940 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_rel_gen_script.py
+-rw-r--r--   0 root         (0) root         (0)     8064 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_release_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_retry.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbNightlyTools/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.984000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11506 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-28 14:48:40.000000 LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbPR/
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPR/LbPRJobManager.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPR/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14057 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPR/_entry_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbPeriodicTools/
+-rw-r--r--   0 root         (0) root         (0)     4171 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicStarter.py
+-rw-r--r--   0 root         (0) root         (0)    11731 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicTest.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicTestSchedule.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/TestSchedule.xsd
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/_entry_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_LHCbPR.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_Starter.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_XMLParsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbRPMTools/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbCompatSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    22912 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbExternalsSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    10040 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbGenericSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    16527 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)     8700 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbMetaSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    54217 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/LHCbRPMSpecBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    29932 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/PackageSlot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbRPMTools/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_ExternalSpec.py
+-rw-r--r--   0 root         (0) root         (0)    14756 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_PackageSlot.py
+-rw-r--r--   0 root         (0) root         (0)    18876 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_Spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbTools/
+-rw-r--r--   0 root         (0) root         (0)     5602 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbTools/Manifest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbTools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/python/LbTools/tests/
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbTools/tests/test_XMLParsing.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/python/LbTools/tests/test_toolchain_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.992000 LbNightlyTools-4.0.1/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)     1053 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/scripts/lbn-get-configs
+-rwxr-xr-x   0 root         (0) root         (0)     1595 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/scripts/lbn-wrapcmd
+-rwxr-xr-x   0 root         (0) root         (0)     2703 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/scripts/lbpr-collect
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-28 14:48:41.008000 LbNightlyTools-4.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    11060 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/testdata/artifacts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/testdata/artifacts/packs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/artifacts/packs/src/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/testdata/build_tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/testdata/build_tests/orig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/build_tests/orig/dummy/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/build_tests/orig/dummy/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/build_tests/test_project/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/build_tests/test_project/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/build_tests/test_project/lhcbproject.yml
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/build_tests/test_project/main.cpp
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/ci-test-hook-content.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.952000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/BadCMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/BadCMT/cmt/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/BadCMT/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/BadCMake/
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/BadCMake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/Gaudi/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/Gaudi/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/Gaudi/toolchain.cmake
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/broken/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Brunel/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Brunel/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Gaudi/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Gaudi/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Gaudi/toolchain.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/LHCb/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/LHCb/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Lbcom/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Lbcom/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/NewLHCbProj/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/NewLHCbProj/lhcbproject.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/NewProj/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Online/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Online/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Rec/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/Rec/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmake/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.996000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Brunel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Brunel/cmt/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Brunel/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Gaudi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Gaudi/cmt/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Gaudi/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/LHCb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/LHCb/cmt/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/LHCb/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Lbcom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Lbcom/cmt/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Lbcom/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/NewLHCbProj/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/NewLHCbProj/lhcbproject.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/NewProj/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/NewProj/project.info
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Online/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Online/cmt/
+-rw-r--r--   0 root         (0) root         (0)      115 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Online/cmt/project.cmt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Rec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Rec/cmt/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/Rec/cmt/project.cmt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/collect_deps/cmt/conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/coverity/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/coverity/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1722 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/bin/cov-analyze
+-rwxr-xr-x   0 root         (0) root         (0)     1630 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/bin/cov-build
+-rwxr-xr-x   0 root         (0) root         (0)     1787 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/bin/cov-commit-defects
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/coverity/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/TEST_HEAD/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/TEST_HEAD/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/TEST_HEAD/InstallArea/.empty
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/build/TEST/TEST_HEAD/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/coverity/configs/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/coverity/configs/coverity_config.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/data-packs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/fix_glimpse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/docs/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/docs/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/level1/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/level1/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/level1/level2/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/level1/level2/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/fix_glimpse/levelA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/levelA/levelB/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/levelA/levelB/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/untouched/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/fix_glimpse/untouched/.glimpse_filenames
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.956000 LbNightlyTools-4.0.1/testdata/indexer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.960000 LbNightlyTools-4.0.1/testdata/indexer/AProject/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.960000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/cmake/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/cmake/AProjectConfig.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/include/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/include/GeneratedHeader.h
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/include/MyHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/AProject_merged_confDb.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/GeneratedPython.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackageConf.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_confDb.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/MyPackage_user_confDb.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/SomeModule.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/SomethingConf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/InstallArea/python/MyPackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.960000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/Headers/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/Headers/MyHeader.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:40.960000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/python/MyPackage/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/python/MyPackage/SomeModule.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/python/MyPackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/scripts/
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/scripts/MyScript
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/src/
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/MyPackage/src/MySource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/indexer/AProject/build.dir/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/indexer/AProject/build.dir/IgnoredSource.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/periodic_tests/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/periodic_tests/lhcbpr_schedule.xml
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/periodic_tests/schedule.xml
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/periodic_tests/scheduleIncorrect.xml
+-rw-r--r--   0 root         (0) root         (0)    15858 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/periodic_tests/slotbuilds.json
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/periodic_tests/starter_schedule.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/rpm/
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/Brunel_v46r0.spec
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/LCG_68_externalsDict.json
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/PARAM_TMVAWeights.spec
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/PARAM_TMVAWeights_rel5.spec
+-rw-r--r--   0 root         (0) root         (0)      938 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/datapkg-slot-config.json
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/glimpse_Brunel_v46r0.spec
+-rw-r--r--   0 root         (0) root         (0)      617 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/manifest.xml
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/manifest_do0.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.004000 LbNightlyTools-4.0.1/testdata/rpm/rel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/rel/PARAM_TMVAWeights_v1r2-1.0.0-1.noarch.rpm
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-1.noarch.rpm
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-4.noarch.rpm
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/rel/PARAM_TMVAWeights_v1r4-1.0.0-toto.noarch.rpm
+-rw-r--r--   0 root         (0) root         (0)      893 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/slot-config.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/rpm/slot-configdo0.json
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-2.json
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-2b.json
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-env.json
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-lbcore-192.json
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-lbcore-664.json
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot-with-shared.json
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/testing-slot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.008000 LbNightlyTools-4.0.1/testdata/tools/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/tools/manifest.xml
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/tools/manifest_do0.xml
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/tools/manifest_with_pkgs.xml
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/tools/manifest_with_pkgs_new.xml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/testdata/tools/mini_manifest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 14:48:41.008000 LbNightlyTools-4.0.1/utils/
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-28 14:48:39.000000 LbNightlyTools-4.0.1/utils/add_ci_webhook.py
```

### Comparing `LbNightlyTools-4.0.0/.gitlab-ci.yml` & `LbNightlyTools-4.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/CHANGELOG.md` & `LbNightlyTools-4.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/COPYING` & `LbNightlyTools-4.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/admin/LHCb_LbScripts.spectemplate` & `LbNightlyTools-4.0.1/admin/LHCb_LbScripts.spectemplate`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/admin/RpmHelpers.py` & `LbNightlyTools-4.0.1/admin/RpmHelpers.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/admin/createLbScriptsRpm` & `LbNightlyTools-4.0.1/admin/createLbScriptsRpm`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/Push CouchDB Nightly Builds.launch` & `LbNightlyTools-4.0.1/couchdb/Push CouchDB Nightly Builds.launch`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/README.md` & `LbNightlyTools-4.0.1/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/auth/validate_doc_update.js` & `LbNightlyTools-4.0.1/couchdb/auth/validate_doc_update.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/deployment/views/ready/map.js` & `LbNightlyTools-4.0.1/couchdb/deployment/views/ready/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/frontend-stats/README.md` & `LbNightlyTools-4.0.1/couchdb/frontend-stats/README.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/frontend-stats/views/byDate/map.js` & `LbNightlyTools-4.0.1/couchdb/frontend-stats/views/byDate/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/merge_requests/views/mrs/map.js` & `LbNightlyTools-4.0.1/couchdb/merge_requests/views/mrs/map.js`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/old_dashboard/rewrites.json` & `LbNightlyTools-4.0.1/couchdb/old_dashboard/rewrites.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/couchdb/webapp_testbench.py` & `LbNightlyTools-4.0.1/couchdb/webapp_testbench.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/cron/cleanup_artifacts.sh` & `LbNightlyTools-4.0.1/cron/cleanup_artifacts.sh`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/Interactive builds of LHCb projects.ipynb` & `LbNightlyTools-4.0.1/docs/Interactive builds of LHCb projects.ipynb`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/LHCbPR2.md` & `LbNightlyTools-4.0.1/docs/LHCbPR2.md`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/configuration/Example.py` & `LbNightlyTools-4.0.1/docs/configuration/Example.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/examples/lbpr-example` & `LbNightlyTools-4.0.1/docs/examples/lbpr-example`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/jenkins-scripts.dot` & `LbNightlyTools-4.0.1/docs/jenkins-scripts.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/jenkins-scripts.dot.png` & `LbNightlyTools-4.0.1/docs/jenkins-scripts.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/LHCb-INT-2013-006.pdf` & `LbNightlyTools-4.0.1/docs/note/LHCb-INT-2013-006.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/LHCb.bst` & `LbNightlyTools-4.0.1/docs/note/LHCb.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/Makefile` & `LbNightlyTools-4.0.1/docs/note/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/appendix.tex` & `LbNightlyTools-4.0.1/docs/note/appendix.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/bibliography.bib` & `LbNightlyTools-4.0.1/docs/note/bibliography.bib`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/cite.sty` & `LbNightlyTools-4.0.1/docs/note/cite.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/conclusions.tex` & `LbNightlyTools-4.0.1/docs/note/conclusions.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/dashboard.tex` & `LbNightlyTools-4.0.1/docs/note/dashboard.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/design.tex` & `LbNightlyTools-4.0.1/docs/note/design.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/cdash-1.png` & `LbNightlyTools-4.0.1/docs/note/figs/cdash-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/cdash-2.png` & `LbNightlyTools-4.0.1/docs/note/figs/cdash-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/cdash-3.png` & `LbNightlyTools-4.0.1/docs/note/figs/cdash-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/cdash-4.png` & `LbNightlyTools-4.0.1/docs/note/figs/cdash-4.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/jenkins-1.png` & `LbNightlyTools-4.0.1/docs/note/figs/jenkins-1.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/jenkins-2.png` & `LbNightlyTools-4.0.1/docs/note/figs/jenkins-2.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/jenkins-3.png` & `LbNightlyTools-4.0.1/docs/note/figs/jenkins-3.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/lhcb-logo.eps` & `LbNightlyTools-4.0.1/docs/note/figs/lhcb-logo.eps`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/lhcb-logo.pdf` & `LbNightlyTools-4.0.1/docs/note/figs/lhcb-logo.pdf`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/figs/old-summary.png` & `LbNightlyTools-4.0.1/docs/note/figs/old-summary.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/implementation.tex` & `LbNightlyTools-4.0.1/docs/note/implementation.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/introduction.tex` & `LbNightlyTools-4.0.1/docs/note/introduction.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/lhcb-int-2013-006.kilepr` & `LbNightlyTools-4.0.1/docs/note/lhcb-int-2013-006.kilepr`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/listsymbols` & `LbNightlyTools-4.0.1/docs/note/listsymbols`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/main.tex` & `LbNightlyTools-4.0.1/docs/note/main.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/mciteplus.sty` & `LbNightlyTools-4.0.1/docs/note/mciteplus.sty`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/preamble.tex` & `LbNightlyTools-4.0.1/docs/note/preamble.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/requirements.tex` & `LbNightlyTools-4.0.1/docs/note/requirements.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/title-LHCb-ANA.tex` & `LbNightlyTools-4.0.1/docs/note/title-LHCb-ANA.tex`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/note/unsrturl.bst` & `LbNightlyTools-4.0.1/docs/note/unsrturl.bst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/operation/Makefile` & `LbNightlyTools-4.0.1/docs/operation/Makefile`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/operation/NightlyBuildsOperation.html` & `LbNightlyTools-4.0.1/docs/operation/NightlyBuildsOperation.html`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/operation/NightlyBuildsOperation.rst` & `LbNightlyTools-4.0.1/docs/operation/NightlyBuildsOperation.rst`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/operation/images/jenkins-jobs.dot` & `LbNightlyTools-4.0.1/docs/operation/images/jenkins-jobs.dot`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/operation/images/jenkins-jobs.dot.png` & `LbNightlyTools-4.0.1/docs/operation/images/jenkins-jobs.dot.png`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/docs/pylint.rc` & `LbNightlyTools-4.0.1/docs/pylint.rc`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbMsg/BuildMsg.py` & `LbNightlyTools-4.0.1/python/LbMsg/BuildMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbMsg/Common.py` & `LbNightlyTools-4.0.1/python/LbMsg/Common.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbMsg/TestMsg.py` & `LbNightlyTools-4.0.1/python/LbMsg/TestMsg.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/ArtifactsServer.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/ArtifactsServer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/BuildLogScanner.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/BuildLogScanner.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/BuildMethods.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/BuildMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,30 +60,31 @@
 
     apptainer = which("apptainer")
     if not apptainer:
         return cmd
 
     image = None
     if re.match(r"x86_64.*-centos7-.*", platform):
-        image = "/cvmfs/cernvm-prod.cern.ch/cvm4"
+        image = "/cvmfs/lhcb.cern.ch/containers/os-base/centos7-devel/prod/amd64"
     elif re.match(r"x86_64.*-slc[56]-.*", platform):
-        image = "/cvmfs/cernvm-prod.cern.ch/cvm3"
+        image = "/cvmfs/lhcb.cern.ch/containers/os-base/slc6-devel/prod/amd64"
     elif re.match(r"x86_64.*-el9-.*", platform):
         image = "/cvmfs/lhcb.cern.ch/containers/os-base/alma9-devel/prod/amd64"
     elif re.match(r"arm.*-centos7-.*", platform):
         image = "/cvmfs/lhcb.cern.ch/containers/os-base/centos7-devel/prod/aarch64"
     elif re.match(r"arm.*-el9-.*", platform):
         image = "/cvmfs/lhcb.cern.ch/containers/os-base/alma9-devel/prod/aarch64"
 
     if not image:
         return cmd
 
     apptainer_cmd = [
         apptainer,
         "exec",
+        "--contain",
         "--bind",
         "/cvmfs",
         "--bind",
         "{}:{}".format(host_root, cont_root),
         # we bind host_root as itself to fix issues with non relocatable local conda environments
         "--bind",
         host_root,
@@ -122,14 +123,16 @@
     cont_root = "/workspace"
 
     # patch the environment for the wrapped command
     kwargs["env"] = {
         key: value.replace(host_root, cont_root)
         for key, value in (kwargs.get("env") or os.environ).items()
     }
+    # patch the command line arguments
+    cmd = [value.replace(host_root, cont_root) for value in cmd]
 
     cmd = _apptainer_wrap_cmd(
         os.environ["BINARY_TAG"],
         cmd,
         host_root,
         cont_root,
         env=kwargs["env"],
```

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/CheckSlotPreconditions.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/CheckSlotPreconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/CheckoutMethods.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/CheckoutMethods.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Configuration.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/GetNightlyRefs.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/GetNightlyRefs.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/GitlabUtils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/GitlabUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/HTMLUtils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/HTMLUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/LbScriptsUtils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/LbScriptsUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/MergeRequestBuilds.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/MergeRequestBuilds.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/ProcUtils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/ProcUtils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Repository.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Repository.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Build.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Checkout.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/CollectBuildLogs.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/CollectBuildLogs.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Common.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Common.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,15 @@
                         "JENKINS_OVERRIDE_PIP_REQUIREMENTS": os.environ.get(
                             "JENKINS_OVERRIDE_PIP_REQUIREMENTS"
                         ),
                         "JENKINS_RESET_VIRTUALENV": os.environ.get(
                             "JENKINS_RESET_VIRTUALENV"
                         ),
                         "env_hash": os.environ.get("env_hash"),
+                        "temp_env": os.environ.get("temp_env"),
                     },
                 }
             )
             return d
 
         self.dashboard.update("ready-builds", changes)
```

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/EnabledSlots.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/EnabledSlots.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/GitlabMR.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/GitlabMR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Index.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Index.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Install.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Install.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Preconditions.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Preconditions.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Release.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Release.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/Test.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/Test.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/__init__.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/_entry_points.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/extract.php` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/extract.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Scripts/listzip.php` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Scripts/listzip.php`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/Utils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/Utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/__init__.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/__init__.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_build.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_build_script.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_build_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_checkout.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_checkout_script.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_checkout_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_config_load.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_config_load.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_config_pickle.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_config_pickle.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_configuration.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_configuration_check.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_configuration_check.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_copytree.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_copytree.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_coverity_support.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_coverity_support.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_enabled_slots_script.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_enabled_slots_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_gitlab_mr_script.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_gitlab_mr_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_indexer.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_install.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_jobconfig.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_jobconfig.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_merge_request_builds.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_merge_request_builds.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_pack.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_precond.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_precond.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_rel_gen_script.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_rel_gen_script.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_release_poll.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_release_poll.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_repository.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_retry.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/test_utils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools/tests/utils.py` & `LbNightlyTools-4.0.1/python/LbNightlyTools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/SOURCES.txt` & `LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbNightlyTools.egg-info/entry_points.txt` & `LbNightlyTools-4.0.1/python/LbNightlyTools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPR/LbPRJobManager.py` & `LbNightlyTools-4.0.1/python/LbPR/LbPRJobManager.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPR/_entry_points.py` & `LbNightlyTools-4.0.1/python/LbPR/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicStarter.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicStarter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicTest.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicTest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/LbPeriodicTestSchedule.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/LbPeriodicTestSchedule.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/TestSchedule.xsd` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/TestSchedule.xsd`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/_entry_points.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_LHCbPR.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_LHCbPR.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_Starter.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_Starter.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbPeriodicTools/tests/test_XMLParsing.py` & `LbNightlyTools-4.0.1/python/LbPeriodicTools/tests/test_XMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbCompatSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbCompatSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbExternalsSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbExternalsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbGenericSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbGenericSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbLbScriptsSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbMetaSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbMetaSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/LHCbRPMSpecBuilder.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/LHCbRPMSpecBuilder.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/PackageSlot.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/PackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_ExternalSpec.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_ExternalSpec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_PackageSlot.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_PackageSlot.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbRPMTools/tests/test_Spec.py` & `LbNightlyTools-4.0.1/python/LbRPMTools/tests/test_Spec.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbTools/Manifest.py` & `LbNightlyTools-4.0.1/python/LbTools/Manifest.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbTools/__init__.py` & `LbNightlyTools-4.0.1/python/LbTools/__init__.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbTools/tests/test_XMLParsing.py` & `LbNightlyTools-4.0.1/python/LbTools/tests/test_XMLParsing.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/python/LbTools/tests/test_toolchain_info.py` & `LbNightlyTools-4.0.1/python/LbTools/tests/test_toolchain_info.py`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/scripts/lbn-get-configs` & `LbNightlyTools-4.0.1/scripts/lbn-get-configs`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/scripts/lbn-wrapcmd` & `LbNightlyTools-4.0.1/scripts/lbn-wrapcmd`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/scripts/lbpr-collect` & `LbNightlyTools-4.0.1/scripts/lbpr-collect`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/setup.py` & `LbNightlyTools-4.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,14 +86,19 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
     # keywords='LHCb Dirac LHCbDirac',  # Optional
     # You can just specify package directories manually here if your project is
@@ -101,17 +106,15 @@
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    packages=find_packages(
-        "python", exclude=["*.tests"] if version_info < (3, 0) else []
-    ),
+    packages=find_packages("python", exclude=["*.tests"]),
     package_dir={"": "python"},
     package_data={
         "LbPeriodicTools": ["TestSchedule.xsd"],
         "LbNightlyTools.Scripts": ["extract.php", "listzip.php"],
     },
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
@@ -120,14 +123,15 @@
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "LbEnv",
         "LbCommon>=0.0.7",
         "LbDevTools",
         "lbinstall",
+        "lbmessaging",
         "python-gitlab" + ("<2" if version_info < (3, 0) else ""),
         "pika==1.1.0",
         "CouchDB",
         "tabulate",
         "joblib",
         "GitPython" + ("<2.1.12" if version_info < (3, 0) else ""),
         "networkx" + ("<2.3" if version_info < (3, 0) else ""),
```

### Comparing `LbNightlyTools-4.0.0/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip` & `LbNightlyTools-4.0.1/testdata/artifacts/packs/src/TestProject.HEAD.testing-slot.src.zip`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/ci-test-hook-content.json` & `LbNightlyTools-4.0.1/testdata/ci-test-hook-content.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/collect_deps/cmake/conf.json` & `LbNightlyTools-4.0.1/testdata/collect_deps/cmake/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/collect_deps/cmt/conf.json` & `LbNightlyTools-4.0.1/testdata/collect_deps/cmt/conf.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/coverity/bin/cov-analyze` & `LbNightlyTools-4.0.1/testdata/coverity/bin/cov-analyze`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/coverity/bin/cov-build` & `LbNightlyTools-4.0.1/testdata/coverity/bin/cov-build`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/coverity/bin/cov-commit-defects` & `LbNightlyTools-4.0.1/testdata/coverity/bin/cov-commit-defects`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/periodic_tests/lhcbpr_schedule.xml` & `LbNightlyTools-4.0.1/testdata/periodic_tests/lhcbpr_schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/periodic_tests/schedule.xml` & `LbNightlyTools-4.0.1/testdata/periodic_tests/schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/periodic_tests/slotbuilds.json` & `LbNightlyTools-4.0.1/testdata/periodic_tests/slotbuilds.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/periodic_tests/starter_schedule.xml` & `LbNightlyTools-4.0.1/testdata/periodic_tests/starter_schedule.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/Brunel_v46r0.spec` & `LbNightlyTools-4.0.1/testdata/rpm/Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec` & `LbNightlyTools-4.0.1/testdata/rpm/Brunel_v46r0_x86_64-slc6-gcc48-opt.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec` & `LbNightlyTools-4.0.1/testdata/rpm/Gaudi_v27r0_x86_64-slc6-gcc49-do0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/LCG_68_externalsDict.json` & `LbNightlyTools-4.0.1/testdata/rpm/LCG_68_externalsDict.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/PARAM_TMVAWeights.spec` & `LbNightlyTools-4.0.1/testdata/rpm/PARAM_TMVAWeights.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/PARAM_TMVAWeights_rel5.spec` & `LbNightlyTools-4.0.1/testdata/rpm/PARAM_TMVAWeights_rel5.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/datapkg-slot-config.json` & `LbNightlyTools-4.0.1/testdata/rpm/datapkg-slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/glimpse_Brunel_v46r0.spec` & `LbNightlyTools-4.0.1/testdata/rpm/glimpse_Brunel_v46r0.spec`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/manifest.xml` & `LbNightlyTools-4.0.1/testdata/rpm/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/manifest_do0.xml` & `LbNightlyTools-4.0.1/testdata/rpm/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/slot-config.json` & `LbNightlyTools-4.0.1/testdata/rpm/slot-config.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/rpm/slot-configdo0.json` & `LbNightlyTools-4.0.1/testdata/rpm/slot-configdo0.json`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/tools/manifest.xml` & `LbNightlyTools-4.0.1/testdata/tools/manifest.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/tools/manifest_do0.xml` & `LbNightlyTools-4.0.1/testdata/tools/manifest_do0.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/tools/manifest_with_pkgs.xml` & `LbNightlyTools-4.0.1/testdata/tools/manifest_with_pkgs.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/testdata/tools/manifest_with_pkgs_new.xml` & `LbNightlyTools-4.0.1/testdata/tools/manifest_with_pkgs_new.xml`

 * *Files identical despite different names*

### Comparing `LbNightlyTools-4.0.0/utils/add_ci_webhook.py` & `LbNightlyTools-4.0.1/utils/add_ci_webhook.py`

 * *Files identical despite different names*


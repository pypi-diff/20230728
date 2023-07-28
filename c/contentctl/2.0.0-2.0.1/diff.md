# Comparing `tmp/contentctl-2.0.0.tar.gz` & `tmp/contentctl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-2.0.0.tar", max compression
+gzip compressed data, was "contentctl-2.0.1.tar", max compression
```

## Comparing `contentctl-2.0.0.tar` & `contentctl-2.0.1.tar`

### file list

```diff
@@ -1,132 +1,133 @@
--rw-r--r--   0        0        0    11344 2023-07-13 00:36:19.774439 contentctl-2.0.0/LICENSE.md
--rw-r--r--   0        0        0    17554 2023-07-13 00:36:19.774439 contentctl-2.0.0/README.md
--rw-r--r--   0        0        0       22 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/__init__.py
--rw-r--r--   0        0        0     2999 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/apav_deploy.py
--rw-r--r--   0        0        0     6963 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/api_deploy.py
--rw-r--r--   0        0        0     5580 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7180 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    16208 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/GitHubService.py
--rw-r--r--   0        0        0     2259 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    27462 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     4051 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      363 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3907 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1368 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4780 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     3348 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/generate.py
--rw-r--r--   0        0        0     3000 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0     1294 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/inspect.py
--rw-r--r--   0        0        0      920 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/new_content.py
--rw-r--r--   0        0        0     1022 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3014 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/test.py
--rw-r--r--   0        0        0     2741 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/validate.py
--rw-r--r--   0        0        0    15135 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/contentctl.py
--rw-r--r--   0        0        0     4392 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0     3242 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     3418 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0     1198 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     7238 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15586 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/utils.py
--rw-r--r--   0        0        0     1906 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2291 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    13759 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    11189 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4485 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     4576 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     2100 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0     4755 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/story_builder.py
--rw-r--r--   0        0        0     1016 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0     7699 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/app.py
--rw-r--r--   0        0        0     1930 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     5658 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/config.py
--rw-r--r--   0        0        0     3519 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/constants.py
--rw-r--r--   0        0        0     1136 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0     5630 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/detection.py
--rw-r--r--   0        0        0     5921 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     2882 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/enums.py
--rw-r--r--   0        0        0     2150 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0     1002 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/lookup.py
--rw-r--r--   0        0        0      845 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0      920 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6522 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0     1875 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     1531 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/story.py
--rw-r--r--   0        0        0     1213 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    22343 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/test_config.py
--rw-r--r--   0        0        0      805 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      580 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0     8186 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0      602 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_test.py
--rw-r--r--   0        0        0     3089 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     3946 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0    11388 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2958 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0     3238 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3050 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      210 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     3065 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     1059 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      586 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0     1011 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/app.conf.j2
--rw-r--r--   0        0        0      180 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0      670 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1432 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      177 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1474 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     5566 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1390 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0       90 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     1003 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon.png
--rw-r--r--   0        0        0     2222 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
--rw-r--r--   0        0        0     1416 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0      235 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0      133 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/README
--rw-r--r--   0        0        0     1293 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0     9381 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0     3312 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0     3508 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_test_fail.yml
--rw-r--r--   0        0        0     3391 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_validation_fail.yml
--rw-r--r--   0        0        0      159 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0     3095 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      949 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/splunk_app/metadata/app.conf.j2
--rw-r--r--   0        0        0       90 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0      796 2023-07-13 00:36:19.778439 contentctl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    18763 1970-01-01 00:00:00.000000 contentctl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-07-28 00:24:14.551601 contentctl-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0    17550 2023-07-28 00:24:14.551601 contentctl-2.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6963 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0     5580 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/detection_testing/DataManipulation.py
+-rw-r--r--   0        0        0     7180 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0    16208 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/detection_testing/GitHubService.py
+-rw-r--r--   0        0        0     2259 2023-07-28 00:24:14.551601 contentctl-2.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    27462 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     4051 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      363 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3907 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1368 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4780 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      857 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     3348 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/generate.py
+-rw-r--r--   0        0        0     3000 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0      920 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0     1022 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     3014 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2741 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    14622 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/contentctl.py
+-rw-r--r--   0        0        0     4392 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3242 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     1198 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/helper/config_handler.py
+-rw-r--r--   0        0        0     7238 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15586 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     1906 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/baseline_builder.py
+-rw-r--r--   0        0        0     2291 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/basic_builder.py
+-rw-r--r--   0        0        0    13759 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/detection_builder.py
+-rw-r--r--   0        0        0    11189 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/director.py
+-rw-r--r--   0        0        0     1244 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/investigation_builder.py
+-rw-r--r--   0        0        0     4485 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/new_content_generator.py
+-rw-r--r--   0        0        0     4576 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0     2100 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/playbook_builder.py
+-rw-r--r--   0        0        0     4755 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/story_builder.py
+-rw-r--r--   0        0        0     1016 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0     5518 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/abstract_security_content_objects/detection_abstract.py
+-rw-r--r--   0        0        0     1893 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
+-rw-r--r--   0        0        0     7753 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/app.py
+-rw-r--r--   0        0        0     1930 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0      711 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0     5658 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3518 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/constants.py
+-rw-r--r--   0        0        0     1136 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      141 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      164 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      201 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      111 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      193 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      129 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0     1454 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/detection.py
+-rw-r--r--   0        0        0     5921 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0     2882 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     2150 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0      191 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     1002 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0      845 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/macro.py
+-rw-r--r--   0        0        0      219 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0      920 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0      315 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     6522 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/repo_config.py
+-rw-r--r--   0        0        0      325 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     1531 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/story.py
+-rw-r--r--   0        0        0     1213 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0    22343 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/test_config.py
+-rw-r--r--   0        0        0      805 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      580 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      255 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0     8186 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0      602 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/objects/unit_test_test.py
+-rw-r--r--   0        0        0     3089 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     1701 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2130 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     3946 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    12344 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     2958 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0     3238 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3050 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1089 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0      210 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     3065 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     1059 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      745 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      496 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      586 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0     1011 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0      180 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0      670 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      671 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1002 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6586 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1822 2023-07-28 00:24:14.555601 contentctl-2.0.1/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0      994 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      369 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1432 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      177 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      424 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      282 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/macros_detections.j2
+-rw-r--r--   0        0        0      221 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1474 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     5566 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1390 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0       90 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0     1003 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/splunk_app/static/appIcon.png
+-rw-r--r--   0        0        0     2222 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/splunk_app/static/appIcon_2x.png
+-rw-r--r--   0        0        0     1416 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0      235 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/README
+-rw-r--r--   0        0        0     1293 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0     9381 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0     3312 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0     3508 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip_test_fail.yml
+-rw-r--r--   0        0        0     3391 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip_validation_fail.yml
+-rw-r--r--   0        0        0      159 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3095 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      949 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/stories/splunk_app/metadata/app.conf.j2
+-rw-r--r--   0        0        0       90 2023-07-28 00:24:14.559601 contentctl-2.0.1/contentctl/templates/stories/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0      797 2023-07-28 00:24:14.559601 contentctl-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    18714 1970-01-01 00:00:00.000000 contentctl-2.0.1/PKG-INFO
```

### Comparing `contentctl-2.0.0/LICENSE.md` & `contentctl-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/README.md` & `contentctl-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,22 +71,22 @@
 | Python 3.11 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions)  |
 | Docker (local) | Yes | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |
 | Docker (remote) | Planned | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | No |
 
 
 
 **Because contentctl uses a large number of dependencies, it's recommended to install contentctl in a virtual environment. 
-The instructions below use "poetry" and follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
+The instructions below using "poetry" ALSO follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
 It is typically recommended to install poetry to the Global Python Environment.**
 
-#### Install via pip (coming soon): 
+#### Install via pip (recommended): 
 ```
 python3.9 -m venv .venv
 source .venv/bin/activate
-pip install splunk-contentctl
+pip install contentctl
 ```
 
 #### From Source (advanced)
 ```
 git clone https://github.com/splunk/contentctl
 cd contentctl
 python3.9 -m pip install poetry
```

### Comparing `contentctl-2.0.0/contentctl/actions/apav_deploy.py` & `contentctl-2.0.1/contentctl/actions/apav_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/api_deploy.py` & `contentctl-2.0.1/contentctl/actions/api_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/DataManipulation.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/DataManipulation.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/GitHubService.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/GitHubService.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class DetectionTestingManagerOutputDto:
     inputQueue: list[Detection] = Field(default_factory=list)
     outputQueue: list[Detection] = Field(default_factory=list)
     currentTestingQueue: dict[str, Union[Detection, None]] = Field(default_factory=dict)
     start_time: Union[datetime.datetime, None] = None
     replay_index: str = "CONTENTCTL_TESTING_INDEX"
     replay_host: str = "CONTENTCTL_HOST"
-    timeout_seconds: int = 15
+    timeout_seconds: int = 60
     terminate: bool = False
 
 
 class DetectionTestingInfrastructure(BaseModel, abc.ABC):
     # thread: threading.Thread = threading.Thread()
     config: TestConfig
     sync_obj: DetectionTestingManagerOutputDto
```

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-2.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/doc_gen.py` & `contentctl-2.0.1/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/generate.py` & `contentctl-2.0.1/contentctl/actions/generate.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/initialize.py` & `contentctl-2.0.1/contentctl/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/initialize_old.py` & `contentctl-2.0.1/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/new_content.py` & `contentctl-2.0.1/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/reporting.py` & `contentctl-2.0.1/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/test.py` & `contentctl-2.0.1/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/actions/validate.py` & `contentctl-2.0.1/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/contentctl.py` & `contentctl-2.0.1/contentctl/contentctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     DirectorOutputDto,
     Generate,
 )
 from contentctl.actions.reporting import ReportingInputDto, Reporting
 from contentctl.actions.new_content import NewContentInputDto, NewContent
 from contentctl.actions.doc_gen import DocGenInputDto, DocGen
 from contentctl.actions.initialize import Initialize, InitializeInputDto
-from contentctl.actions.inspect import InspectInputDto, Inspect
 from contentctl.actions.api_deploy import API_Deploy, API_DeployInputDto
 
 from contentctl.input.director import DirectorInputDto
 from contentctl.objects.enums import (
     SecurityContentType,
     SecurityContentProduct,
     DetectionTestingMode,
@@ -112,22 +111,14 @@
     generate_input_dto = GenerateInputDto(director_input_dto)
 
     generate = Generate()
 
     return generate.execute(generate_input_dto)
 
 
-def inspect(args) -> None:
-    config=start(args)
-    app_path = pathlib.Path(config.build.path_root)/f"{config.build.name}.tar.gz"
-    input_dto = InspectInputDto(path=app_path)
-    i = Inspect()
-    i.execute(input_dto=input_dto)
-
-
 def api_deploy(args) -> None:
     config = start(args)
     deploy_input_dto = API_DeployInputDto(path=pathlib.Path(args.path), config=config)
     deploy = API_Deploy()
     
     deploy.execute(deploy_input_dto)
 
@@ -166,14 +157,15 @@
         appid=config.build.name,
         title=config.build.name,
         release=config.build.version,
         http_path=None,
         local_path=str(pathlib.Path(config.build.path_root)/f"{config.build.name}.tar.gz"),
         description=config.build.description,
         splunkbase_path=None,
+        force_local=True
     )
 
     # We need to do this instead of appending to retrigger validation.
     # It does not happen the first time since validation does not run for default values
     # unless we use always=True in the validator
     # we always want to keep CIM as the last app installed
 
@@ -334,23 +326,15 @@
         type=str,
         help="Type of security content object, choose between `detection`, `story`",
     )
     new_content_parser.set_defaults(func=new_content)
 
     reporting_parser.set_defaults(func=reporting)
 
-    inspect_parser.add_argument(
-        "-ap",
-        "--app_path",
-        required=False,
-        type=str,
-        default=None,
-        help="path to the Splunk app to be inspected",
-    )
-    inspect_parser.set_defaults(func=inspect)
+
 
     api_deploy_parser.set_defaults(func=api_deploy)
 
     test_parser.add_argument(
         "--mode",
         required=False,
         default=DetectionTestingMode.all.name,
```

### Comparing `contentctl-2.0.0/contentctl/enrichments/attack_enrichment.py` & `contentctl-2.0.1/contentctl/enrichments/attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/enrichments/cve_enrichment.py` & `contentctl-2.0.1/contentctl/enrichments/cve_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-2.0.1/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/helper/config_handler.py` & `contentctl-2.0.1/contentctl/helper/config_handler.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/helper/link_validator.py` & `contentctl-2.0.1/contentctl/helper/link_validator.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/helper/utils.py` & `contentctl-2.0.1/contentctl/helper/utils.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/baseline_builder.py` & `contentctl-2.0.1/contentctl/input/baseline_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/basic_builder.py` & `contentctl-2.0.1/contentctl/input/basic_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/detection_builder.py` & `contentctl-2.0.1/contentctl/input/detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/director.py` & `contentctl-2.0.1/contentctl/input/director.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/investigation_builder.py` & `contentctl-2.0.1/contentctl/input/investigation_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/new_content_generator.py` & `contentctl-2.0.1/contentctl/input/new_content_generator.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/new_content_questions.py` & `contentctl-2.0.1/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/playbook_builder.py` & `contentctl-2.0.1/contentctl/input/playbook_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/story_builder.py` & `contentctl-2.0.1/contentctl/input/story_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/input/yml_reader.py` & `contentctl-2.0.1/contentctl/input/yml_reader.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/app.py` & `contentctl-2.0.1/contentctl/objects/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,28 +40,29 @@
     # Splunkbase path is made of the combination of uid and release fields
     splunkbase_path: Union[str, None]
 
     # Ultimate source of the app. Can be a local path or a Splunkbase Path.
     # This will be set via a function call and should not be provided in the YML
     # Note that this is the path relative to the container mount
     environment_path: str = ENVIRONMENT_PATH_NOT_SET
+    force_local:bool = False
 
     def configure_app_source_for_container(
         self,
         splunkbase_username: Union[str, None],
         splunkbase_password: Union[str, None],
         apps_directory: pathlib.Path,
         container_mount_path: pathlib.Path,
     ):
 
         splunkbase_creds_provided = (
             splunkbase_username is not None and splunkbase_password is not None
         )
 
-        if splunkbase_creds_provided and self.splunkbase_path is not None:
+        if splunkbase_creds_provided and self.splunkbase_path is not None and not self.force_local:
             self.environment_path = self.splunkbase_path
 
         elif self.local_path is not None:
             # local path existence already validated
             filename = pathlib.Path(self.local_path)
             destination = str(apps_directory / filename.name)
             Utils.copy_local_file(self.local_path, destination, verbose_print=True)
```

### Comparing `contentctl-2.0.0/contentctl/objects/baseline.py` & `contentctl-2.0.1/contentctl/objects/baseline.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/baseline_tags.py` & `contentctl-2.0.1/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/config.py` & `contentctl-2.0.1/contentctl/objects/config.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/constants.py` & `contentctl-2.0.1/contentctl/objects/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     "MAC Address": 3,
     "User Name": 4,
     "Email Address": 5,
     "URL String": 6,
     "File Name": 7,
     "File Hash": 8,
     "Process Name": 9,
-    "Ressource UID": 10,
+    "Resource UID": 10,
     "Endpoint": 20,
     "User": 21,
     "Email": 22,
     "Uniform Resource Locator": 23,
     "File": 24,
     "Process": 25,
     "Geo Location": 26,
```

### Comparing `contentctl-2.0.0/contentctl/objects/deployment.py` & `contentctl-2.0.1/contentctl/objects/deployment.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/detection.py` & `contentctl-2.0.1/contentctl/objects/abstract_security_content_objects/detection_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,18 @@
 from contentctl.objects.lookup import Lookup
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.playbook import Playbook
 from contentctl.helper.link_validator import LinkValidator
 from contentctl.objects.enums import SecurityContentType
 
 
-class Detection(SecurityContentObject):
-    # detection spec
-    #name: str
-    #id: str
-    #version: int
-    #date: str
-    #author: str
+class Detection_Abstract(SecurityContentObject):
     contentType: SecurityContentType = SecurityContentType.detections
     type: str
     status: DetectionStatus
-    #description: str
     data_source: list[str]
     search: Union[str, dict]
     how_to_implement: str
     known_false_positives: str
     check_references: bool = False  
     references: list
     tags: DetectionTags
```

### Comparing `contentctl-2.0.0/contentctl/objects/detection_tags.py` & `contentctl-2.0.1/contentctl/objects/detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/enums.py` & `contentctl-2.0.1/contentctl/objects/enums.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/investigation.py` & `contentctl-2.0.1/contentctl/objects/investigation.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/lookup.py` & `contentctl-2.0.1/contentctl/objects/lookup.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/macro.py` & `contentctl-2.0.1/contentctl/objects/macro.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/playbook.py` & `contentctl-2.0.1/contentctl/objects/playbook.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/repo_config.py` & `contentctl-2.0.1/contentctl/objects/repo_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/security_content_object.py` & `contentctl-2.0.1/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import string
 import uuid
 from datetime import datetime
 from pydantic import BaseModel, validator, ValidationError
 from contentctl.objects.enums import SecurityContentType
 
 
-class SecurityContentObject(BaseModel, abc.ABC):
+class SecurityContentObject_Abstract(BaseModel, abc.ABC):
     contentType: SecurityContentType
     name: str
     author: str = "UNKNOWN_AUTHOR"
     date: str = "1990-01-01"
     version: int = 99999
     id: str = None
     description: str = "UNKNOWN_DESCRIPTION"
@@ -53,8 +53,8 @@
             v.encode('ascii')
         except UnicodeEncodeError:
             raise ValueError('encoding error in ' + field.name + ': ' + values["name"])
         return v
     
     @validator('description')
     def description_valid(cls, v, values, field):
-        return SecurityContentObject.free_text_field_valid(cls,v,values,field)
+        return SecurityContentObject_Abstract.free_text_field_valid(cls,v,values,field)
```

### Comparing `contentctl-2.0.0/contentctl/objects/story.py` & `contentctl-2.0.1/contentctl/objects/story.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/story_tags.py` & `contentctl-2.0.1/contentctl/objects/story_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/test_config.py` & `contentctl-2.0.1/contentctl/objects/test_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/unit_test.py` & `contentctl-2.0.1/contentctl/objects/unit_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/unit_test_attack_data.py` & `contentctl-2.0.1/contentctl/objects/unit_test_attack_data.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/unit_test_result.py` & `contentctl-2.0.1/contentctl/objects/unit_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/objects/unit_test_test.py` & `contentctl-2.0.1/contentctl/objects/unit_test_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/api_json_output.py` & `contentctl-2.0.1/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/attack_nav_output.py` & `contentctl-2.0.1/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/attack_nav_writer.py` & `contentctl-2.0.1/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/ba_yml_output.py` & `contentctl-2.0.1/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/conf_output.py` & `contentctl-2.0.1/contentctl/output/conf_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 import glob
 import shutil
 import sys
 import tarfile
 from typing import Union
 from pathlib import Path
 import pathlib
-from splunk_appinspect.main import (
-    validate, MODE_OPTION, APP_PACKAGE_ARGUMENT, OUTPUT_FILE_OPTION, 
-    LOG_FILE_OPTION, INCLUDED_TAGS_OPTION, EXCLUDED_TAGS_OPTION, 
-    PRECERT_MODE, TEST_MODE)
+
 import shutil
 from contentctl.output.conf_writer import ConfWriter
 from contentctl.objects.enums import SecurityContentType
 from contentctl.objects.config import Config
 
 
 class ConfOutput:
@@ -171,14 +168,31 @@
     
     def inspectApp(self)-> None:
         
         output_app_expected_name = pathlib.Path(self.config.build.path_root)/f"{self.config.build.name}-{self.config.build.version}.tar.gz"
         name_without_version = pathlib.Path(self.config.build.path_root)/f"{self.config.build.name}.tar.gz"
         shutil.copy2(output_app_expected_name, name_without_version, follow_symlinks=False)
         
+        try:
+            from splunk_appinspect.main import (
+                validate, MODE_OPTION, APP_PACKAGE_ARGUMENT, OUTPUT_FILE_OPTION, 
+                LOG_FILE_OPTION, INCLUDED_TAGS_OPTION, EXCLUDED_TAGS_OPTION, 
+                PRECERT_MODE, TEST_MODE)
+        except Exception as e:
+            print("******WARNING******")
+            if sys.version_info.major == 3 and sys.version_info.minor == 9:
+                print("The package splunk-appinspect was not installed due to a current issue with the library on Python3.10+.  "
+                      "Please use the following commands to set up a virtualenvironment in a different folder so you may run appinspect manually:"
+                      f"\n\tpython3.9 -m venv .venv; source .venv/bin/activate; python3 -m pip install splunk-appinspect; splunk-appinspect inspect {name_without_version} --mode precert")    
+                
+            else:
+                print("splunk-appinspect is only compatable with Python3.9 at this time.  Please see the following open issue here: https://github.com/splunk/contentctl/issues/28")
+            print("******WARNING******")
+            return
+
         # Note that all tags are available and described here:
         # https://dev.splunk.com/enterprise/reference/appinspect/appinspecttagreference/ 
         # By default, precert mode will run ALL checks.  Explicitly included or excluding tags will 
         # change this behavior. To give the most thorough inspection, we leave these empty so that
         # ALL checks are run
         included_tags = []
         excluded_tags = []
```

### Comparing `contentctl-2.0.0/contentctl/output/conf_writer.py` & `contentctl-2.0.1/contentctl/output/conf_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/doc_md_output.py` & `contentctl-2.0.1/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/finding_report_writer.py` & `contentctl-2.0.1/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/jinja_writer.py` & `contentctl-2.0.1/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/new_content_yml_output.py` & `contentctl-2.0.1/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/svg_output.py` & `contentctl-2.0.1/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-2.0.1/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-2.0.1/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/app.conf.j2` & `contentctl-2.0.1/contentctl/output/templates/app.conf.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/detection_count.j2` & `contentctl-2.0.1/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/detection_coverage.j2` & `contentctl-2.0.1/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_detection_page.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_detections.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_navigation.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_playbooks.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_stories.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/doc_story_page.j2` & `contentctl-2.0.1/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-2.0.1/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/finding_report.j2` & `contentctl-2.0.1/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-2.0.1/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-2.0.1/contentctl/output/templates/savedsearches_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-2.0.1/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon.png` & `contentctl-2.0.1/contentctl/output/templates/splunk_app/static/appIcon.png`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png` & `contentctl-2.0.1/contentctl/output/templates/splunk_app/static/appIcon_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/transforms.j2` & `contentctl-2.0.1/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/output/templates/workflow_actions.j2` & `contentctl-2.0.1/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/app_default.yml` & `contentctl-2.0.1/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/datamodels_cim.conf` & `contentctl-2.0.1/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_test_fail.yml` & `contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip_test_fail.yml`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_validation_fail.yml` & `contentctl-2.0.1/contentctl/templates/detections/anomalous_usage_of_7zip_validation_fail.yml`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-2.0.1/contentctl/templates/stories/cobalt_strike.yml`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/contentctl/templates/stories/splunk_app/metadata/app.conf.j2` & `contentctl-2.0.1/contentctl/templates/stories/splunk_app/metadata/app.conf.j2`

 * *Files identical despite different names*

### Comparing `contentctl-2.0.0/pyproject.toml` & `contentctl-2.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "contentctl"
-version = "2.0.0"
+version = "2.0.1"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.11"
-PyYAML = "<6.0"
+PyYAML = "^6.0"
 requests = "^2.28.1"
 pycvesearch = "^1.2"
 xmltodict = "^0.13.0"
 attackcti = "^0.3.7"
 Jinja2 = "^3.1.2"
 questionary = "^1.10.0"
 gitpython = "^3.1.29"
 docker = "^6.0.1"
 splunk-sdk = "^1.7.2"
 validators = "^0.20.0"
 semantic-version = "^2.10.0"
 bottle = "^0.12.23"
 tqdm = "^4.65.0"
-splunk-appinspect = "^2.36.0"
+#splunk-appinspect = "^2.36.0"
 splunk-packaging-toolkit = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contentctl-2.0.0/PKG-INFO` & `contentctl-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: PyYAML (<6.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: attackcti (>=0.3.7,<0.4.0)
 Requires-Dist: bottle (>=0.12.23,<0.13.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: gitpython (>=3.1.29,<4.0.0)
 Requires-Dist: pycvesearch (>=1.2,<2.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: splunk-appinspect (>=2.36.0,<3.0.0)
 Requires-Dist: splunk-packaging-toolkit (>=1.0.1,<2.0.0)
 Requires-Dist: splunk-sdk (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
@@ -103,22 +102,22 @@
 | Python 3.11 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions)  |
 | Docker (local) | Yes | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |
 | Docker (remote) | Planned | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | No |
 
 
 
 **Because contentctl uses a large number of dependencies, it's recommended to install contentctl in a virtual environment. 
-The instructions below use "poetry" and follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
+The instructions below using "poetry" ALSO follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
 It is typically recommended to install poetry to the Global Python Environment.**
 
-#### Install via pip (coming soon): 
+#### Install via pip (recommended): 
 ```
 python3.9 -m venv .venv
 source .venv/bin/activate
-pip install splunk-contentctl
+pip install contentctl
 ```
 
 #### From Source (advanced)
 ```
 git clone https://github.com/splunk/contentctl
 cd contentctl
 python3.9 -m pip install poetry
```


# Comparing `tmp/phrase-api-1.9.0.tar.gz` & `tmp/phrase-api-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phrase-api-1.9.0.tar", last modified: Thu Apr 13 13:43:13 2023, max compression
+gzip compressed data, was "phrase-api-1.9.1.tar", last modified: Fri Jul 28 08:54:23 2023, max compression
```

## Comparing `phrase-api-1.9.0.tar` & `phrase-api-1.9.1.tar`

### file list

```diff
@@ -1,516 +1,516 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.666182 phrase-api-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-13 13:43:13.666182 phrase-api-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53148 2023-04-13 13:43:07.000000 phrase-api-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.510182 phrase-api-1.9.0/phrase_api/
--rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.530182 phrase-api-1.9.0/phrase_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/authorizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/bitbucket_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/blacklisted_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45255 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/branches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32592 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/distributions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/documents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/formats_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/git_hub_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45692 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/git_lab_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/glossaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26023 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/glossary_term_translations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36713 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/glossary_terms_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/icu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47616 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/invitations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36032 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/job_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60409 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/job_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39596 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/job_template_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/job_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    87790 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    77606 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    56195 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/members_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/notification_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33244 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39935 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/organization_job_template_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33993 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/organization_job_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43074 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/releases_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/screenshot_markers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/screenshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52346 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/spaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32432 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/style_guides_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    72438 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   128333 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/translations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/variables_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/versions___history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/webhook_deliveries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37755 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.594182 phrase-api-1.9.0/phrase_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/account_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/account_search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/affected_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/affected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/authorization_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/authorization_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/authorization_with_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/authorization_with_token1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/bitbucket_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/bitbucket_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/bitbucket_sync_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/bitbucket_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/blacklisted_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/blacklisted_key_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/blacklisted_key_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/branch_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/branch_merge_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/branch_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/branch_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/comment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/comment_mark_read_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/comment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/distribution_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/distribution_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/distribution_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/github_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/github_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/gitlab_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/gitlab_sync_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/gitlab_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/gitlab_sync_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/gitlab_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term_translation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term_translation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_term_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/glossary_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/icu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/icu_skeleton_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/inline_response422.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/inline_response422_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/invitation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/invitation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/invitation_update_settings_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_comment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_comment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_complete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_keys_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locale_complete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locale_complete_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locale_reopen_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_reopen_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_start_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_template_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/job_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/key_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/key_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/key_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/keys_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/keys_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/keys_search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/keys_tag_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/keys_untag_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_preview1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_team_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/locale_user_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member_project_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member_project_detail_project_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/member_update_settings_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/notification_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/notification_group_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/order_confirm_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/order_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/organization_job_template_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35444 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_locales1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_member_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_short.py
--rw-r--r--   0 runner    (1001) docker     (123)    34249 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/project_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/release_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/release_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/release_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot_marker_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot_marker_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/screenshot_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/search_in_account_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/space1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/space_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/space_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/spaces_projects_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide.py
--rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/styleguide_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag_with_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag_with_stats1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag_with_stats1_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/tag_with_stats1_statistics1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/team_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/team_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/team_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/team_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/teams_projects_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/teams_spaces_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/teams_users_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_key_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_key_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_unverify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_version_with_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translation_version_with_user1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_unverify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/translations_verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/upload_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/upload_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/user_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/variable_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/variable_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/webhook_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/webhook_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/models/webhook_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-04-13 13:43:07.000000 phrase-api-1.9.0/phrase_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.514181 phrase-api-1.9.0/phrase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-13 13:43:13.000000 phrase-api-1.9.0/phrase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-04-13 13:43:13.000000 phrase-api-1.9.0/phrase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:43:13.000000 phrase-api-1.9.0/phrase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 13:43:13.000000 phrase-api-1.9.0/phrase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 13:43:13.000000 phrase-api-1.9.0/phrase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 13:43:13.666182 phrase-api-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-13 13:43:07.000000 phrase-api-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:43:13.666182 phrase-api-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_account_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_account_search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_affected_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_affected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorization_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorization_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorization_with_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorization_with_token1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_authorizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_bitbucket_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_bitbucket_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_bitbucket_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_bitbucket_sync_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_bitbucket_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_blacklisted_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_blacklisted_key_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_blacklisted_key_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_blacklisted_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branch_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branch_merge_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branch_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branch_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_branches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_comment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_comment_mark_read_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_comment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_distribution_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_distribution_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_distribution_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_distributions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_formats_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_git_hub_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_git_lab_sync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_github_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_github_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_gitlab_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_gitlab_sync_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_gitlab_sync_export_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_gitlab_sync_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_gitlab_sync_import_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_translation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_translation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_translations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_term_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_terms_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_glossary_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_icu.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_icu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_icu_skeleton_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_inline_response422.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_inline_response422_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_invitation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_invitation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_invitation_update_settings_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_invitations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_comment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_comment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_complete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_keys_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locale_complete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locale_complete_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locale_reopen_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_reopen_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_start_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_template_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_job_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_key_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_key_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_key_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_tag_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_keys_untag_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_preview1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_team_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locale_user_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member_project_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member_project_detail_project_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_member_update_settings_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_members_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_notification_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_notification_group_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_notification_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_order_confirm_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_order_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_locale_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_locales_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_locales_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_template_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_organization_job_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_locales1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_member_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_project_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_release_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_release_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_release_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_releases_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_marker_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_marker_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_markers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshot_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_screenshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_search_in_account_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_space1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_space_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_space_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_spaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_spaces_projects_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_style_guides_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_styleguide_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag_with_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag_with_stats1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag_with_stats1_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tag_with_stats1_statistics1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_team_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_team_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_team_short.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_team_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_teams_projects_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_teams_spaces_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_teams_users_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_key_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_key_details1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_unverify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_version_with_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translation_version_with_user1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_exclude_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_include_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_review_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_unverify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_translations_verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_upload_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_upload_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_user_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_variable_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_variable_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_variables_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_versions___history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhook_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhook_deliveries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhook_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhook_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 13:43:07.000000 phrase-api-1.9.0/test/test_webhooks_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.085735 phrase-api-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 08:54:23.085735 phrase-api-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53238 2023-07-28 08:54:16.000000 phrase-api-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.009735 phrase-api-1.9.1/phrase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.017735 phrase-api-1.9.1/phrase_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/authorizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/bitbucket_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/blacklisted_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45255 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/branches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32592 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/distributions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/formats_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/git_hub_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45692 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/git_lab_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/glossaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26023 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/glossary_term_translations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36713 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/glossary_terms_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/icu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47616 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36032 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/job_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60543 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/job_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39596 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/job_template_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/job_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87790 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77606 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56155 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/members_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/notification_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33244 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39935 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/organization_job_template_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33993 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/organization_job_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43074 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/screenshot_markers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/screenshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52404 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/spaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32432 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/style_guides_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72474 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128333 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/translations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/variables_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/versions___history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/webhook_deliveries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37755 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.049735 phrase-api-1.9.1/phrase_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/account_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/account_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/affected_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/affected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/authorization_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/authorization_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/authorization_with_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/authorization_with_token1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/bitbucket_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/bitbucket_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/bitbucket_sync_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/bitbucket_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/blacklisted_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/blacklisted_key_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/blacklisted_key_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/branch_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/branch_merge_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/branch_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/branch_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/comment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/comment_mark_read_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/comment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/distribution_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/distribution_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/distribution_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/github_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/github_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/gitlab_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/gitlab_sync_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/gitlab_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/gitlab_sync_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/gitlab_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term_translation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term_translation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_term_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/glossary_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/icu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/icu_skeleton_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/inline_response422.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/inline_response422_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/invitation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/invitation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/invitation_update_settings_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_comment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_comment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_complete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_keys_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locale_complete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locale_complete_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locale_reopen_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_reopen_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_start_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_template_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/job_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/key_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/key_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/key_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/keys_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/keys_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/keys_search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/keys_tag_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/keys_untag_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_preview1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_team_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/locale_user_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member_project_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member_project_detail_project_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/member_update_settings_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/notification_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/notification_group_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/order_confirm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/order_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/organization_job_template_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35444 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_locales1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_member_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34249 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/project_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/release_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/release_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/release_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot_marker_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot_marker_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/screenshot_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/search_in_account_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/space1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/space_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/space_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/spaces_projects_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/styleguide_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag_with_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag_with_stats1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag_with_stats1_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/tag_with_stats1_statistics1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/team_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/team_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/team_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/team_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/teams_projects_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/teams_spaces_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/teams_users_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_key_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_key_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_unverify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_version_with_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translation_version_with_user1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_unverify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/translations_verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/upload_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/upload_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/user_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/variable_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/variable_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/webhook_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/webhook_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/models/webhook_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-07-28 08:54:16.000000 phrase-api-1.9.1/phrase_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.009735 phrase-api-1.9.1/phrase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 08:54:22.000000 phrase-api-1.9.1/phrase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-28 08:54:23.000000 phrase-api-1.9.1/phrase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:54:22.000000 phrase-api-1.9.1/phrase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 08:54:22.000000 phrase-api-1.9.1/phrase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:54:22.000000 phrase-api-1.9.1/phrase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 08:54:23.089735 phrase-api-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-28 08:54:16.000000 phrase-api-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:54:23.085735 phrase-api-1.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_account_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_account_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_affected_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_affected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorization_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorization_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorization_with_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorization_with_token1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_authorizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_bitbucket_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_bitbucket_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_bitbucket_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_bitbucket_sync_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_bitbucket_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_blacklisted_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_blacklisted_key_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_blacklisted_key_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_blacklisted_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branch_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branch_merge_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branch_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branch_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_branches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_comment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_comment_mark_read_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_comment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_distribution_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_distribution_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_distribution_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_distributions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_formats_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_git_hub_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_git_lab_sync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_github_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_github_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_gitlab_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_gitlab_sync_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_gitlab_sync_export_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_gitlab_sync_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_gitlab_sync_import_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_translation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_translation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_translations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_term_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_terms_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_glossary_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_icu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_icu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_icu_skeleton_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_inline_response422.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_inline_response422_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_invitation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_invitation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_invitation_update_settings_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_comment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_comment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_complete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_keys_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locale_complete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locale_complete_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locale_reopen_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_reopen_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_start_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_template_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_job_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_key_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_key_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_key_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_tag_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_keys_untag_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_preview1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_team_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locale_user_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member_project_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member_project_detail_project_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_member_update_settings_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_members_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_notification_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_notification_group_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_notification_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_order_confirm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_order_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_locale_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_locales_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_locales_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_template_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_organization_job_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_locales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_locales1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_member_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_project_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_release_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_release_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_release_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_marker_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_marker_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_markers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshot_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_screenshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_search_in_account_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_space1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_space_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_space_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_spaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_spaces_projects_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_style_guides_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_styleguide_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag_with_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag_with_stats1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag_with_stats1_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tag_with_stats1_statistics1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_team_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_team_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_team_short.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_team_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_teams_projects_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_teams_spaces_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_teams_users_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_key_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_key_details1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_unverify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_version_with_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translation_version_with_user1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_exclude_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_include_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_review_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_unverify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_translations_verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_upload_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_upload_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_user_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_variable_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_variable_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_variables_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_versions___history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhook_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhook_deliveries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhook_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhook_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-28 08:54:16.000000 phrase-api-1.9.1/test/test_webhooks_api.py
```

### Comparing `phrase-api-1.9.0/PKG-INFO` & `phrase-api-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phrase-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: Phrase Strings API Reference
 Home-page: https://github.com/phrase/phrase-python
 Author: Phrase Support
 Author-email: support@phrase.com
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Phrase Strings API Reference
```

### Comparing `phrase-api-1.9.0/README.md` & `phrase-api-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # phrase-api
 
 Phrase Strings is a translation management platform for software projects. You can collaborate on language file translation with your team or order translations through our platform. The API allows you to import locale files, download locale files, tag keys or interact in other ways with the localization data stored in Phrase Strings for your account.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://developers.phrase.com/api/](https://developers.phrase.com/api/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -216,20 +216,20 @@
 *JobCommentsApi* | [**job_comment_create**](docs/JobCommentsApi.md#job_comment_create) | **POST** /projects/{project_id}/jobs/{job_id}/comments | Create a job comment
 *JobCommentsApi* | [**job_comment_delete**](docs/JobCommentsApi.md#job_comment_delete) | **DELETE** /projects/{project_id}/jobs/{job_id}/comments/{id} | Delete a job comment
 *JobCommentsApi* | [**job_comment_show**](docs/JobCommentsApi.md#job_comment_show) | **GET** /projects/{project_id}/jobs/{job_id}/comments/{id} | Get a single job comment
 *JobCommentsApi* | [**job_comment_update**](docs/JobCommentsApi.md#job_comment_update) | **PATCH** /projects/{project_id}/jobs/{job_id}/comments/{id} | Update a job comment
 *JobCommentsApi* | [**job_comments_list**](docs/JobCommentsApi.md#job_comments_list) | **GET** /projects/{project_id}/jobs/{job_id}/comments | List job comments
 *JobLocalesApi* | [**job_locale_complete**](docs/JobLocalesApi.md#job_locale_complete) | **POST** /projects/{project_id}/jobs/{job_id}/locales/{id}/complete | Complete a job locale
 *JobLocalesApi* | [**job_locale_complete_review**](docs/JobLocalesApi.md#job_locale_complete_review) | **POST** /projects/{project_id}/jobs/{job_id}/locales/{id}/complete_review | Review a job locale
-*JobLocalesApi* | [**job_locale_delete**](docs/JobLocalesApi.md#job_locale_delete) | **DELETE** /projects/{project_id}/jobs/{job_id}/locales/{id} | Delete a job locale
+*JobLocalesApi* | [**job_locale_delete**](docs/JobLocalesApi.md#job_locale_delete) | **DELETE** /projects/{project_id}/jobs/{job_id}/locales/{id} | Remove a target locale from a job
 *JobLocalesApi* | [**job_locale_reopen**](docs/JobLocalesApi.md#job_locale_reopen) | **POST** /projects/{project_id}/jobs/{job_id}/locales/{id}/reopen | Reopen a job locale
-*JobLocalesApi* | [**job_locale_show**](docs/JobLocalesApi.md#job_locale_show) | **GET** /projects/{project_id}/jobs/{job_id}/locales/{id} | Get a single job locale
-*JobLocalesApi* | [**job_locale_update**](docs/JobLocalesApi.md#job_locale_update) | **PATCH** /projects/{project_id}/jobs/{job_id}/locales/{id} | Update a job locale
-*JobLocalesApi* | [**job_locales_create**](docs/JobLocalesApi.md#job_locales_create) | **POST** /projects/{project_id}/jobs/{job_id}/locales | Create a job locale
-*JobLocalesApi* | [**job_locales_list**](docs/JobLocalesApi.md#job_locales_list) | **GET** /projects/{project_id}/jobs/{job_id}/locales | List job locales
+*JobLocalesApi* | [**job_locale_show**](docs/JobLocalesApi.md#job_locale_show) | **GET** /projects/{project_id}/jobs/{job_id}/locales/{id} | Show single job target locale
+*JobLocalesApi* | [**job_locale_update**](docs/JobLocalesApi.md#job_locale_update) | **PATCH** /projects/{project_id}/jobs/{job_id}/locales/{id} | Update a job target locale
+*JobLocalesApi* | [**job_locales_create**](docs/JobLocalesApi.md#job_locales_create) | **POST** /projects/{project_id}/jobs/{job_id}/locales | Add a target locale to a job
+*JobLocalesApi* | [**job_locales_list**](docs/JobLocalesApi.md#job_locales_list) | **GET** /projects/{project_id}/jobs/{job_id}/locales | List job target locales
 *JobTemplateLocalesApi* | [**job_template_locale_delete**](docs/JobTemplateLocalesApi.md#job_template_locale_delete) | **DELETE** /projects/{project_id}/job_templates/{job_template_id}/locales/{job_template_locale_id} | Delete a job template locale
 *JobTemplateLocalesApi* | [**job_template_locale_show**](docs/JobTemplateLocalesApi.md#job_template_locale_show) | **GET** /projects/{project_id}/job_templates/{job_template_id}/locales/{job_template_locale_id} | Get a single job template locale
 *JobTemplateLocalesApi* | [**job_template_locale_update**](docs/JobTemplateLocalesApi.md#job_template_locale_update) | **PATCH** /projects/{project_id}/job_templates/{job_template_id}/locales/{job_template_locale_id} | Update a job template locale
 *JobTemplateLocalesApi* | [**job_template_locales_create**](docs/JobTemplateLocalesApi.md#job_template_locales_create) | **POST** /projects/{project_id}/job_templates/{job_template_id}/locales | Create a job template locale
 *JobTemplateLocalesApi* | [**job_template_locales_list**](docs/JobTemplateLocalesApi.md#job_template_locales_list) | **GET** /projects/{project_id}/job_templates/{job_template_id}/locales | List job template locales
 *JobTemplatesApi* | [**job_template_create**](docs/JobTemplatesApi.md#job_template_create) | **POST** /projects/{project_id}/job_templates | Create a job template
 *JobTemplatesApi* | [**job_template_delete**](docs/JobTemplatesApi.md#job_template_delete) | **DELETE** /projects/{project_id}/job_templates/{id} | Delete a job template
@@ -316,33 +316,33 @@
 *ScreenshotsApi* | [**screenshots_list**](docs/ScreenshotsApi.md#screenshots_list) | **GET** /projects/{project_id}/screenshots | List screenshots
 *SearchApi* | [**search_in_account**](docs/SearchApi.md#search_in_account) | **POST** /accounts/{account_id}/search | Search across projects
 *SpacesApi* | [**space_create**](docs/SpacesApi.md#space_create) | **POST** /accounts/{account_id}/spaces | Create a Space
 *SpacesApi* | [**space_delete**](docs/SpacesApi.md#space_delete) | **DELETE** /accounts/{account_id}/spaces/{id} | Delete Space
 *SpacesApi* | [**space_show**](docs/SpacesApi.md#space_show) | **GET** /accounts/{account_id}/spaces/{id} | Get Space
 *SpacesApi* | [**space_update**](docs/SpacesApi.md#space_update) | **PATCH** /accounts/{account_id}/spaces/{id} | Update Space
 *SpacesApi* | [**spaces_list**](docs/SpacesApi.md#spaces_list) | **GET** /accounts/{account_id}/spaces | List Spaces
-*SpacesApi* | [**spaces_projects_create**](docs/SpacesApi.md#spaces_projects_create) | **POST** /accounts/{account_id}/spaces/{space_id}/projects | Add Project
-*SpacesApi* | [**spaces_projects_delete**](docs/SpacesApi.md#spaces_projects_delete) | **DELETE** /accounts/{account_id}/spaces/{space_id}/projects/{id} | Remove Project
-*SpacesApi* | [**spaces_projects_list**](docs/SpacesApi.md#spaces_projects_list) | **GET** /accounts/{account_id}/spaces/{space_id}/projects | List Projects
+*SpacesApi* | [**spaces_projects_create**](docs/SpacesApi.md#spaces_projects_create) | **POST** /accounts/{account_id}/spaces/{space_id}/projects | Add Project to Space
+*SpacesApi* | [**spaces_projects_delete**](docs/SpacesApi.md#spaces_projects_delete) | **DELETE** /accounts/{account_id}/spaces/{space_id}/projects/{id} | Remove Project from Space
+*SpacesApi* | [**spaces_projects_list**](docs/SpacesApi.md#spaces_projects_list) | **GET** /accounts/{account_id}/spaces/{space_id}/projects | List Projects in Space
 *StyleGuidesApi* | [**styleguide_create**](docs/StyleGuidesApi.md#styleguide_create) | **POST** /projects/{project_id}/styleguides | Create a style guide
 *StyleGuidesApi* | [**styleguide_delete**](docs/StyleGuidesApi.md#styleguide_delete) | **DELETE** /projects/{project_id}/styleguides/{id} | Delete a style guide
 *StyleGuidesApi* | [**styleguide_show**](docs/StyleGuidesApi.md#styleguide_show) | **GET** /projects/{project_id}/styleguides/{id} | Get a single style guide
 *StyleGuidesApi* | [**styleguide_update**](docs/StyleGuidesApi.md#styleguide_update) | **PATCH** /projects/{project_id}/styleguides/{id} | Update a style guide
 *StyleGuidesApi* | [**styleguides_list**](docs/StyleGuidesApi.md#styleguides_list) | **GET** /projects/{project_id}/styleguides | List style guides
 *TagsApi* | [**tag_create**](docs/TagsApi.md#tag_create) | **POST** /projects/{project_id}/tags | Create a tag
 *TagsApi* | [**tag_delete**](docs/TagsApi.md#tag_delete) | **DELETE** /projects/{project_id}/tags/{name} | Delete a tag
 *TagsApi* | [**tag_show**](docs/TagsApi.md#tag_show) | **GET** /projects/{project_id}/tags/{name} | Get a single tag
 *TagsApi* | [**tags_list**](docs/TagsApi.md#tags_list) | **GET** /projects/{project_id}/tags | List tags
 *TeamsApi* | [**team_create**](docs/TeamsApi.md#team_create) | **POST** /accounts/{account_id}/teams | Create a Team
 *TeamsApi* | [**team_delete**](docs/TeamsApi.md#team_delete) | **DELETE** /accounts/{account_id}/teams/{id} | Delete Team
 *TeamsApi* | [**team_show**](docs/TeamsApi.md#team_show) | **GET** /accounts/{account_id}/teams/{id} | Get Team
 *TeamsApi* | [**team_update**](docs/TeamsApi.md#team_update) | **PATCH** /accounts/{account_id}/teams/{id} | Update Team
 *TeamsApi* | [**teams_list**](docs/TeamsApi.md#teams_list) | **GET** /accounts/{account_id}/teams | List Teams
-*TeamsApi* | [**teams_projects_create**](docs/TeamsApi.md#teams_projects_create) | **POST** /accounts/{account_id}/teams/{team_id}/projects | Add Project
-*TeamsApi* | [**teams_projects_delete**](docs/TeamsApi.md#teams_projects_delete) | **DELETE** /accounts/{account_id}/teams/{team_id}/projects/{id} | Remove Project
+*TeamsApi* | [**teams_projects_create**](docs/TeamsApi.md#teams_projects_create) | **POST** /accounts/{account_id}/teams/{team_id}/projects | Add Project to Team
+*TeamsApi* | [**teams_projects_delete**](docs/TeamsApi.md#teams_projects_delete) | **DELETE** /accounts/{account_id}/teams/{team_id}/projects/{id} | Remove Project from Team
 *TeamsApi* | [**teams_spaces_create**](docs/TeamsApi.md#teams_spaces_create) | **POST** /accounts/{account_id}/teams/{team_id}/spaces | Add Space
 *TeamsApi* | [**teams_spaces_delete**](docs/TeamsApi.md#teams_spaces_delete) | **DELETE** /accounts/{account_id}/teams/{team_id}/spaces/{id} | Remove Space
 *TeamsApi* | [**teams_users_create**](docs/TeamsApi.md#teams_users_create) | **POST** /accounts/{account_id}/teams/{team_id}/users | Add User
 *TeamsApi* | [**teams_users_delete**](docs/TeamsApi.md#teams_users_delete) | **DELETE** /accounts/{account_id}/teams/{team_id}/users/{id} | Remove User
 *TranslationsApi* | [**translation_create**](docs/TranslationsApi.md#translation_create) | **POST** /projects/{project_id}/translations | Create a translation
 *TranslationsApi* | [**translation_exclude**](docs/TranslationsApi.md#translation_exclude) | **PATCH** /projects/{project_id}/translations/{id}/exclude | Exclude a translation from export
 *TranslationsApi* | [**translation_include**](docs/TranslationsApi.md#translation_include) | **PATCH** /projects/{project_id}/translations/{id}/include | Include a translation
```

### Comparing `phrase-api-1.9.0/phrase_api/__init__.py` & `phrase-api-1.9.1/phrase_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: support@phrase.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 # import apis into sdk package
 from phrase_api.api.accounts_api import AccountsApi
 from phrase_api.api.authorizations_api import AuthorizationsApi
 from phrase_api.api.bitbucket_sync_api import BitbucketSyncApi
 from phrase_api.api.blacklisted_keys_api import BlacklistedKeysApi
 from phrase_api.api.branches_api import BranchesApi
```

### Comparing `phrase-api-1.9.0/phrase_api/api/__init__.py` & `phrase-api-1.9.1/phrase_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/accounts_api.py` & `phrase-api-1.9.1/phrase_api/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/authorizations_api.py` & `phrase-api-1.9.1/phrase_api/api/authorizations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/bitbucket_sync_api.py` & `phrase-api-1.9.1/phrase_api/api/bitbucket_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/blacklisted_keys_api.py` & `phrase-api-1.9.1/phrase_api/api/blacklisted_keys_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/branches_api.py` & `phrase-api-1.9.1/phrase_api/api/branches_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/comments_api.py` & `phrase-api-1.9.1/phrase_api/api/comments_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/distributions_api.py` & `phrase-api-1.9.1/phrase_api/api/distributions_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/documents_api.py` & `phrase-api-1.9.1/phrase_api/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/formats_api.py` & `phrase-api-1.9.1/phrase_api/api/formats_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/git_hub_sync_api.py` & `phrase-api-1.9.1/phrase_api/api/git_hub_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/git_lab_sync_api.py` & `phrase-api-1.9.1/phrase_api/api/git_lab_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/glossaries_api.py` & `phrase-api-1.9.1/phrase_api/api/glossaries_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/glossary_term_translations_api.py` & `phrase-api-1.9.1/phrase_api/api/glossary_term_translations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/glossary_terms_api.py` & `phrase-api-1.9.1/phrase_api/api/glossary_terms_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/icu_api.py` & `phrase-api-1.9.1/phrase_api/api/icu_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/invitations_api.py` & `phrase-api-1.9.1/phrase_api/api/invitations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/job_comments_api.py` & `phrase-api-1.9.1/phrase_api/api/job_comments_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/job_locales_api.py` & `phrase-api-1.9.1/phrase_api/api/job_locales_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -332,17 +332,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_locale_delete(self, project_id, job_id, id, **kwargs):  # noqa: E501
-        """Delete a job locale  # noqa: E501
+        """Remove a target locale from a job  # noqa: E501
 
-        Delete an existing job locale.  # noqa: E501
+        Removes a target locale from a job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_delete(project_id, job_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -361,17 +361,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.job_locale_delete_with_http_info(project_id, job_id, id, **kwargs)  # noqa: E501
 
     def job_locale_delete_with_http_info(self, project_id, job_id, id, **kwargs):  # noqa: E501
-        """Delete a job locale  # noqa: E501
+        """Remove a target locale from a job  # noqa: E501
 
-        Delete an existing job locale.  # noqa: E501
+        Removes a target locale from a job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_delete_with_http_info(project_id, job_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -620,17 +620,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_locale_show(self, project_id, job_id, id, **kwargs):  # noqa: E501
-        """Get a single job locale  # noqa: E501
+        """Show single job target locale  # noqa: E501
 
-        Get a single job locale for a given job.  # noqa: E501
+        Get a single target locale for a given job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_show(project_id, job_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -649,17 +649,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.job_locale_show_with_http_info(project_id, job_id, id, **kwargs)  # noqa: E501
 
     def job_locale_show_with_http_info(self, project_id, job_id, id, **kwargs):  # noqa: E501
-        """Get a single job locale  # noqa: E501
+        """Show single job target locale  # noqa: E501
 
-        Get a single job locale for a given job.  # noqa: E501
+        Get a single target locale for a given job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_show_with_http_info(project_id, job_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -762,17 +762,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_locale_update(self, project_id, job_id, id, job_locale_update_parameters, **kwargs):  # noqa: E501
-        """Update a job locale  # noqa: E501
+        """Update a job target locale  # noqa: E501
 
-        Update an existing job locale.  # noqa: E501
+        Update an existing job target locale.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_update(project_id, job_id, id, job_locale_update_parameters, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -791,17 +791,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.job_locale_update_with_http_info(project_id, job_id, id, job_locale_update_parameters, **kwargs)  # noqa: E501
 
     def job_locale_update_with_http_info(self, project_id, job_id, id, job_locale_update_parameters, **kwargs):  # noqa: E501
-        """Update a job locale  # noqa: E501
+        """Update a job target locale  # noqa: E501
 
-        Update an existing job locale.  # noqa: E501
+        Update an existing job target locale.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locale_update_with_http_info(project_id, job_id, id, job_locale_update_parameters, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -912,17 +912,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_locales_create(self, project_id, job_id, job_locales_create_parameters, **kwargs):  # noqa: E501
-        """Create a job locale  # noqa: E501
+        """Add a target locale to a job  # noqa: E501
 
-        Create a new job locale.  # noqa: E501
+        Adds a target locale to a job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locales_create(project_id, job_id, job_locales_create_parameters, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -940,17 +940,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.job_locales_create_with_http_info(project_id, job_id, job_locales_create_parameters, **kwargs)  # noqa: E501
 
     def job_locales_create_with_http_info(self, project_id, job_id, job_locales_create_parameters, **kwargs):  # noqa: E501
-        """Create a job locale  # noqa: E501
+        """Add a target locale to a job  # noqa: E501
 
-        Create a new job locale.  # noqa: E501
+        Adds a target locale to a job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locales_create_with_http_info(project_id, job_id, job_locales_create_parameters, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -1053,17 +1053,17 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_locales_list(self, project_id, job_id, **kwargs):  # noqa: E501
-        """List job locales  # noqa: E501
+        """List job target locales  # noqa: E501
 
-        List all job locales for a given job.  # noqa: E501
+        List all target locales for a given job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locales_list(project_id, job_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
@@ -1083,17 +1083,17 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.job_locales_list_with_http_info(project_id, job_id, **kwargs)  # noqa: E501
 
     def job_locales_list_with_http_info(self, project_id, job_id, **kwargs):  # noqa: E501
-        """List job locales  # noqa: E501
+        """List job target locales  # noqa: E501
 
-        List all job locales for a given job.  # noqa: E501
+        List all target locales for a given job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_locales_list_with_http_info(project_id, job_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_id: Project ID (required)
```

### Comparing `phrase-api-1.9.0/phrase_api/api/job_template_locales_api.py` & `phrase-api-1.9.1/phrase_api/api/job_template_locales_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/job_templates_api.py` & `phrase-api-1.9.1/phrase_api/api/job_templates_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/jobs_api.py` & `phrase-api-1.9.1/phrase_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/keys_api.py` & `phrase-api-1.9.1/phrase_api/api/keys_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/locales_api.py` & `phrase-api-1.9.1/phrase_api/api/locales_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         :param bool include_translated_keys: Include translated keys in the locale file. Use in combination with include_empty_translations to obtain only untranslated keys.
         :param bool keep_notranslate_tags: Indicates whether [NOTRANSLATE] tags should be kept.
         :param bool convert_emoji: This option is obsolete. Projects that were created on or after Nov 29th 2019 or that did not contain emoji by then will not require this flag any longer since emoji are now supported natively.
         :param object format_options: Additional formatting and render options. See the <a href=\"https://support.phrase.com/hc/en-us/sections/6111343326364\">format guide</a> for a list of options available for each format. Specify format options like this: <code>...&format_options[foo]=bar</code>
         :param str encoding: Enforces a specific encoding on the file contents. Valid options are \"UTF-8\", \"UTF-16\" and \"ISO-8859-1\".
         :param bool skip_unverified_translations: Indicates whether the locale file should skip all unverified translations. This parameter is deprecated and should be replaced with <code>include_unverified_translations</code>.
         :param bool include_unverified_translations: if set to false unverified translations are excluded
-        :param bool use_last_reviewed_version: If set to true the last reviewed version of a translation is used. This is only available if the review workflow (currently in beta) is enabled for the project.
+        :param bool use_last_reviewed_version: If set to true the last reviewed version of a translation is used. This is only available if the review workflow is enabled for the project.
         :param str fallback_locale_id: If a key has no translation in the locale being downloaded the translation in the fallback locale will be used. Provide the public ID of the locale that should be used as the fallback. Requires include_empty_translations to be set to <code>true</code>.
         :param str source_locale_id: Provides the source language of a corresponding job as the source language of the generated locale file. This parameter will be ignored unless used in combination with a <code>tag</code> parameter indicating a specific job.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -494,15 +494,15 @@
         :param bool include_translated_keys: Include translated keys in the locale file. Use in combination with include_empty_translations to obtain only untranslated keys.
         :param bool keep_notranslate_tags: Indicates whether [NOTRANSLATE] tags should be kept.
         :param bool convert_emoji: This option is obsolete. Projects that were created on or after Nov 29th 2019 or that did not contain emoji by then will not require this flag any longer since emoji are now supported natively.
         :param object format_options: Additional formatting and render options. See the <a href=\"https://support.phrase.com/hc/en-us/sections/6111343326364\">format guide</a> for a list of options available for each format. Specify format options like this: <code>...&format_options[foo]=bar</code>
         :param str encoding: Enforces a specific encoding on the file contents. Valid options are \"UTF-8\", \"UTF-16\" and \"ISO-8859-1\".
         :param bool skip_unverified_translations: Indicates whether the locale file should skip all unverified translations. This parameter is deprecated and should be replaced with <code>include_unverified_translations</code>.
         :param bool include_unverified_translations: if set to false unverified translations are excluded
-        :param bool use_last_reviewed_version: If set to true the last reviewed version of a translation is used. This is only available if the review workflow (currently in beta) is enabled for the project.
+        :param bool use_last_reviewed_version: If set to true the last reviewed version of a translation is used. This is only available if the review workflow is enabled for the project.
         :param str fallback_locale_id: If a key has no translation in the locale being downloaded the translation in the fallback locale will be used. Provide the public ID of the locale that should be used as the fallback. Requires include_empty_translations to be set to <code>true</code>.
         :param str source_locale_id: Provides the source language of a corresponding job as the source language of the generated locale file. This parameter will be ignored unless used in combination with a <code>tag</code> parameter indicating a specific job.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
```

### Comparing `phrase-api-1.9.0/phrase_api/api/members_api.py` & `phrase-api-1.9.1/phrase_api/api/members_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/notification_groups_api.py` & `phrase-api-1.9.1/phrase_api/api/notification_groups_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/notifications_api.py` & `phrase-api-1.9.1/phrase_api/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/orders_api.py` & `phrase-api-1.9.1/phrase_api/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/organization_job_template_locales_api.py` & `phrase-api-1.9.1/phrase_api/api/organization_job_template_locales_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/organization_job_templates_api.py` & `phrase-api-1.9.1/phrase_api/api/organization_job_templates_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/projects_api.py` & `phrase-api-1.9.1/phrase_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/releases_api.py` & `phrase-api-1.9.1/phrase_api/api/releases_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/screenshot_markers_api.py` & `phrase-api-1.9.1/phrase_api/api/screenshot_markers_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/screenshots_api.py` & `phrase-api-1.9.1/phrase_api/api/screenshots_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/search_api.py` & `phrase-api-1.9.1/phrase_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/spaces_api.py` & `phrase-api-1.9.1/phrase_api/api/spaces_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def spaces_projects_create(self, account_id, space_id, spaces_projects_create_parameters, **kwargs):  # noqa: E501
-        """Add Project  # noqa: E501
+        """Add Project to Space  # noqa: E501
 
         Adds an existing project to the space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_create(account_id, space_id, spaces_projects_create_parameters, async_req=True)
         >>> result = thread.get()
 
@@ -714,15 +714,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.spaces_projects_create_with_http_info(account_id, space_id, spaces_projects_create_parameters, **kwargs)  # noqa: E501
 
     def spaces_projects_create_with_http_info(self, account_id, space_id, spaces_projects_create_parameters, **kwargs):  # noqa: E501
-        """Add Project  # noqa: E501
+        """Add Project to Space  # noqa: E501
 
         Adds an existing project to the space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_create_with_http_info(account_id, space_id, spaces_projects_create_parameters, async_req=True)
         >>> result = thread.get()
 
@@ -823,15 +823,15 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def spaces_projects_delete(self, account_id, space_id, id, **kwargs):  # noqa: E501
-        """Remove Project  # noqa: E501
+        """Remove Project from Space  # noqa: E501
 
         Removes a specified project from the specified space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_delete(account_id, space_id, id, async_req=True)
         >>> result = thread.get()
 
@@ -851,15 +851,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.spaces_projects_delete_with_http_info(account_id, space_id, id, **kwargs)  # noqa: E501
 
     def spaces_projects_delete_with_http_info(self, account_id, space_id, id, **kwargs):  # noqa: E501
-        """Remove Project  # noqa: E501
+        """Remove Project from Space  # noqa: E501
 
         Removes a specified project from the specified space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_delete_with_http_info(account_id, space_id, id, async_req=True)
         >>> result = thread.get()
 
@@ -956,15 +956,15 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def spaces_projects_list(self, account_id, space_id, **kwargs):  # noqa: E501
-        """List Projects  # noqa: E501
+        """List Projects in Space  # noqa: E501
 
         List all projects for the specified Space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_list(account_id, space_id, async_req=True)
         >>> result = thread.get()
 
@@ -985,15 +985,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.spaces_projects_list_with_http_info(account_id, space_id, **kwargs)  # noqa: E501
 
     def spaces_projects_list_with_http_info(self, account_id, space_id, **kwargs):  # noqa: E501
-        """List Projects  # noqa: E501
+        """List Projects in Space  # noqa: E501
 
         List all projects for the specified Space.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.spaces_projects_list_with_http_info(account_id, space_id, async_req=True)
         >>> result = thread.get()
```

### Comparing `phrase-api-1.9.0/phrase_api/api/style_guides_api.py` & `phrase-api-1.9.1/phrase_api/api/style_guides_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/tags_api.py` & `phrase-api-1.9.1/phrase_api/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/teams_api.py` & `phrase-api-1.9.1/phrase_api/api/teams_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def teams_projects_create(self, account_id, team_id, teams_projects_create_parameters, **kwargs):  # noqa: E501
-        """Add Project  # noqa: E501
+        """Add Project to Team  # noqa: E501
 
         Adds an existing project to the team.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.teams_projects_create(account_id, team_id, teams_projects_create_parameters, async_req=True)
         >>> result = thread.get()
 
@@ -714,15 +714,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.teams_projects_create_with_http_info(account_id, team_id, teams_projects_create_parameters, **kwargs)  # noqa: E501
 
     def teams_projects_create_with_http_info(self, account_id, team_id, teams_projects_create_parameters, **kwargs):  # noqa: E501
-        """Add Project  # noqa: E501
+        """Add Project to Team  # noqa: E501
 
         Adds an existing project to the team.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.teams_projects_create_with_http_info(account_id, team_id, teams_projects_create_parameters, async_req=True)
         >>> result = thread.get()
 
@@ -823,15 +823,15 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def teams_projects_delete(self, account_id, team_id, id, **kwargs):  # noqa: E501
-        """Remove Project  # noqa: E501
+        """Remove Project from Team  # noqa: E501
 
         Removes a specified project from the specified team.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.teams_projects_delete(account_id, team_id, id, async_req=True)
         >>> result = thread.get()
 
@@ -851,15 +851,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.teams_projects_delete_with_http_info(account_id, team_id, id, **kwargs)  # noqa: E501
 
     def teams_projects_delete_with_http_info(self, account_id, team_id, id, **kwargs):  # noqa: E501
-        """Remove Project  # noqa: E501
+        """Remove Project from Team  # noqa: E501
 
         Removes a specified project from the specified team.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.teams_projects_delete_with_http_info(account_id, team_id, id, async_req=True)
         >>> result = thread.get()
```

### Comparing `phrase-api-1.9.0/phrase_api/api/translations_api.py` & `phrase-api-1.9.1/phrase_api/api/translations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/uploads_api.py` & `phrase-api-1.9.1/phrase_api/api/uploads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         :param bool convert_emoji: This option is obsolete. Providing the option will cause a bad request error.
         :param bool skip_upload_tags: Indicates whether the upload should not create upload tags.
         :param bool skip_unverification: Indicates whether the upload should unverify updated translations.
         :param str file_encoding: Enforces a specific encoding on the file contents. Valid options are \\\"UTF-8\\\", \\\"UTF-16\\\" and \\\"ISO-8859-1\\\".
         :param object locale_mapping: Optional, format specific mapping between locale names and the columns the translations to those locales are contained in.
         :param object format_options: Additional options available for specific formats. See our format guide for complete list.
         :param bool autotranslate: If set, translations for the uploaded language will be fetched automatically.
-        :param bool mark_reviewed: Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow (currently beta) is enabled for the project.
+        :param bool mark_reviewed: Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow is enabled for the project.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -98,15 +98,15 @@
         :param bool convert_emoji: This option is obsolete. Providing the option will cause a bad request error.
         :param bool skip_upload_tags: Indicates whether the upload should not create upload tags.
         :param bool skip_unverification: Indicates whether the upload should unverify updated translations.
         :param str file_encoding: Enforces a specific encoding on the file contents. Valid options are \\\"UTF-8\\\", \\\"UTF-16\\\" and \\\"ISO-8859-1\\\".
         :param object locale_mapping: Optional, format specific mapping between locale names and the columns the translations to those locales are contained in.
         :param object format_options: Additional options available for specific formats. See our format guide for complete list.
         :param bool autotranslate: If set, translations for the uploaded language will be fetched automatically.
-        :param bool mark_reviewed: Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow (currently beta) is enabled for the project.
+        :param bool mark_reviewed: Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow is enabled for the project.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `phrase-api-1.9.0/phrase_api/api/users_api.py` & `phrase-api-1.9.1/phrase_api/api/users_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/variables_api.py` & `phrase-api-1.9.1/phrase_api/api/variables_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/versions___history_api.py` & `phrase-api-1.9.1/phrase_api/api/versions___history_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/webhook_deliveries_api.py` & `phrase-api-1.9.1/phrase_api/api/webhook_deliveries_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api/webhooks_api.py` & `phrase-api-1.9.1/phrase_api/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/api_client.py` & `phrase-api-1.9.1/phrase_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.9.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.9.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `phrase-api-1.9.0/phrase_api/configuration.py` & `phrase-api-1.9.1/phrase_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 1.9.0".\
+               "SDK Package Version: 1.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `phrase-api-1.9.0/phrase_api/exceptions.py` & `phrase-api-1.9.1/phrase_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/__init__.py` & `phrase-api-1.9.1/phrase_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/account.py` & `phrase-api-1.9.1/phrase_api/models/account.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/account_details.py` & `phrase-api-1.9.1/phrase_api/models/account_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/account_details1.py` & `phrase-api-1.9.1/phrase_api/models/account_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/account_search_result.py` & `phrase-api-1.9.1/phrase_api/models/account_search_result.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/affected_count.py` & `phrase-api-1.9.1/phrase_api/models/affected_count.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/affected_resources.py` & `phrase-api-1.9.1/phrase_api/models/affected_resources.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/authorization.py` & `phrase-api-1.9.1/phrase_api/models/authorization.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/authorization_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/authorization_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/authorization_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/authorization_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/authorization_with_token.py` & `phrase-api-1.9.1/phrase_api/models/authorization_with_token.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/authorization_with_token1.py` & `phrase-api-1.9.1/phrase_api/models/authorization_with_token1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/bitbucket_sync.py` & `phrase-api-1.9.1/phrase_api/models/bitbucket_sync.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/bitbucket_sync_export_parameters.py` & `phrase-api-1.9.1/phrase_api/models/bitbucket_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/bitbucket_sync_export_response.py` & `phrase-api-1.9.1/phrase_api/models/bitbucket_sync_export_response.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/bitbucket_sync_import_parameters.py` & `phrase-api-1.9.1/phrase_api/models/bitbucket_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/blacklisted_key.py` & `phrase-api-1.9.1/phrase_api/models/blacklisted_key.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/blacklisted_key_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/blacklisted_key_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/blacklisted_key_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/blacklisted_key_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/branch.py` & `phrase-api-1.9.1/phrase_api/models/branch.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/branch_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/branch_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/branch_merge_parameters.py` & `phrase-api-1.9.1/phrase_api/models/branch_merge_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/branch_name.py` & `phrase-api-1.9.1/phrase_api/models/branch_name.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/branch_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/branch_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/comment.py` & `phrase-api-1.9.1/phrase_api/models/comment.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/comment_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/comment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/comment_mark_read_parameters.py` & `phrase-api-1.9.1/phrase_api/models/comment_mark_read_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/comment_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/comment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/current_user.py` & `phrase-api-1.9.1/phrase_api/models/current_user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/distribution.py` & `phrase-api-1.9.1/phrase_api/models/distribution.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/distribution_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/distribution_create_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,26 +137,26 @@
 
         self._project_id = project_id
 
     @property
     def platforms(self):
         """Gets the platforms of this DistributionCreateParameters.  # noqa: E501
 
-        List of platforms the distribution should support.  # noqa: E501
+        List of platforms the distribution should support. Valid values are: * `android` * `ios` * `flutter` * `i18next`  # noqa: E501
 
         :return: The platforms of this DistributionCreateParameters.  # noqa: E501
         :rtype: list[str]
         """
         return self._platforms
 
     @platforms.setter
     def platforms(self, platforms):
         """Sets the platforms of this DistributionCreateParameters.
 
-        List of platforms the distribution should support.  # noqa: E501
+        List of platforms the distribution should support. Valid values are: * `android` * `ios` * `flutter` * `i18next`  # noqa: E501
 
         :param platforms: The platforms of this DistributionCreateParameters.  # noqa: E501
         :type: list[str]
         """
 
         self._platforms = platforms
```

### Comparing `phrase-api-1.9.0/phrase_api/models/distribution_preview.py` & `phrase-api-1.9.1/phrase_api/models/distribution_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/distribution_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/distribution_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/document.py` & `phrase-api-1.9.1/phrase_api/models/document.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/format.py` & `phrase-api-1.9.1/phrase_api/models/format.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/github_sync_export_parameters.py` & `phrase-api-1.9.1/phrase_api/models/github_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/github_sync_import_parameters.py` & `phrase-api-1.9.1/phrase_api/models/github_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/gitlab_sync.py` & `phrase-api-1.9.1/phrase_api/models/gitlab_sync.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/gitlab_sync_export.py` & `phrase-api-1.9.1/phrase_api/models/gitlab_sync_export.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/gitlab_sync_export_parameters.py` & `phrase-api-1.9.1/phrase_api/models/gitlab_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/gitlab_sync_history.py` & `phrase-api-1.9.1/phrase_api/models/gitlab_sync_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'status': 'int',
+        'status': 'str',
         'action': 'str',
         'errors': 'list[str]',
         'date': 'datetime',
         'details': 'object'
     }
 
     attribute_map = {
@@ -73,25 +73,25 @@
 
     @property
     def status(self):
         """Gets the status of this GitlabSyncHistory.  # noqa: E501
 
 
         :return: The status of this GitlabSyncHistory.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this GitlabSyncHistory.
 
 
         :param status: The status of this GitlabSyncHistory.  # noqa: E501
-        :type: int
+        :type: str
         """
 
         self._status = status
 
     @property
     def action(self):
         """Gets the action of this GitlabSyncHistory.  # noqa: E501
```

### Comparing `phrase-api-1.9.0/phrase_api/models/gitlab_sync_import_parameters.py` & `phrase-api-1.9.1/phrase_api/models/gitlab_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary.py` & `phrase-api-1.9.1/phrase_api/models/glossary.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term_translation.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term_translation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term_translation_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term_translation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term_translation_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term_translation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_term_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_term_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/glossary_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/glossary_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/icu.py` & `phrase-api-1.9.1/phrase_api/models/icu.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/icu_skeleton_parameters.py` & `phrase-api-1.9.1/phrase_api/models/icu_skeleton_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/inline_response422.py` & `phrase-api-1.9.1/phrase_api/models/inline_response422.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/inline_response422_errors.py` & `phrase-api-1.9.1/phrase_api/models/inline_response422_errors.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/invitation.py` & `phrase-api-1.9.1/phrase_api/models/invitation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/invitation_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/invitation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/invitation_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/invitation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/invitation_update_settings_parameters.py` & `phrase-api-1.9.1/phrase_api/models/invitation_update_settings_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job.py` & `phrase-api-1.9.1/phrase_api/models/job.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_comment.py` & `phrase-api-1.9.1/phrase_api/models/job_comment.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_comment_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_comment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_comment_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_comment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_complete_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_complete_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_details.py` & `phrase-api-1.9.1/phrase_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_details1.py` & `phrase-api-1.9.1/phrase_api/models/job_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_keys_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_keys_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locale.py` & `phrase-api-1.9.1/phrase_api/models/job_locale.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locale_complete_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_locale_complete_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locale_complete_review_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_locale_complete_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locale_reopen_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_locale_reopen_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locale_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_locale_update_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,26 +99,26 @@
 
         self._branch = branch
 
     @property
     def locale_id(self):
         """Gets the locale_id of this JobLocaleUpdateParameters.  # noqa: E501
 
-        locale id  # noqa: E501
+        ID of a target locale to update  # noqa: E501
 
         :return: The locale_id of this JobLocaleUpdateParameters.  # noqa: E501
         :rtype: str
         """
         return self._locale_id
 
     @locale_id.setter
     def locale_id(self, locale_id):
         """Sets the locale_id of this JobLocaleUpdateParameters.
 
-        locale id  # noqa: E501
+        ID of a target locale to update  # noqa: E501
 
         :param locale_id: The locale_id of this JobLocaleUpdateParameters.  # noqa: E501
         :type: str
         """
 
         self._locale_id = locale_id
```

### Comparing `phrase-api-1.9.0/phrase_api/models/job_locales_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_locales_create_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,26 +98,26 @@
 
         self._branch = branch
 
     @property
     def locale_id(self):
         """Gets the locale_id of this JobLocalesCreateParameters.  # noqa: E501
 
-        locale id  # noqa: E501
+        ID of a locale to be added  # noqa: E501
 
         :return: The locale_id of this JobLocalesCreateParameters.  # noqa: E501
         :rtype: str
         """
         return self._locale_id
 
     @locale_id.setter
     def locale_id(self, locale_id):
         """Sets the locale_id of this JobLocalesCreateParameters.
 
-        locale id  # noqa: E501
+        ID of a locale to be added  # noqa: E501
 
         :param locale_id: The locale_id of this JobLocalesCreateParameters.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and locale_id is None:  # noqa: E501
             raise ValueError("Invalid value for `locale_id`, must not be `None`")  # noqa: E501
```

### Comparing `phrase-api-1.9.0/phrase_api/models/job_preview.py` & `phrase-api-1.9.1/phrase_api/models/job_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_reopen_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_reopen_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_start_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_start_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template.py` & `phrase-api-1.9.1/phrase_api/models/job_template.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_details.py` & `phrase-api-1.9.1/phrase_api/models/job_template_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_details1.py` & `phrase-api-1.9.1/phrase_api/models/job_template_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_locale_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_template_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_locales.py` & `phrase-api-1.9.1/phrase_api/models/job_template_locales.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_locales_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_template_locales_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_preview.py` & `phrase-api-1.9.1/phrase_api/models/job_template_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_template_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_template_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/job_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/job_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/key_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/key_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/key_preview.py` & `phrase-api-1.9.1/phrase_api/models/key_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/key_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/key_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/keys_exclude_parameters.py` & `phrase-api-1.9.1/phrase_api/models/keys_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/keys_include_parameters.py` & `phrase-api-1.9.1/phrase_api/models/keys_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/keys_search_parameters.py` & `phrase-api-1.9.1/phrase_api/models/keys_search_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/keys_tag_parameters.py` & `phrase-api-1.9.1/phrase_api/models/keys_tag_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/keys_untag_parameters.py` & `phrase-api-1.9.1/phrase_api/models/keys_untag_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale.py` & `phrase-api-1.9.1/phrase_api/models/locale.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/locale_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_details.py` & `phrase-api-1.9.1/phrase_api/models/locale_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_details1.py` & `phrase-api-1.9.1/phrase_api/models/locale_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_preview.py` & `phrase-api-1.9.1/phrase_api/models/locale_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_preview1.py` & `phrase-api-1.9.1/phrase_api/models/locale_preview1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_statistics.py` & `phrase-api-1.9.1/phrase_api/models/locale_statistics.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_team_preview.py` & `phrase-api-1.9.1/phrase_api/models/locale_team_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/locale_user_preview.py` & `phrase-api-1.9.1/phrase_api/models/locale_user_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member.py` & `phrase-api-1.9.1/phrase_api/models/member.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member_project_detail.py` & `phrase-api-1.9.1/phrase_api/models/member_project_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member_project_detail_project_roles.py` & `phrase-api-1.9.1/phrase_api/models/member_project_detail_project_roles.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member_spaces.py` & `phrase-api-1.9.1/phrase_api/models/member_spaces.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/member_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/member_update_settings_parameters.py` & `phrase-api-1.9.1/phrase_api/models/member_update_settings_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/notification.py` & `phrase-api-1.9.1/phrase_api/models/notification.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/notification_group.py` & `phrase-api-1.9.1/phrase_api/models/notification_group.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/notification_group_detail.py` & `phrase-api-1.9.1/phrase_api/models/notification_group_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/order_confirm_parameters.py` & `phrase-api-1.9.1/phrase_api/models/order_confirm_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/order_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/order_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template_details.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template_locale_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template_locales_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template_locales_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/organization_job_template_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/organization_job_template_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project.py` & `phrase-api-1.9.1/phrase_api/models/project.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/project_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_details.py` & `phrase-api-1.9.1/phrase_api/models/project_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_details1.py` & `phrase-api-1.9.1/phrase_api/models/project_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_locales.py` & `phrase-api-1.9.1/phrase_api/models/project_locales.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_locales1.py` & `phrase-api-1.9.1/phrase_api/models/project_locales1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_member_specific.py` & `phrase-api-1.9.1/phrase_api/models/project_member_specific.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_short.py` & `phrase-api-1.9.1/phrase_api/models/project_short.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/project_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/project_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/release.py` & `phrase-api-1.9.1/phrase_api/models/release.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/release_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/release_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/release_preview.py` & `phrase-api-1.9.1/phrase_api/models/release_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/release_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/release_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot.py` & `phrase-api-1.9.1/phrase_api/models/screenshot.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/screenshot_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot_marker.py` & `phrase-api-1.9.1/phrase_api/models/screenshot_marker.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot_marker_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/screenshot_marker_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot_marker_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/screenshot_marker_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/screenshot_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/screenshot_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/search_in_account_parameters.py` & `phrase-api-1.9.1/phrase_api/models/search_in_account_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/space.py` & `phrase-api-1.9.1/phrase_api/models/space.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/space1.py` & `phrase-api-1.9.1/phrase_api/models/space1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/space_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/space_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/space_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/space_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/spaces_projects_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/spaces_projects_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide.py` & `phrase-api-1.9.1/phrase_api/models/styleguide.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/styleguide_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide_details.py` & `phrase-api-1.9.1/phrase_api/models/styleguide_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide_details1.py` & `phrase-api-1.9.1/phrase_api/models/styleguide_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide_preview.py` & `phrase-api-1.9.1/phrase_api/models/styleguide_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/styleguide_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/styleguide_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/subscription.py` & `phrase-api-1.9.1/phrase_api/models/subscription.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag.py` & `phrase-api-1.9.1/phrase_api/models/tag.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/tag_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag_with_stats.py` & `phrase-api-1.9.1/phrase_api/models/tag_with_stats.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag_with_stats1.py` & `phrase-api-1.9.1/phrase_api/models/tag_with_stats1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag_with_stats1_statistics.py` & `phrase-api-1.9.1/phrase_api/models/tag_with_stats1_statistics.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/tag_with_stats1_statistics1.py` & `phrase-api-1.9.1/phrase_api/models/tag_with_stats1_statistics1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/team.py` & `phrase-api-1.9.1/phrase_api/models/team.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/team_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/team_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/team_detail.py` & `phrase-api-1.9.1/phrase_api/models/team_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/team_short.py` & `phrase-api-1.9.1/phrase_api/models/team_short.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/team_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/team_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/teams_projects_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/teams_projects_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/teams_spaces_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/teams_spaces_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/teams_users_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/teams_users_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation.py` & `phrase-api-1.9.1/phrase_api/models/translation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_details.py` & `phrase-api-1.9.1/phrase_api/models/translation_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_details1.py` & `phrase-api-1.9.1/phrase_api/models/translation_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_exclude_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_include_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_key.py` & `phrase-api-1.9.1/phrase_api/models/translation_key.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_key_details.py` & `phrase-api-1.9.1/phrase_api/models/translation_key_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_key_details1.py` & `phrase-api-1.9.1/phrase_api/models/translation_key_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_order.py` & `phrase-api-1.9.1/phrase_api/models/translation_order.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_review_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_unverify_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_unverify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_verify_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translation_verify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_version.py` & `phrase-api-1.9.1/phrase_api/models/translation_version.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_version_with_user.py` & `phrase-api-1.9.1/phrase_api/models/translation_version_with_user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translation_version_with_user1.py` & `phrase-api-1.9.1/phrase_api/models/translation_version_with_user1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_exclude_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_include_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_review_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_search_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_search_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_unverify_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_unverify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/translations_verify_parameters.py` & `phrase-api-1.9.1/phrase_api/models/translations_verify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/upload.py` & `phrase-api-1.9.1/phrase_api/models/upload.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/upload_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/upload_create_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,26 +443,26 @@
 
         self._autotranslate = autotranslate
 
     @property
     def mark_reviewed(self):
         """Gets the mark_reviewed of this UploadCreateParameters.  # noqa: E501
 
-        Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow (currently beta) is enabled for the project.  # noqa: E501
+        Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow is enabled for the project.  # noqa: E501
 
         :return: The mark_reviewed of this UploadCreateParameters.  # noqa: E501
         :rtype: bool
         """
         return self._mark_reviewed
 
     @mark_reviewed.setter
     def mark_reviewed(self, mark_reviewed):
         """Sets the mark_reviewed of this UploadCreateParameters.
 
-        Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow (currently beta) is enabled for the project.  # noqa: E501
+        Indicated whether the imported translations should be marked as reviewed. This setting is available if the review workflow is enabled for the project.  # noqa: E501
 
         :param mark_reviewed: The mark_reviewed of this UploadCreateParameters.  # noqa: E501
         :type: bool
         """
 
         self._mark_reviewed = mark_reviewed
```

### Comparing `phrase-api-1.9.0/phrase_api/models/upload_summary.py` & `phrase-api-1.9.1/phrase_api/models/upload_summary.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/user.py` & `phrase-api-1.9.1/phrase_api/models/user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/user_preview.py` & `phrase-api-1.9.1/phrase_api/models/user_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/variable.py` & `phrase-api-1.9.1/phrase_api/models/variable.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/variable_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/variable_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/variable_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/variable_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/webhook.py` & `phrase-api-1.9.1/phrase_api/models/webhook.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/webhook_create_parameters.py` & `phrase-api-1.9.1/phrase_api/models/webhook_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/webhook_delivery.py` & `phrase-api-1.9.1/phrase_api/models/webhook_delivery.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/models/webhook_update_parameters.py` & `phrase-api-1.9.1/phrase_api/models/webhook_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api/rest.py` & `phrase-api-1.9.1/phrase_api/rest.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/phrase_api.egg-info/PKG-INFO` & `phrase-api-1.9.1/phrase_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phrase-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: Phrase Strings API Reference
 Home-page: https://github.com/phrase/phrase-python
 Author: Phrase Support
 Author-email: support@phrase.com
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Phrase Strings API Reference
```

### Comparing `phrase-api-1.9.0/phrase_api.egg-info/SOURCES.txt` & `phrase-api-1.9.1/phrase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/setup.py` & `phrase-api-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "phrase-api"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `phrase-api-1.9.0/test/test_account.py` & `phrase-api-1.9.1/test/test_account.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_account_details.py` & `phrase-api-1.9.1/test/test_account_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_account_details1.py` & `phrase-api-1.9.1/test/test_account_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_account_search_result.py` & `phrase-api-1.9.1/test/test_account_search_result.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_accounts_api.py` & `phrase-api-1.9.1/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_affected_count.py` & `phrase-api-1.9.1/test/test_affected_count.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_affected_resources.py` & `phrase-api-1.9.1/test/test_affected_resources.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorization.py` & `phrase-api-1.9.1/test/test_authorization.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorization_create_parameters.py` & `phrase-api-1.9.1/test/test_authorization_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorization_update_parameters.py` & `phrase-api-1.9.1/test/test_authorization_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorization_with_token.py` & `phrase-api-1.9.1/test/test_authorization_with_token.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorization_with_token1.py` & `phrase-api-1.9.1/test/test_authorization_with_token1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_authorizations_api.py` & `phrase-api-1.9.1/test/test_authorizations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_bitbucket_sync.py` & `phrase-api-1.9.1/test/test_bitbucket_sync.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_bitbucket_sync_api.py` & `phrase-api-1.9.1/test/test_bitbucket_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_bitbucket_sync_export_parameters.py` & `phrase-api-1.9.1/test/test_bitbucket_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_bitbucket_sync_export_response.py` & `phrase-api-1.9.1/test/test_bitbucket_sync_export_response.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_bitbucket_sync_import_parameters.py` & `phrase-api-1.9.1/test/test_bitbucket_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_blacklisted_key.py` & `phrase-api-1.9.1/test/test_blacklisted_key.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_blacklisted_key_create_parameters.py` & `phrase-api-1.9.1/test/test_blacklisted_key_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_blacklisted_key_update_parameters.py` & `phrase-api-1.9.1/test/test_blacklisted_key_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_blacklisted_keys_api.py` & `phrase-api-1.9.1/test/test_blacklisted_keys_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branch.py` & `phrase-api-1.9.1/test/test_branch.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branch_create_parameters.py` & `phrase-api-1.9.1/test/test_branch_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branch_merge_parameters.py` & `phrase-api-1.9.1/test/test_branch_merge_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branch_name.py` & `phrase-api-1.9.1/test/test_branch_name.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branch_update_parameters.py` & `phrase-api-1.9.1/test/test_branch_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_branches_api.py` & `phrase-api-1.9.1/test/test_branches_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_comment.py` & `phrase-api-1.9.1/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_comment_create_parameters.py` & `phrase-api-1.9.1/test/test_comment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_comment_mark_read_parameters.py` & `phrase-api-1.9.1/test/test_comment_mark_read_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_comment_update_parameters.py` & `phrase-api-1.9.1/test/test_comment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_comments_api.py` & `phrase-api-1.9.1/test/test_comments_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_current_user.py` & `phrase-api-1.9.1/test/test_current_user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_distribution.py` & `phrase-api-1.9.1/test/test_distribution.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_distribution_create_parameters.py` & `phrase-api-1.9.1/test/test_distribution_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_distribution_preview.py` & `phrase-api-1.9.1/test/test_distribution_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_distribution_update_parameters.py` & `phrase-api-1.9.1/test/test_distribution_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_distributions_api.py` & `phrase-api-1.9.1/test/test_distributions_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_document.py` & `phrase-api-1.9.1/test/test_document.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_documents_api.py` & `phrase-api-1.9.1/test/test_documents_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_format.py` & `phrase-api-1.9.1/test/test_format.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_formats_api.py` & `phrase-api-1.9.1/test/test_formats_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_git_hub_sync_api.py` & `phrase-api-1.9.1/test/test_git_hub_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_git_lab_sync_api.py` & `phrase-api-1.9.1/test/test_git_lab_sync_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_github_sync_export_parameters.py` & `phrase-api-1.9.1/test/test_github_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_github_sync_import_parameters.py` & `phrase-api-1.9.1/test/test_github_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_gitlab_sync.py` & `phrase-api-1.9.1/test/test_gitlab_sync.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_gitlab_sync_export.py` & `phrase-api-1.9.1/test/test_gitlab_sync_export.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_gitlab_sync_export_parameters.py` & `phrase-api-1.9.1/test/test_gitlab_sync_export_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_gitlab_sync_history.py` & `phrase-api-1.9.1/test/test_gitlab_sync_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Test GitlabSyncHistory
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = phrase_api.models.gitlab_sync_history.GitlabSyncHistory()  # noqa: E501
         if include_optional :
             return GitlabSyncHistory(
-                status = 56, 
+                status = '0', 
                 action = '0', 
                 errors = [
                     '0'
                     ], 
                 date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 details = None
             )
```

### Comparing `phrase-api-1.9.0/test/test_gitlab_sync_import_parameters.py` & `phrase-api-1.9.1/test/test_gitlab_sync_import_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossaries_api.py` & `phrase-api-1.9.1/test/test_glossaries_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary.py` & `phrase-api-1.9.1/test/test_glossary.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_create_parameters.py` & `phrase-api-1.9.1/test/test_glossary_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term.py` & `phrase-api-1.9.1/test/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_create_parameters.py` & `phrase-api-1.9.1/test/test_glossary_term_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_translation.py` & `phrase-api-1.9.1/test/test_glossary_term_translation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_translation_create_parameters.py` & `phrase-api-1.9.1/test/test_glossary_term_translation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_translation_update_parameters.py` & `phrase-api-1.9.1/test/test_glossary_term_translation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_translations_api.py` & `phrase-api-1.9.1/test/test_glossary_term_translations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_term_update_parameters.py` & `phrase-api-1.9.1/test/test_glossary_term_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_terms_api.py` & `phrase-api-1.9.1/test/test_glossary_terms_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_glossary_update_parameters.py` & `phrase-api-1.9.1/test/test_glossary_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_icu.py` & `phrase-api-1.9.1/test/test_icu.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_icu_api.py` & `phrase-api-1.9.1/test/test_icu_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_icu_skeleton_parameters.py` & `phrase-api-1.9.1/test/test_icu_skeleton_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_inline_response422.py` & `phrase-api-1.9.1/test/test_inline_response422.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_inline_response422_errors.py` & `phrase-api-1.9.1/test/test_inline_response422_errors.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_invitation.py` & `phrase-api-1.9.1/test/test_invitation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_invitation_create_parameters.py` & `phrase-api-1.9.1/test/test_invitation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_invitation_update_parameters.py` & `phrase-api-1.9.1/test/test_invitation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_invitation_update_settings_parameters.py` & `phrase-api-1.9.1/test/test_invitation_update_settings_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_invitations_api.py` & `phrase-api-1.9.1/test/test_invitations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job.py` & `phrase-api-1.9.1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_comment.py` & `phrase-api-1.9.1/test/test_job_comment.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_comment_create_parameters.py` & `phrase-api-1.9.1/test/test_job_comment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_comment_update_parameters.py` & `phrase-api-1.9.1/test/test_job_comment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_comments_api.py` & `phrase-api-1.9.1/test/test_job_comments_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_complete_parameters.py` & `phrase-api-1.9.1/test/test_job_complete_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_create_parameters.py` & `phrase-api-1.9.1/test/test_job_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_details.py` & `phrase-api-1.9.1/test/test_job_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_details1.py` & `phrase-api-1.9.1/test/test_job_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_keys_create_parameters.py` & `phrase-api-1.9.1/test/test_job_keys_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locale.py` & `phrase-api-1.9.1/test/test_job_locale.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locale_complete_parameters.py` & `phrase-api-1.9.1/test/test_job_locale_complete_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locale_complete_review_parameters.py` & `phrase-api-1.9.1/test/test_job_locale_complete_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locale_reopen_parameters.py` & `phrase-api-1.9.1/test/test_job_locale_reopen_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locale_update_parameters.py` & `phrase-api-1.9.1/test/test_job_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_locales_api.py` & `phrase-api-1.9.1/test/test_job_locales_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,49 +40,49 @@
         Review a job locale  # noqa: E501
         """
         pass
 
     def test_job_locale_delete(self):
         """Test case for job_locale_delete
 
-        Delete a job locale  # noqa: E501
+        Remove a target locale from a job  # noqa: E501
         """
         pass
 
     def test_job_locale_reopen(self):
         """Test case for job_locale_reopen
 
         Reopen a job locale  # noqa: E501
         """
         pass
 
     def test_job_locale_show(self):
         """Test case for job_locale_show
 
-        Get a single job locale  # noqa: E501
+        Show single job target locale  # noqa: E501
         """
         pass
 
     def test_job_locale_update(self):
         """Test case for job_locale_update
 
-        Update a job locale  # noqa: E501
+        Update a job target locale  # noqa: E501
         """
         pass
 
     def test_job_locales_create(self):
         """Test case for job_locales_create
 
-        Create a job locale  # noqa: E501
+        Add a target locale to a job  # noqa: E501
         """
         pass
 
     def test_job_locales_list(self):
         """Test case for job_locales_list
 
-        List job locales  # noqa: E501
+        List job target locales  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `phrase-api-1.9.0/test/test_job_locales_create_parameters.py` & `phrase-api-1.9.1/test/test_job_locales_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_preview.py` & `phrase-api-1.9.1/test/test_job_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_reopen_parameters.py` & `phrase-api-1.9.1/test/test_job_reopen_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_start_parameters.py` & `phrase-api-1.9.1/test/test_job_start_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template.py` & `phrase-api-1.9.1/test/test_job_template.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_create_parameters.py` & `phrase-api-1.9.1/test/test_job_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_details.py` & `phrase-api-1.9.1/test/test_job_template_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_details1.py` & `phrase-api-1.9.1/test/test_job_template_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_locale_update_parameters.py` & `phrase-api-1.9.1/test/test_job_template_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_locales.py` & `phrase-api-1.9.1/test/test_job_template_locales.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_locales_api.py` & `phrase-api-1.9.1/test/test_job_template_locales_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_locales_create_parameters.py` & `phrase-api-1.9.1/test/test_job_template_locales_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_preview.py` & `phrase-api-1.9.1/test/test_job_template_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_template_update_parameters.py` & `phrase-api-1.9.1/test/test_job_template_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_templates_api.py` & `phrase-api-1.9.1/test/test_job_templates_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_job_update_parameters.py` & `phrase-api-1.9.1/test/test_job_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_jobs_api.py` & `phrase-api-1.9.1/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_key_create_parameters.py` & `phrase-api-1.9.1/test/test_key_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_key_preview.py` & `phrase-api-1.9.1/test/test_key_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_key_update_parameters.py` & `phrase-api-1.9.1/test/test_key_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_api.py` & `phrase-api-1.9.1/test/test_keys_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_exclude_parameters.py` & `phrase-api-1.9.1/test/test_keys_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_include_parameters.py` & `phrase-api-1.9.1/test/test_keys_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_search_parameters.py` & `phrase-api-1.9.1/test/test_keys_search_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_tag_parameters.py` & `phrase-api-1.9.1/test/test_keys_tag_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_keys_untag_parameters.py` & `phrase-api-1.9.1/test/test_keys_untag_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale.py` & `phrase-api-1.9.1/test/test_locale.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_create_parameters.py` & `phrase-api-1.9.1/test/test_locale_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_details.py` & `phrase-api-1.9.1/test/test_locale_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_details1.py` & `phrase-api-1.9.1/test/test_locale_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_preview.py` & `phrase-api-1.9.1/test/test_locale_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_preview1.py` & `phrase-api-1.9.1/test/test_locale_preview1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_statistics.py` & `phrase-api-1.9.1/test/test_locale_statistics.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_team_preview.py` & `phrase-api-1.9.1/test/test_locale_team_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_update_parameters.py` & `phrase-api-1.9.1/test/test_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locale_user_preview.py` & `phrase-api-1.9.1/test/test_locale_user_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_locales_api.py` & `phrase-api-1.9.1/test/test_locales_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member.py` & `phrase-api-1.9.1/test/test_member.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member_project_detail.py` & `phrase-api-1.9.1/test/test_member_project_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member_project_detail_project_roles.py` & `phrase-api-1.9.1/test/test_member_project_detail_project_roles.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member_spaces.py` & `phrase-api-1.9.1/test/test_member_spaces.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member_update_parameters.py` & `phrase-api-1.9.1/test/test_member_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_member_update_settings_parameters.py` & `phrase-api-1.9.1/test/test_member_update_settings_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_members_api.py` & `phrase-api-1.9.1/test/test_members_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_notification.py` & `phrase-api-1.9.1/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_notification_group.py` & `phrase-api-1.9.1/test/test_notification_group.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_notification_group_detail.py` & `phrase-api-1.9.1/test/test_notification_group_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_notification_groups_api.py` & `phrase-api-1.9.1/test/test_notification_groups_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_notifications_api.py` & `phrase-api-1.9.1/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_order_confirm_parameters.py` & `phrase-api-1.9.1/test/test_order_confirm_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_order_create_parameters.py` & `phrase-api-1.9.1/test/test_order_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_orders_api.py` & `phrase-api-1.9.1/test/test_orders_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template.py` & `phrase-api-1.9.1/test/test_organization_job_template.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_create_parameters.py` & `phrase-api-1.9.1/test/test_organization_job_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_details.py` & `phrase-api-1.9.1/test/test_organization_job_template_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_locale_update_parameters.py` & `phrase-api-1.9.1/test/test_organization_job_template_locale_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_locales_api.py` & `phrase-api-1.9.1/test/test_organization_job_template_locales_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_locales_create_parameters.py` & `phrase-api-1.9.1/test/test_organization_job_template_locales_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_template_update_parameters.py` & `phrase-api-1.9.1/test/test_organization_job_template_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_organization_job_templates_api.py` & `phrase-api-1.9.1/test/test_organization_job_templates_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project.py` & `phrase-api-1.9.1/test/test_project.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_create_parameters.py` & `phrase-api-1.9.1/test/test_project_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_details.py` & `phrase-api-1.9.1/test/test_project_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_details1.py` & `phrase-api-1.9.1/test/test_project_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_locales.py` & `phrase-api-1.9.1/test/test_project_locales.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_locales1.py` & `phrase-api-1.9.1/test/test_project_locales1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_member_specific.py` & `phrase-api-1.9.1/test/test_project_member_specific.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_short.py` & `phrase-api-1.9.1/test/test_project_short.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_project_update_parameters.py` & `phrase-api-1.9.1/test/test_project_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_projects_api.py` & `phrase-api-1.9.1/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_release.py` & `phrase-api-1.9.1/test/test_release.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_release_create_parameters.py` & `phrase-api-1.9.1/test/test_release_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_release_preview.py` & `phrase-api-1.9.1/test/test_release_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_release_update_parameters.py` & `phrase-api-1.9.1/test/test_release_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_releases_api.py` & `phrase-api-1.9.1/test/test_releases_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot.py` & `phrase-api-1.9.1/test/test_screenshot.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_create_parameters.py` & `phrase-api-1.9.1/test/test_screenshot_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_marker.py` & `phrase-api-1.9.1/test/test_screenshot_marker.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_marker_create_parameters.py` & `phrase-api-1.9.1/test/test_screenshot_marker_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_marker_update_parameters.py` & `phrase-api-1.9.1/test/test_screenshot_marker_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_markers_api.py` & `phrase-api-1.9.1/test/test_screenshot_markers_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshot_update_parameters.py` & `phrase-api-1.9.1/test/test_screenshot_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_screenshots_api.py` & `phrase-api-1.9.1/test/test_screenshots_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_search_api.py` & `phrase-api-1.9.1/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_search_in_account_parameters.py` & `phrase-api-1.9.1/test/test_search_in_account_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_space.py` & `phrase-api-1.9.1/test/test_space.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_space1.py` & `phrase-api-1.9.1/test/test_space1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_space_create_parameters.py` & `phrase-api-1.9.1/test/test_space_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_space_update_parameters.py` & `phrase-api-1.9.1/test/test_space_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_spaces_api.py` & `phrase-api-1.9.1/test/test_spaces_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,28 +61,28 @@
         List Spaces  # noqa: E501
         """
         pass
 
     def test_spaces_projects_create(self):
         """Test case for spaces_projects_create
 
-        Add Project  # noqa: E501
+        Add Project to Space  # noqa: E501
         """
         pass
 
     def test_spaces_projects_delete(self):
         """Test case for spaces_projects_delete
 
-        Remove Project  # noqa: E501
+        Remove Project from Space  # noqa: E501
         """
         pass
 
     def test_spaces_projects_list(self):
         """Test case for spaces_projects_list
 
-        List Projects  # noqa: E501
+        List Projects in Space  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `phrase-api-1.9.0/test/test_spaces_projects_create_parameters.py` & `phrase-api-1.9.1/test/test_spaces_projects_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_style_guides_api.py` & `phrase-api-1.9.1/test/test_style_guides_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide.py` & `phrase-api-1.9.1/test/test_styleguide.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide_create_parameters.py` & `phrase-api-1.9.1/test/test_styleguide_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide_details.py` & `phrase-api-1.9.1/test/test_styleguide_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide_details1.py` & `phrase-api-1.9.1/test/test_styleguide_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide_preview.py` & `phrase-api-1.9.1/test/test_styleguide_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_styleguide_update_parameters.py` & `phrase-api-1.9.1/test/test_styleguide_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_subscription.py` & `phrase-api-1.9.1/test/test_subscription.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag.py` & `phrase-api-1.9.1/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag_create_parameters.py` & `phrase-api-1.9.1/test/test_tag_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag_with_stats.py` & `phrase-api-1.9.1/test/test_tag_with_stats.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag_with_stats1.py` & `phrase-api-1.9.1/test/test_tag_with_stats1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag_with_stats1_statistics.py` & `phrase-api-1.9.1/test/test_tag_with_stats1_statistics.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tag_with_stats1_statistics1.py` & `phrase-api-1.9.1/test/test_tag_with_stats1_statistics1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_tags_api.py` & `phrase-api-1.9.1/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_team.py` & `phrase-api-1.9.1/test/test_team.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_team_create_parameters.py` & `phrase-api-1.9.1/test/test_team_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_team_detail.py` & `phrase-api-1.9.1/test/test_team_detail.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_team_short.py` & `phrase-api-1.9.1/test/test_team_short.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_team_update_parameters.py` & `phrase-api-1.9.1/test/test_team_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_teams_api.py` & `phrase-api-1.9.1/test/test_teams_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,22 @@
         List Teams  # noqa: E501
         """
         pass
 
     def test_teams_projects_create(self):
         """Test case for teams_projects_create
 
-        Add Project  # noqa: E501
+        Add Project to Team  # noqa: E501
         """
         pass
 
     def test_teams_projects_delete(self):
         """Test case for teams_projects_delete
 
-        Remove Project  # noqa: E501
+        Remove Project from Team  # noqa: E501
         """
         pass
 
     def test_teams_spaces_create(self):
         """Test case for teams_spaces_create
 
         Add Space  # noqa: E501
```

### Comparing `phrase-api-1.9.0/test/test_teams_projects_create_parameters.py` & `phrase-api-1.9.1/test/test_teams_projects_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_teams_spaces_create_parameters.py` & `phrase-api-1.9.1/test/test_teams_spaces_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_teams_users_create_parameters.py` & `phrase-api-1.9.1/test/test_teams_users_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation.py` & `phrase-api-1.9.1/test/test_translation.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_create_parameters.py` & `phrase-api-1.9.1/test/test_translation_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_details.py` & `phrase-api-1.9.1/test/test_translation_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_details1.py` & `phrase-api-1.9.1/test/test_translation_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_exclude_parameters.py` & `phrase-api-1.9.1/test/test_translation_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_include_parameters.py` & `phrase-api-1.9.1/test/test_translation_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_key.py` & `phrase-api-1.9.1/test/test_translation_key.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_key_details.py` & `phrase-api-1.9.1/test/test_translation_key_details.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_key_details1.py` & `phrase-api-1.9.1/test/test_translation_key_details1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_order.py` & `phrase-api-1.9.1/test/test_translation_order.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_review_parameters.py` & `phrase-api-1.9.1/test/test_translation_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_unverify_parameters.py` & `phrase-api-1.9.1/test/test_translation_unverify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_update_parameters.py` & `phrase-api-1.9.1/test/test_translation_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_verify_parameters.py` & `phrase-api-1.9.1/test/test_translation_verify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_version.py` & `phrase-api-1.9.1/test/test_translation_version.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_version_with_user.py` & `phrase-api-1.9.1/test/test_translation_version_with_user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translation_version_with_user1.py` & `phrase-api-1.9.1/test/test_translation_version_with_user1.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_api.py` & `phrase-api-1.9.1/test/test_translations_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_exclude_parameters.py` & `phrase-api-1.9.1/test/test_translations_exclude_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_include_parameters.py` & `phrase-api-1.9.1/test/test_translations_include_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_review_parameters.py` & `phrase-api-1.9.1/test/test_translations_review_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_search_parameters.py` & `phrase-api-1.9.1/test/test_translations_search_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_unverify_parameters.py` & `phrase-api-1.9.1/test/test_translations_unverify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_translations_verify_parameters.py` & `phrase-api-1.9.1/test/test_translations_verify_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_upload.py` & `phrase-api-1.9.1/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_upload_create_parameters.py` & `phrase-api-1.9.1/test/test_upload_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_upload_summary.py` & `phrase-api-1.9.1/test/test_upload_summary.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_uploads_api.py` & `phrase-api-1.9.1/test/test_uploads_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_user.py` & `phrase-api-1.9.1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_user_preview.py` & `phrase-api-1.9.1/test/test_user_preview.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_users_api.py` & `phrase-api-1.9.1/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_variable.py` & `phrase-api-1.9.1/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_variable_create_parameters.py` & `phrase-api-1.9.1/test/test_variable_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_variable_update_parameters.py` & `phrase-api-1.9.1/test/test_variable_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_variables_api.py` & `phrase-api-1.9.1/test/test_variables_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_versions___history_api.py` & `phrase-api-1.9.1/test/test_versions___history_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhook.py` & `phrase-api-1.9.1/test/test_webhook.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhook_create_parameters.py` & `phrase-api-1.9.1/test/test_webhook_create_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhook_deliveries_api.py` & `phrase-api-1.9.1/test/test_webhook_deliveries_api.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhook_delivery.py` & `phrase-api-1.9.1/test/test_webhook_delivery.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhook_update_parameters.py` & `phrase-api-1.9.1/test/test_webhook_update_parameters.py`

 * *Files identical despite different names*

### Comparing `phrase-api-1.9.0/test/test_webhooks_api.py` & `phrase-api-1.9.1/test/test_webhooks_api.py`

 * *Files identical despite different names*


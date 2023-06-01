# Comparing `tmp/pulumi_gitlab-5.1.0a1685165842.tar.gz` & `tmp/pulumi_gitlab-6.0.0a1685643149.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-5.1.0a1685165842.tar", last modified: Sat May 27 05:48:03 2023, max compression
+gzip compressed data, was "pulumi_gitlab-6.0.0a1685643149.tar", last modified: Thu Jun  1 18:17:24 2023, max compression
```

## Comparing `pulumi_gitlab-5.1.0a1685165842.tar` & `pulumi_gitlab-6.0.0a1685643149.tar`

### file list

```diff
@@ -1,132 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/application.py
--rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/cluster_agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    44219 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_user_sshkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21008 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/managed_license.py
--rw-r--r--   0 runner    (1001) docker     (123)   164830 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pages_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)   263073 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    24116 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    45107 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    37942 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 05:48:03.000000 pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:48:03.175568 pulumi_gitlab-5.1.0a1685165842/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-27 05:48:02.000000 pulumi_gitlab-5.1.0a1685165842/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/cluster_agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43520 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24330 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_user_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23721 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26646 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45241 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59785 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165040 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20010 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   260430 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38116 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59807 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 18:17:24.000000 pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:17:24.086413 pulumi_gitlab-6.0.0a1685643149/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-01 18:17:23.000000 pulumi_gitlab-6.0.0a1685643149/setup.py
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/PKG-INFO` & `pulumi_gitlab-6.0.0a1685643149/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 5.1.0a1685165842
+Version: 6.0.0a1685643149
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -43,15 +43,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
 
@@ -60,15 +60,15 @@
 The `@pulumi/gitlab` package provides a strongly-typed means to create cloud applications that create and interact
 closely with GitLab resources.
 
 ## Configuration
 
 The following configuration points are available:
 
-* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`. 
+* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`.
 
 * base_url (Optional) - This is the target GitLab base API endpoint. Providing a value is a requirement when working with GitLab CE or GitLab Enterprise e.g. https://my.gitlab.server/api/v4/. It is optional to provide this value and it can also be sourced from the GITLAB_BASE_URL environment variable. The value must end with a slash.
 
 * cacert_file (Optional) - This is a file containing the ca cert to verify the gitlab instance. This is available for use when working with GitLab CE or Gitlab Enterprise with a locally-issued or self-signed certificate chain.
 
 * insecure (Optional) - When set to true this disables SSL verification of the connection to the GitLab instance. Defaults to `false`.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/README.md` & `pulumi_gitlab-6.0.0a1685643149/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -31,15 +31,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
 
@@ -48,15 +48,15 @@
 The `@pulumi/gitlab` package provides a strongly-typed means to create cloud applications that create and interact
 closely with GitLab resources.
 
 ## Configuration
 
 The following configuration points are available:
 
-* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`. 
+* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`.
 
 * base_url (Optional) - This is the target GitLab base API endpoint. Providing a value is a requirement when working with GitLab CE or GitLab Enterprise e.g. https://my.gitlab.server/api/v4/. It is optional to provide this value and it can also be sourced from the GITLAB_BASE_URL environment variable. The value must end with a slash.
 
 * cacert_file (Optional) - This is a file containing the ca cert to verify the gitlab instance. This is available for use when working with GitLab CE or Gitlab Enterprise with a locally-issued or self-signed certificate chain.
 
 * insecure (Optional) - When set to true this disables SSL verification of the connection to the GitLab instance. Defaults to `false`.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/__init__.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,16 +65,23 @@
 from .group_membership import *
 from .group_project_file_template import *
 from .group_saml_link import *
 from .group_share_group import *
 from .group_variable import *
 from .instance_cluster import *
 from .instance_variable import *
+from .integration_custom_issue_tracker import *
+from .integration_emails_on_push import *
+from .integration_external_wiki import *
+from .integration_github import *
+from .integration_jira import *
+from .integration_microsoft_teams import *
+from .integration_pipelines_email import *
+from .integration_slack import *
 from .label import *
-from .managed_license import *
 from .pages_domain import *
 from .personal_access_token import *
 from .pipeline_schedule import *
 from .pipeline_schedule_variable import *
 from .pipeline_trigger import *
 from .project import *
 from .project_access_token import *
@@ -83,14 +90,15 @@
 from .project_cluster import *
 from .project_custom_attribute import *
 from .project_environment import *
 from .project_freeze_period import *
 from .project_hook import *
 from .project_issue import *
 from .project_issue_board import *
+from .project_label import *
 from .project_level_mr_approvals import *
 from .project_membership import *
 from .project_milestone import *
 from .project_mirror import *
 from .project_protected_environment import *
 from .project_runner_enablement import *
 from .project_share_group import *
@@ -318,26 +326,82 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/instanceVariable:InstanceVariable": "InstanceVariable"
   }
  },
  {
   "pkg": "gitlab",
-  "mod": "index/label",
+  "mod": "index/integrationCustomIssueTracker",
   "fqn": "pulumi_gitlab",
   "classes": {
-   "gitlab:index/label:Label": "Label"
+   "gitlab:index/integrationCustomIssueTracker:IntegrationCustomIssueTracker": "IntegrationCustomIssueTracker"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationEmailsOnPush",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationEmailsOnPush:IntegrationEmailsOnPush": "IntegrationEmailsOnPush"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationExternalWiki",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationExternalWiki:IntegrationExternalWiki": "IntegrationExternalWiki"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationGithub",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationGithub:IntegrationGithub": "IntegrationGithub"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationJira",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationJira:IntegrationJira": "IntegrationJira"
   }
  },
  {
   "pkg": "gitlab",
-  "mod": "index/managedLicense",
+  "mod": "index/integrationMicrosoftTeams",
   "fqn": "pulumi_gitlab",
   "classes": {
-   "gitlab:index/managedLicense:ManagedLicense": "ManagedLicense"
+   "gitlab:index/integrationMicrosoftTeams:IntegrationMicrosoftTeams": "IntegrationMicrosoftTeams"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationPipelinesEmail",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationPipelinesEmail:IntegrationPipelinesEmail": "IntegrationPipelinesEmail"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/integrationSlack",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/integrationSlack:IntegrationSlack": "IntegrationSlack"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/label",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/label:Label": "Label"
   }
  },
  {
   "pkg": "gitlab",
   "mod": "index/pagesDomain",
   "fqn": "pulumi_gitlab",
   "classes": {
@@ -462,14 +526,22 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/projectIssueBoard:ProjectIssueBoard": "ProjectIssueBoard"
   }
  },
  {
   "pkg": "gitlab",
+  "mod": "index/projectLabel",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/projectLabel:ProjectLabel": "ProjectLabel"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/projectLevelMrApprovals",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/projectLevelMrApprovals:ProjectLevelMrApprovals": "ProjectLevelMrApprovals"
   }
  },
  {
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/application.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/application_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/branch.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,26 +80,30 @@
         pulumi.set(self, "can_push", value)
 
 
 @pulumi.input_type
 class _DeployKeyState:
     def __init__(__self__, *,
                  can_push: Optional[pulumi.Input[bool]] = None,
+                 deploy_key_id: Optional[pulumi.Input[int]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering DeployKey resources.
         :param pulumi.Input[bool] can_push: Allow this deploy key to be used to push changes to the project. Defaults to `false`.
+        :param pulumi.Input[int] deploy_key_id: The id of the project deploy key.
         :param pulumi.Input[str] key: The public ssh key body.
         :param pulumi.Input[str] project: The name or id of the project to add the deploy key to.
         :param pulumi.Input[str] title: A title to describe the deploy key with.
         """
         if can_push is not None:
             pulumi.set(__self__, "can_push", can_push)
+        if deploy_key_id is not None:
+            pulumi.set(__self__, "deploy_key_id", deploy_key_id)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
@@ -112,14 +116,26 @@
         return pulumi.get(self, "can_push")
 
     @can_push.setter
     def can_push(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "can_push", value)
 
     @property
+    @pulumi.getter(name="deployKeyId")
+    def deploy_key_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the project deploy key.
+        """
+        return pulumi.get(self, "deploy_key_id")
+
+    @deploy_key_id.setter
+    def deploy_key_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "deploy_key_id", value)
+
+    @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
         The public ssh key body.
         """
         return pulumi.get(self, "key")
 
@@ -271,59 +287,71 @@
             __props__.__dict__["key"] = key
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
             __props__.__dict__["title"] = title
+            __props__.__dict__["deploy_key_id"] = None
         super(DeployKey, __self__).__init__(
             'gitlab:index/deployKey:DeployKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             can_push: Optional[pulumi.Input[bool]] = None,
+            deploy_key_id: Optional[pulumi.Input[int]] = None,
             key: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             title: Optional[pulumi.Input[str]] = None) -> 'DeployKey':
         """
         Get an existing DeployKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] can_push: Allow this deploy key to be used to push changes to the project. Defaults to `false`.
+        :param pulumi.Input[int] deploy_key_id: The id of the project deploy key.
         :param pulumi.Input[str] key: The public ssh key body.
         :param pulumi.Input[str] project: The name or id of the project to add the deploy key to.
         :param pulumi.Input[str] title: A title to describe the deploy key with.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DeployKeyState.__new__(_DeployKeyState)
 
         __props__.__dict__["can_push"] = can_push
+        __props__.__dict__["deploy_key_id"] = deploy_key_id
         __props__.__dict__["key"] = key
         __props__.__dict__["project"] = project
         __props__.__dict__["title"] = title
         return DeployKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="canPush")
     def can_push(self) -> pulumi.Output[Optional[bool]]:
         """
         Allow this deploy key to be used to push changes to the project. Defaults to `false`.
         """
         return pulumi.get(self, "can_push")
 
     @property
+    @pulumi.getter(name="deployKeyId")
+    def deploy_key_id(self) -> pulumi.Output[int]:
+        """
+        The id of the project deploy key.
+        """
+        return pulumi.get(self, "deploy_key_id")
+
+    @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
         """
         The public ssh key body.
         """
         return pulumi.get(self, "key")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_key_enable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/deploy_token.py`

 * *Files 13% similar despite different names*

```diff
@@ -113,31 +113,35 @@
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
 class _DeployTokenState:
     def __init__(__self__, *,
+                 deploy_token_id: Optional[pulumi.Input[int]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering DeployToken resources.
+        :param pulumi.Input[int] deploy_token_id: The id of the deploy token.
         :param pulumi.Input[str] expires_at: Time the token will expire it, RFC3339 format. Will not expire per default.
         :param pulumi.Input[str] group: The name or id of the group to add the deploy token to.
         :param pulumi.Input[str] name: A name to describe the deploy token with.
         :param pulumi.Input[str] project: The name or id of the project to add the deploy token to.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `read_repository`, `read_registry`, `read_package_registry`, `write_registry`, `write_package_registry`.
         :param pulumi.Input[str] token: The secret token. This is only populated when creating a new deploy token. **Note**: The token is not available for imported resources.
         :param pulumi.Input[str] username: A username for the deploy token. Default is `gitlab+deploy-token-{n}`.
         """
+        if deploy_token_id is not None:
+            pulumi.set(__self__, "deploy_token_id", deploy_token_id)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
@@ -146,14 +150,26 @@
             pulumi.set(__self__, "scopes", scopes)
         if token is not None:
             pulumi.set(__self__, "token", token)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
+    @pulumi.getter(name="deployTokenId")
+    def deploy_token_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the deploy token.
+        """
+        return pulumi.get(self, "deploy_token_id")
+
+    @deploy_token_id.setter
+    def deploy_token_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "deploy_token_id", value)
+
+    @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
         Time the token will expire it, RFC3339 format. Will not expire per default.
         """
         return pulumi.get(self, "expires_at")
 
@@ -333,63 +349,75 @@
             __props__.__dict__["group"] = group
             __props__.__dict__["name"] = name
             __props__.__dict__["project"] = project
             if scopes is None and not opts.urn:
                 raise TypeError("Missing required property 'scopes'")
             __props__.__dict__["scopes"] = scopes
             __props__.__dict__["username"] = username
+            __props__.__dict__["deploy_token_id"] = None
             __props__.__dict__["token"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["token"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(DeployToken, __self__).__init__(
             'gitlab:index/deployToken:DeployToken',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            deploy_token_id: Optional[pulumi.Input[int]] = None,
             expires_at: Optional[pulumi.Input[str]] = None,
             group: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             token: Optional[pulumi.Input[str]] = None,
             username: Optional[pulumi.Input[str]] = None) -> 'DeployToken':
         """
         Get an existing DeployToken resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[int] deploy_token_id: The id of the deploy token.
         :param pulumi.Input[str] expires_at: Time the token will expire it, RFC3339 format. Will not expire per default.
         :param pulumi.Input[str] group: The name or id of the group to add the deploy token to.
         :param pulumi.Input[str] name: A name to describe the deploy token with.
         :param pulumi.Input[str] project: The name or id of the project to add the deploy token to.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `read_repository`, `read_registry`, `read_package_registry`, `write_registry`, `write_package_registry`.
         :param pulumi.Input[str] token: The secret token. This is only populated when creating a new deploy token. **Note**: The token is not available for imported resources.
         :param pulumi.Input[str] username: A username for the deploy token. Default is `gitlab+deploy-token-{n}`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DeployTokenState.__new__(_DeployTokenState)
 
+        __props__.__dict__["deploy_token_id"] = deploy_token_id
         __props__.__dict__["expires_at"] = expires_at
         __props__.__dict__["group"] = group
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
         __props__.__dict__["scopes"] = scopes
         __props__.__dict__["token"] = token
         __props__.__dict__["username"] = username
         return DeployToken(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="deployTokenId")
+    def deploy_token_id(self) -> pulumi.Output[int]:
+        """
+        The id of the deploy token.
+        """
+        return pulumi.get(self, "deploy_token_id")
+
+    @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> pulumi.Output[Optional[str]]:
         """
         Time the token will expire it, RFC3339 format. Will not expire per default.
         """
         return pulumi.get(self, "expires_at")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_application.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_cluster_agents.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_current_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_subgroups.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_subgroups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetGroupVariableResult:
     """
     A collection of values returned by getGroupVariable.
     """
-    def __init__(__self__, environment_scope=None, group=None, id=None, key=None, masked=None, protected=None, value=None, variable_type=None):
+    def __init__(__self__, environment_scope=None, group=None, id=None, key=None, masked=None, protected=None, raw=None, value=None, variable_type=None):
         if environment_scope and not isinstance(environment_scope, str):
             raise TypeError("Expected argument 'environment_scope' to be a str")
         pulumi.set(__self__, "environment_scope", environment_scope)
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
         pulumi.set(__self__, "group", group)
         if id and not isinstance(id, str):
@@ -36,14 +36,17 @@
         pulumi.set(__self__, "key", key)
         if masked and not isinstance(masked, bool):
             raise TypeError("Expected argument 'masked' to be a bool")
         pulumi.set(__self__, "masked", masked)
         if protected and not isinstance(protected, bool):
             raise TypeError("Expected argument 'protected' to be a bool")
         pulumi.set(__self__, "protected", protected)
+        if raw and not isinstance(raw, bool):
+            raise TypeError("Expected argument 'raw' to be a bool")
+        pulumi.set(__self__, "raw", raw)
         if value and not isinstance(value, str):
             raise TypeError("Expected argument 'value' to be a str")
         pulumi.set(__self__, "value", value)
         if variable_type and not isinstance(variable_type, str):
             raise TypeError("Expected argument 'variable_type' to be a str")
         pulumi.set(__self__, "variable_type", variable_type)
 
@@ -93,14 +96,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
@@ -120,14 +131,15 @@
         return GetGroupVariableResult(
             environment_scope=self.environment_scope,
             group=self.group,
             id=self.id,
             key=self.key,
             masked=self.masked,
             protected=self.protected,
+            raw=self.raw,
             value=self.value,
             variable_type=self.variable_type)
 
 
 def get_group_variable(environment_scope: Optional[str] = None,
                        group: Optional[str] = None,
                        key: Optional[str] = None,
@@ -165,14 +177,15 @@
     return AwaitableGetGroupVariableResult(
         environment_scope=__ret__.environment_scope,
         group=__ret__.group,
         id=__ret__.id,
         key=__ret__.key,
         masked=__ret__.masked,
         protected=__ret__.protected,
+        raw=__ret__.raw,
         value=__ret__.value,
         variable_type=__ret__.variable_type)
 
 
 @_utilities.lift_output_func(get_group_variable)
 def get_group_variable_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                               group: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_group_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_groups.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 ]
 
 @pulumi.output_type
 class GetInstanceVariableResult:
     """
     A collection of values returned by getInstanceVariable.
     """
-    def __init__(__self__, id=None, key=None, masked=None, protected=None, value=None, variable_type=None):
+    def __init__(__self__, id=None, key=None, masked=None, protected=None, raw=None, value=None, variable_type=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if key and not isinstance(key, str):
             raise TypeError("Expected argument 'key' to be a str")
         pulumi.set(__self__, "key", key)
         if masked and not isinstance(masked, bool):
             raise TypeError("Expected argument 'masked' to be a bool")
         pulumi.set(__self__, "masked", masked)
         if protected and not isinstance(protected, bool):
             raise TypeError("Expected argument 'protected' to be a bool")
         pulumi.set(__self__, "protected", protected)
+        if raw and not isinstance(raw, bool):
+            raise TypeError("Expected argument 'raw' to be a bool")
+        pulumi.set(__self__, "raw", raw)
         if value and not isinstance(value, str):
             raise TypeError("Expected argument 'value' to be a str")
         pulumi.set(__self__, "value", value)
         if variable_type and not isinstance(variable_type, str):
             raise TypeError("Expected argument 'variable_type' to be a str")
         pulumi.set(__self__, "variable_type", variable_type)
 
@@ -71,14 +74,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
@@ -96,14 +107,15 @@
         if False:
             yield self
         return GetInstanceVariableResult(
             id=self.id,
             key=self.key,
             masked=self.masked,
             protected=self.protected,
+            raw=self.raw,
             value=self.value,
             variable_type=self.variable_type)
 
 
 def get_instance_variable(key: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstanceVariableResult:
     """
@@ -129,14 +141,15 @@
     __ret__ = pulumi.runtime.invoke('gitlab:index/getInstanceVariable:getInstanceVariable', __args__, opts=opts, typ=GetInstanceVariableResult).value
 
     return AwaitableGetInstanceVariableResult(
         id=__ret__.id,
         key=__ret__.key,
         masked=__ret__.masked,
         protected=__ret__.protected,
+        raw=__ret__.raw,
         value=__ret__.value,
         variable_type=__ret__.variable_type)
 
 
 @_utilities.lift_output_func(get_instance_variable)
 def get_instance_variable_output(key: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceVariableResult]:
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_instance_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_metadata.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, ci_separated_caches=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, environments_access_level=None, external_authorization_classification_label=None, feature_flags_access_level=None, forking_access_level=None, http_url_to_repo=None, id=None, import_url=None, infrastructure_access_level=None, issues_access_level=None, issues_enabled=None, keep_latest_artifact=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, monitor_access_level=None, name=None, namespace_id=None, operations_access_level=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, releases_access_level=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, restrict_user_defined_variables=None, runners_token=None, security_and_compliance_access_level=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, suggestion_commit_message=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
+    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, ci_separated_caches=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, environments_access_level=None, external_authorization_classification_label=None, feature_flags_access_level=None, forking_access_level=None, http_url_to_repo=None, id=None, import_url=None, infrastructure_access_level=None, issues_access_level=None, issues_enabled=None, keep_latest_artifact=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, monitor_access_level=None, name=None, namespace_id=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, releases_access_level=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, restrict_user_defined_variables=None, runners_token=None, security_and_compliance_access_level=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, suggestion_commit_message=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
         if analytics_access_level and not isinstance(analytics_access_level, str):
             raise TypeError("Expected argument 'analytics_access_level' to be a str")
         pulumi.set(__self__, "analytics_access_level", analytics_access_level)
         if archived and not isinstance(archived, bool):
             raise TypeError("Expected argument 'archived' to be a bool")
         pulumi.set(__self__, "archived", archived)
         if auto_cancel_pending_pipelines and not isinstance(auto_cancel_pending_pipelines, str):
@@ -130,17 +130,14 @@
         pulumi.set(__self__, "monitor_access_level", monitor_access_level)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if namespace_id and not isinstance(namespace_id, int):
             raise TypeError("Expected argument 'namespace_id' to be a int")
         pulumi.set(__self__, "namespace_id", namespace_id)
-        if operations_access_level and not isinstance(operations_access_level, str):
-            raise TypeError("Expected argument 'operations_access_level' to be a str")
-        pulumi.set(__self__, "operations_access_level", operations_access_level)
         if path and not isinstance(path, str):
             raise TypeError("Expected argument 'path' to be a str")
         pulumi.set(__self__, "path", path)
         if path_with_namespace and not isinstance(path_with_namespace, str):
             raise TypeError("Expected argument 'path_with_namespace' to be a str")
         pulumi.set(__self__, "path_with_namespace", path_with_namespace)
         if pipelines_enabled and not isinstance(pipelines_enabled, bool):
@@ -509,22 +506,14 @@
     def namespace_id(self) -> int:
         """
         The namespace (group or user) of the project. Defaults to your user.
         """
         return pulumi.get(self, "namespace_id")
 
     @property
-    @pulumi.getter(name="operationsAccessLevel")
-    def operations_access_level(self) -> str:
-        """
-        Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
-        """
-        return pulumi.get(self, "operations_access_level")
-
-    @property
     @pulumi.getter
     def path(self) -> str:
         """
         The path of the repository.
         """
         return pulumi.get(self, "path")
 
@@ -768,15 +757,14 @@
             merge_pipelines_enabled=self.merge_pipelines_enabled,
             merge_requests_access_level=self.merge_requests_access_level,
             merge_requests_enabled=self.merge_requests_enabled,
             merge_trains_enabled=self.merge_trains_enabled,
             monitor_access_level=self.monitor_access_level,
             name=self.name,
             namespace_id=self.namespace_id,
-            operations_access_level=self.operations_access_level,
             path=self.path,
             path_with_namespace=self.path_with_namespace,
             pipelines_enabled=self.pipelines_enabled,
             printing_merge_request_link_enabled=self.printing_merge_request_link_enabled,
             public_builds=self.public_builds,
             push_rules=self.push_rules,
             releases_access_level=self.releases_access_level,
@@ -868,15 +856,14 @@
         merge_pipelines_enabled=__ret__.merge_pipelines_enabled,
         merge_requests_access_level=__ret__.merge_requests_access_level,
         merge_requests_enabled=__ret__.merge_requests_enabled,
         merge_trains_enabled=__ret__.merge_trains_enabled,
         monitor_access_level=__ret__.monitor_access_level,
         name=__ret__.name,
         namespace_id=__ret__.namespace_id,
-        operations_access_level=__ret__.operations_access_level,
         path=__ret__.path,
         path_with_namespace=__ret__.path_with_namespace,
         pipelines_enabled=__ret__.pipelines_enabled,
         printing_merge_request_link_enabled=__ret__.printing_merge_request_link_enabled,
         public_builds=__ret__.public_builds,
         push_rules=__ret__.push_rules,
         releases_access_level=__ret__.releases_access_level,
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_branches.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    foo = gitlab.get_project(id="foo/bar/baz")
+    foo = gitlab.get_project(path_with_namespace="foo/bar/baz")
     welcome_issue = gitlab.get_project_issue(project=foo.id,
         iid=1)
     pulumi.export("welcomeIssueWebUrl", data["gitlab_project_issue"]["web_url"])
     ```
 
 
     :param int iid: The internal ID of the project's issue.
@@ -597,15 +597,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    foo = gitlab.get_project(id="foo/bar/baz")
+    foo = gitlab.get_project(path_with_namespace="foo/bar/baz")
     welcome_issue = gitlab.get_project_issue(project=foo.id,
         iid=1)
     pulumi.export("welcomeIssueWebUrl", data["gitlab_project_issue"]["web_url"])
     ```
 
 
     :param int iid: The internal ID of the project's issue.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_issues.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_milestones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_protected_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_protected_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectVariableResult:
     """
     A collection of values returned by getProjectVariable.
     """
-    def __init__(__self__, environment_scope=None, id=None, key=None, masked=None, project=None, protected=None, value=None, variable_type=None):
+    def __init__(__self__, environment_scope=None, id=None, key=None, masked=None, project=None, protected=None, raw=None, value=None, variable_type=None):
         if environment_scope and not isinstance(environment_scope, str):
             raise TypeError("Expected argument 'environment_scope' to be a str")
         pulumi.set(__self__, "environment_scope", environment_scope)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if key and not isinstance(key, str):
@@ -36,14 +36,17 @@
         pulumi.set(__self__, "masked", masked)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if protected and not isinstance(protected, bool):
             raise TypeError("Expected argument 'protected' to be a bool")
         pulumi.set(__self__, "protected", protected)
+        if raw and not isinstance(raw, bool):
+            raise TypeError("Expected argument 'raw' to be a bool")
+        pulumi.set(__self__, "raw", raw)
         if value and not isinstance(value, str):
             raise TypeError("Expected argument 'value' to be a str")
         pulumi.set(__self__, "value", value)
         if variable_type and not isinstance(variable_type, str):
             raise TypeError("Expected argument 'variable_type' to be a str")
         pulumi.set(__self__, "variable_type", variable_type)
 
@@ -93,14 +96,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
@@ -120,14 +131,15 @@
         return GetProjectVariableResult(
             environment_scope=self.environment_scope,
             id=self.id,
             key=self.key,
             masked=self.masked,
             project=self.project,
             protected=self.protected,
+            raw=self.raw,
             value=self.value,
             variable_type=self.variable_type)
 
 
 def get_project_variable(environment_scope: Optional[str] = None,
                          key: Optional[str] = None,
                          project: Optional[str] = None,
@@ -165,14 +177,15 @@
     return AwaitableGetProjectVariableResult(
         environment_scope=__ret__.environment_scope,
         id=__ret__.id,
         key=__ret__.key,
         masked=__ret__.masked,
         project=__ret__.project,
         protected=__ret__.protected,
+        raw=__ret__.raw,
         value=__ret__.value,
         variable_type=__ret__.variable_type)
 
 
 @_utilities.lift_output_func(get_project_variable)
 def get_project_variable_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                                 key: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_project_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_release_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_repository_file.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_repository_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_user.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_user_sshkeys.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_user_sshkeys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/get_users.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GroupAccessToken resource.
         :param pulumi.Input[str] group: The ID or path of the group to add the group access token to.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the group access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_api`, `read_registry`, `write_registry`, `read_repository`, `write_repository`.
         :param pulumi.Input[str] access_level: The access level for the group access token. Valid values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] name: The name of the group access token.
         """
         pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "scopes", scopes)
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if expires_at is not None:
@@ -72,15 +72,15 @@
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -111,15 +111,15 @@
                  token: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering GroupAccessToken resources.
         :param pulumi.Input[str] access_level: The access level for the group access token. Valid values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] group: The ID or path of the group to add the group access token to.
         :param pulumi.Input[str] name: The name of the group access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the group access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_api`, `read_registry`, `write_registry`, `read_repository`, `write_repository`.
         :param pulumi.Input[str] token: The group access token. This is only populated when creating a new group access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The user id associated to the token.
         """
@@ -180,15 +180,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -309,15 +309,15 @@
         ```
 
          ATTENTIONthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the group access token. Valid values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] group: The ID or path of the group to add the group access token to.
         :param pulumi.Input[str] name: The name of the group access token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the group access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_api`, `read_registry`, `write_registry`, `read_repository`, `write_repository`.
         """
         ...
     @overload
     def __init__(__self__,
@@ -429,15 +429,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the group access token. Valid values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] group: The ID or path of the group to add the group access token to.
         :param pulumi.Input[str] name: The name of the group access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the group access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_api`, `read_registry`, `write_registry`, `read_repository`, `write_repository`.
         :param pulumi.Input[str] token: The group access token. This is only populated when creating a new group access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The user id associated to the token.
         """
@@ -479,17 +479,17 @@
         """
         Time the token has been created, RFC3339 format.
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> pulumi.Output[Optional[str]]:
+    def expires_at(self) -> pulumi.Output[str]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @property
     @pulumi.getter
     def group(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_label.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,28 +83,32 @@
 
 @pulumi.input_type
 class _GroupLabelState:
     def __init__(__self__, *,
                  color: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
+                 label_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering GroupLabel resources.
         :param pulumi.Input[str] color: The color of the label given in 6-digit hex notation with leading '#' sign (e.g. #FFAABB) or one of the [CSS color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords).
         :param pulumi.Input[str] description: The description of the label.
         :param pulumi.Input[str] group: The name or id of the group to add the label to.
+        :param pulumi.Input[int] label_id: The id of the group label.
         :param pulumi.Input[str] name: The name of the label.
         """
         if color is not None:
             pulumi.set(__self__, "color", color)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if group is not None:
             pulumi.set(__self__, "group", group)
+        if label_id is not None:
+            pulumi.set(__self__, "label_id", label_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def color(self) -> Optional[pulumi.Input[str]]:
         """
@@ -137,14 +141,26 @@
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
+    @pulumi.getter(name="labelId")
+    def label_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the group label.
+        """
+        return pulumi.get(self, "label_id")
+
+    @label_id.setter
+    def label_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "label_id", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the label.
         """
         return pulumi.get(self, "name")
 
@@ -258,47 +274,51 @@
                 raise TypeError("Missing required property 'color'")
             __props__.__dict__["color"] = color
             __props__.__dict__["description"] = description
             if group is None and not opts.urn:
                 raise TypeError("Missing required property 'group'")
             __props__.__dict__["group"] = group
             __props__.__dict__["name"] = name
+            __props__.__dict__["label_id"] = None
         super(GroupLabel, __self__).__init__(
             'gitlab:index/groupLabel:GroupLabel',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             color: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             group: Optional[pulumi.Input[str]] = None,
+            label_id: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None) -> 'GroupLabel':
         """
         Get an existing GroupLabel resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] color: The color of the label given in 6-digit hex notation with leading '#' sign (e.g. #FFAABB) or one of the [CSS color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords).
         :param pulumi.Input[str] description: The description of the label.
         :param pulumi.Input[str] group: The name or id of the group to add the label to.
+        :param pulumi.Input[int] label_id: The id of the group label.
         :param pulumi.Input[str] name: The name of the label.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupLabelState.__new__(_GroupLabelState)
 
         __props__.__dict__["color"] = color
         __props__.__dict__["description"] = description
         __props__.__dict__["group"] = group
+        __props__.__dict__["label_id"] = label_id
         __props__.__dict__["name"] = name
         return GroupLabel(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def color(self) -> pulumi.Output[str]:
         """
@@ -319,14 +339,22 @@
     def group(self) -> pulumi.Output[str]:
         """
         The name or id of the group to add the label to.
         """
         return pulumi.get(self, "group")
 
     @property
+    @pulumi.getter(name="labelId")
+    def label_id(self) -> pulumi.Output[int]:
+        """
+        The id of the group label.
+        """
+        return pulumi.get(self, "label_id")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the label.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_ldap_link.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,65 +10,58 @@
 from . import _utilities
 
 __all__ = ['GroupLdapLinkArgs', 'GroupLdapLink']
 
 @pulumi.input_type
 class GroupLdapLinkArgs:
     def __init__(__self__, *,
-                 cn: pulumi.Input[str],
-                 group_id: pulumi.Input[str],
+                 group: pulumi.Input[str],
                  ldap_provider: pulumi.Input[str],
                  access_level: Optional[pulumi.Input[str]] = None,
+                 cn: Optional[pulumi.Input[str]] = None,
+                 filter: Optional[pulumi.Input[str]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
                  group_access: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GroupLdapLink resource.
-        :param pulumi.Input[str] cn: The CN of the LDAP group to link with.
-        :param pulumi.Input[str] group_id: The id of the GitLab group.
+        :param pulumi.Input[str] group: The ID or URL-encoded path of the group
         :param pulumi.Input[str] ldap_provider: The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         :param pulumi.Input[str] access_level: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
+        :param pulumi.Input[str] cn: The CN of the LDAP group to link with. Required if `filter` is not provided.
+        :param pulumi.Input[str] filter: The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
         :param pulumi.Input[bool] force: If true, then delete and replace an existing LDAP link if one exists.
         :param pulumi.Input[str] group_access: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
-        pulumi.set(__self__, "cn", cn)
-        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "ldap_provider", ldap_provider)
         if access_level is not None:
             warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
             pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
+        if cn is not None:
+            pulumi.set(__self__, "cn", cn)
+        if filter is not None:
+            pulumi.set(__self__, "filter", filter)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if group_access is not None:
             pulumi.set(__self__, "group_access", group_access)
 
     @property
     @pulumi.getter
-    def cn(self) -> pulumi.Input[str]:
-        """
-        The CN of the LDAP group to link with.
-        """
-        return pulumi.get(self, "cn")
-
-    @cn.setter
-    def cn(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cn", value)
-
-    @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> pulumi.Input[str]:
+    def group(self) -> pulumi.Input[str]:
         """
-        The id of the GitLab group.
+        The ID or URL-encoded path of the group
         """
-        return pulumi.get(self, "group_id")
+        return pulumi.get(self, "group")
 
-    @group_id.setter
-    def group_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "group_id", value)
+    @group.setter
+    def group(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter(name="ldapProvider")
     def ldap_provider(self) -> pulumi.Input[str]:
         """
         The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
@@ -88,14 +81,38 @@
 
     @access_level.setter
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
     @pulumi.getter
+    def cn(self) -> Optional[pulumi.Input[str]]:
+        """
+        The CN of the LDAP group to link with. Required if `filter` is not provided.
+        """
+        return pulumi.get(self, "cn")
+
+    @cn.setter
+    def cn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cn", value)
+
+    @property
+    @pulumi.getter
+    def filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
+        """
+        return pulumi.get(self, "filter")
+
+    @filter.setter
+    def filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "filter", value)
+
+    @property
+    @pulumi.getter
     def force(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, then delete and replace an existing LDAP link if one exists.
         """
         return pulumi.get(self, "force")
 
     @force.setter
@@ -116,40 +133,44 @@
 
 
 @pulumi.input_type
 class _GroupLdapLinkState:
     def __init__(__self__, *,
                  access_level: Optional[pulumi.Input[str]] = None,
                  cn: Optional[pulumi.Input[str]] = None,
+                 filter: Optional[pulumi.Input[str]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 group: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
                  ldap_provider: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering GroupLdapLink resources.
         :param pulumi.Input[str] access_level: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] cn: The CN of the LDAP group to link with.
+        :param pulumi.Input[str] cn: The CN of the LDAP group to link with. Required if `filter` is not provided.
+        :param pulumi.Input[str] filter: The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
         :param pulumi.Input[bool] force: If true, then delete and replace an existing LDAP link if one exists.
+        :param pulumi.Input[str] group: The ID or URL-encoded path of the group
         :param pulumi.Input[str] group_access: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] group_id: The id of the GitLab group.
         :param pulumi.Input[str] ldap_provider: The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
         if access_level is not None:
             warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
             pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if cn is not None:
             pulumi.set(__self__, "cn", cn)
+        if filter is not None:
+            pulumi.set(__self__, "filter", filter)
         if force is not None:
             pulumi.set(__self__, "force", force)
+        if group is not None:
+            pulumi.set(__self__, "group", group)
         if group_access is not None:
             pulumi.set(__self__, "group_access", group_access)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
         if ldap_provider is not None:
             pulumi.set(__self__, "ldap_provider", ldap_provider)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
@@ -161,59 +182,71 @@
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
     @pulumi.getter
     def cn(self) -> Optional[pulumi.Input[str]]:
         """
-        The CN of the LDAP group to link with.
+        The CN of the LDAP group to link with. Required if `filter` is not provided.
         """
         return pulumi.get(self, "cn")
 
     @cn.setter
     def cn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cn", value)
 
     @property
     @pulumi.getter
+    def filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
+        """
+        return pulumi.get(self, "filter")
+
+    @filter.setter
+    def filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "filter", value)
+
+    @property
+    @pulumi.getter
     def force(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, then delete and replace an existing LDAP link if one exists.
         """
         return pulumi.get(self, "force")
 
     @force.setter
     def force(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force", value)
 
     @property
+    @pulumi.getter
+    def group(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID or URL-encoded path of the group
+        """
+        return pulumi.get(self, "group")
+
+    @group.setter
+    def group(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "group", value)
+
+    @property
     @pulumi.getter(name="groupAccess")
     def group_access(self) -> Optional[pulumi.Input[str]]:
         """
         Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
         return pulumi.get(self, "group_access")
 
     @group_access.setter
     def group_access(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_access", value)
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The id of the GitLab group.
-        """
-        return pulumi.get(self, "group_id")
-
-    @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_id", value)
-
-    @property
     @pulumi.getter(name="ldapProvider")
     def ldap_provider(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
         return pulumi.get(self, "ldap_provider")
 
@@ -225,84 +258,72 @@
 class GroupLdapLink(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  cn: Optional[pulumi.Input[str]] = None,
+                 filter: Optional[pulumi.Input[str]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 group: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
                  ldap_provider: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `GroupLdapLink` resource allows to manage the lifecycle of an LDAP integration with a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#ldap-group-links)
 
-        ## Example Usage
+        ## Import
 
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        test = gitlab.GroupLdapLink("test",
-            cn="testuser",
-            group_access="developer",
-            group_id="12345",
-            ldap_provider="ldapmain")
-        ```
+        GitLab group ldap links can be imported using an id made up of `group_id:ldap_provider:cn:filter`. CN and Filter are mutually exclusive, so one will be missing. If using the CN for the group link, the ID will end with a blank filter (":"). e.g.,
 
-        ## Import
+        ```sh
+         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain:testcn:"
+        ```
 
-        GitLab group ldap links can be imported using an id made up of `group_id:ldap_provider:cn`, e.g.
+         If using the Filter for the group link, the ID will have two "::" in the middle due to having a blank CN. e.g.,
 
         ```sh
-         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain:testuser"
+         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain::testfilter"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] cn: The CN of the LDAP group to link with.
+        :param pulumi.Input[str] cn: The CN of the LDAP group to link with. Required if `filter` is not provided.
+        :param pulumi.Input[str] filter: The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
         :param pulumi.Input[bool] force: If true, then delete and replace an existing LDAP link if one exists.
+        :param pulumi.Input[str] group: The ID or URL-encoded path of the group
         :param pulumi.Input[str] group_access: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] group_id: The id of the GitLab group.
         :param pulumi.Input[str] ldap_provider: The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupLdapLinkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `GroupLdapLink` resource allows to manage the lifecycle of an LDAP integration with a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#ldap-group-links)
 
-        ## Example Usage
+        ## Import
 
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        test = gitlab.GroupLdapLink("test",
-            cn="testuser",
-            group_access="developer",
-            group_id="12345",
-            ldap_provider="ldapmain")
-        ```
+        GitLab group ldap links can be imported using an id made up of `group_id:ldap_provider:cn:filter`. CN and Filter are mutually exclusive, so one will be missing. If using the CN for the group link, the ID will end with a blank filter (":"). e.g.,
 
-        ## Import
+        ```sh
+         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain:testcn:"
+        ```
 
-        GitLab group ldap links can be imported using an id made up of `group_id:ldap_provider:cn`, e.g.
+         If using the Filter for the group link, the ID will have two "::" in the middle due to having a blank CN. e.g.,
 
         ```sh
-         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain:testuser"
+         $ pulumi import gitlab:index/groupLdapLink:GroupLdapLink test "12345:ldapmain::testfilter"
         ```
 
         :param str resource_name: The name of the resource.
         :param GroupLdapLinkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -314,39 +335,39 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  cn: Optional[pulumi.Input[str]] = None,
+                 filter: Optional[pulumi.Input[str]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 group: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
                  ldap_provider: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupLdapLinkArgs.__new__(GroupLdapLinkArgs)
 
             if access_level is not None and not opts.urn:
                 warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
                 pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
             __props__.__dict__["access_level"] = access_level
-            if cn is None and not opts.urn:
-                raise TypeError("Missing required property 'cn'")
             __props__.__dict__["cn"] = cn
+            __props__.__dict__["filter"] = filter
             __props__.__dict__["force"] = force
+            if group is None and not opts.urn:
+                raise TypeError("Missing required property 'group'")
+            __props__.__dict__["group"] = group
             __props__.__dict__["group_access"] = group_access
-            if group_id is None and not opts.urn:
-                raise TypeError("Missing required property 'group_id'")
-            __props__.__dict__["group_id"] = group_id
             if ldap_provider is None and not opts.urn:
                 raise TypeError("Missing required property 'ldap_provider'")
             __props__.__dict__["ldap_provider"] = ldap_provider
         super(GroupLdapLink, __self__).__init__(
             'gitlab:index/groupLdapLink:GroupLdapLink',
             resource_name,
             __props__,
@@ -354,41 +375,44 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_level: Optional[pulumi.Input[str]] = None,
             cn: Optional[pulumi.Input[str]] = None,
+            filter: Optional[pulumi.Input[str]] = None,
             force: Optional[pulumi.Input[bool]] = None,
+            group: Optional[pulumi.Input[str]] = None,
             group_access: Optional[pulumi.Input[str]] = None,
-            group_id: Optional[pulumi.Input[str]] = None,
             ldap_provider: Optional[pulumi.Input[str]] = None) -> 'GroupLdapLink':
         """
         Get an existing GroupLdapLink resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] cn: The CN of the LDAP group to link with.
+        :param pulumi.Input[str] cn: The CN of the LDAP group to link with. Required if `filter` is not provided.
+        :param pulumi.Input[str] filter: The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
         :param pulumi.Input[bool] force: If true, then delete and replace an existing LDAP link if one exists.
+        :param pulumi.Input[str] group: The ID or URL-encoded path of the group
         :param pulumi.Input[str] group_access: Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] group_id: The id of the GitLab group.
         :param pulumi.Input[str] ldap_provider: The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupLdapLinkState.__new__(_GroupLdapLinkState)
 
         __props__.__dict__["access_level"] = access_level
         __props__.__dict__["cn"] = cn
+        __props__.__dict__["filter"] = filter
         __props__.__dict__["force"] = force
+        __props__.__dict__["group"] = group
         __props__.__dict__["group_access"] = group_access
-        __props__.__dict__["group_id"] = group_id
         __props__.__dict__["ldap_provider"] = ldap_provider
         return GroupLdapLink(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Output[Optional[str]]:
         """
@@ -396,41 +420,49 @@
         """
         return pulumi.get(self, "access_level")
 
     @property
     @pulumi.getter
     def cn(self) -> pulumi.Output[str]:
         """
-        The CN of the LDAP group to link with.
+        The CN of the LDAP group to link with. Required if `filter` is not provided.
         """
         return pulumi.get(self, "cn")
 
     @property
     @pulumi.getter
+    def filter(self) -> pulumi.Output[str]:
+        """
+        The LDAP filter for the group. Required if `cn` is not provided. Requires GitLab Premium or above.
+        """
+        return pulumi.get(self, "filter")
+
+    @property
+    @pulumi.getter
     def force(self) -> pulumi.Output[Optional[bool]]:
         """
         If true, then delete and replace an existing LDAP link if one exists.
         """
         return pulumi.get(self, "force")
 
     @property
-    @pulumi.getter(name="groupAccess")
-    def group_access(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def group(self) -> pulumi.Output[str]:
         """
-        Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
+        The ID or URL-encoded path of the group
         """
-        return pulumi.get(self, "group_access")
+        return pulumi.get(self, "group")
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="groupAccess")
+    def group_access(self) -> pulumi.Output[Optional[str]]:
         """
-        The id of the GitLab group.
+        Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
-        return pulumi.get(self, "group_id")
+        return pulumi.get(self, "group_access")
 
     @property
     @pulumi.getter(name="ldapProvider")
     def ldap_provider(self) -> pulumi.Output[str]:
         """
         The name of the LDAP provider as stored in the GitLab database. Note that this is NOT the value of the `label` attribute as shown in the web UI. In most cases this will be `ldapmain` but you may use the [LDAP check rake task](https://docs.gitlab.com/ee/administration/raketasks/ldap.html#check) for receiving the LDAP server name: `LDAP: ... Server: ldapmain`
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_project_file_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_saml_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/group_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,38 @@
     def __init__(__self__, *,
                  group: pulumi.Input[str],
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GroupVariable resource.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter
     def group(self) -> pulumi.Input[str]:
         """
@@ -112,14 +116,26 @@
         return pulumi.get(self, "protected")
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
+    @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         return pulumi.get(self, "variable_type")
 
@@ -132,36 +148,40 @@
 class _GroupVariableState:
     def __init__(__self__, *,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering GroupVariable resources.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if value is not None:
             pulumi.set(__self__, "value", value)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter(name="environmentScope")
@@ -221,14 +241,26 @@
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
     @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
+    @pulumi.getter
     def value(self) -> Optional[pulumi.Input[str]]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @value.setter
@@ -254,14 +286,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `GroupVariable` resource allows to manage the lifecycle of a CI/CD variable for a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/group_level_variables.html)
@@ -292,14 +325,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -349,14 +383,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -369,20 +404,19 @@
                 raise TypeError("Missing required property 'group'")
             __props__.__dict__["group"] = group
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["masked"] = masked
             __props__.__dict__["protected"] = protected
+            __props__.__dict__["raw"] = raw
             if value is None and not opts.urn:
                 raise TypeError("Missing required property 'value'")
-            __props__.__dict__["value"] = None if value is None else pulumi.Output.secret(value)
+            __props__.__dict__["value"] = value
             __props__.__dict__["variable_type"] = variable_type
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["value"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(GroupVariable, __self__).__init__(
             'gitlab:index/groupVariable:GroupVariable',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -390,40 +424,43 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             environment_scope: Optional[pulumi.Input[str]] = None,
             group: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             masked: Optional[pulumi.Input[bool]] = None,
             protected: Optional[pulumi.Input[bool]] = None,
+            raw: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None,
             variable_type: Optional[pulumi.Input[str]] = None) -> 'GroupVariable':
         """
         Get an existing GroupVariable resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupVariableState.__new__(_GroupVariableState)
 
         __props__.__dict__["environment_scope"] = environment_scope
         __props__.__dict__["group"] = group
         __props__.__dict__["key"] = key
         __props__.__dict__["masked"] = masked
         __props__.__dict__["protected"] = protected
+        __props__.__dict__["raw"] = raw
         __props__.__dict__["value"] = value
         __props__.__dict__["variable_type"] = variable_type
         return GroupVariable(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> pulumi.Output[Optional[str]]:
@@ -462,14 +499,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> pulumi.Output[str]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/instance_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 @pulumi.input_type
 class InstanceVariableArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a InstanceVariable resource.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
@@ -81,14 +85,26 @@
         return pulumi.get(self, "protected")
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
+    @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         return pulumi.get(self, "variable_type")
 
@@ -99,30 +115,34 @@
 
 @pulumi.input_type
 class _InstanceVariableState:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering InstanceVariable resources.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if value is not None:
             pulumi.set(__self__, "value", value)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter
@@ -158,14 +178,26 @@
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
     @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
+    @pulumi.getter
     def value(self) -> Optional[pulumi.Input[str]]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @value.setter
@@ -189,14 +221,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `InstanceVariable` resource allows to manage the lifecycle of an instance-level CI/CD variable.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/instance_level_ci_variables.html)
@@ -223,14 +256,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -276,14 +310,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -292,55 +327,57 @@
             __props__ = InstanceVariableArgs.__new__(InstanceVariableArgs)
 
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["masked"] = masked
             __props__.__dict__["protected"] = protected
+            __props__.__dict__["raw"] = raw
             if value is None and not opts.urn:
                 raise TypeError("Missing required property 'value'")
-            __props__.__dict__["value"] = None if value is None else pulumi.Output.secret(value)
+            __props__.__dict__["value"] = value
             __props__.__dict__["variable_type"] = variable_type
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["value"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(InstanceVariable, __self__).__init__(
             'gitlab:index/instanceVariable:InstanceVariable',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             key: Optional[pulumi.Input[str]] = None,
             masked: Optional[pulumi.Input[bool]] = None,
             protected: Optional[pulumi.Input[bool]] = None,
+            raw: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None,
             variable_type: Optional[pulumi.Input[str]] = None) -> 'InstanceVariable':
         """
         Get an existing InstanceVariable resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstanceVariableState.__new__(_InstanceVariableState)
 
         __props__.__dict__["key"] = key
         __props__.__dict__["masked"] = masked
         __props__.__dict__["protected"] = protected
+        __props__.__dict__["raw"] = raw
         __props__.__dict__["value"] = value
         __props__.__dict__["variable_type"] = variable_type
         return InstanceVariable(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
@@ -363,14 +400,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> pulumi.Output[str]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/label.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,27 +82,31 @@
 
 
 @pulumi.input_type
 class _LabelState:
     def __init__(__self__, *,
                  color: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 label_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Label resources.
         :param pulumi.Input[str] color: The color of the label given in 6-digit hex notation with leading '#' sign (e.g. #FFAABB) or one of the [CSS color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords).
         :param pulumi.Input[str] description: The description of the label.
+        :param pulumi.Input[int] label_id: The id of the project label.
         :param pulumi.Input[str] name: The name of the label.
         :param pulumi.Input[str] project: The name or id of the project to add the label to.
         """
         if color is not None:
             pulumi.set(__self__, "color", color)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if label_id is not None:
+            pulumi.set(__self__, "label_id", label_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
 
     @property
     @pulumi.getter
@@ -125,14 +129,26 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="labelId")
+    def label_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the project label.
+        """
+        return pulumi.get(self, "label_id")
+
+    @label_id.setter
+    def label_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "label_id", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the label.
         """
         return pulumi.get(self, "name")
 
@@ -162,40 +178,17 @@
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `Label` resource allows to manage the lifecycle of a project label.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/labels.html#project-labels)
-
-        ## Example Usage
+        > This resource is deprecated. use `ProjectLabel`instead!
 
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        fixme = gitlab.Label("fixme",
-            project="example",
-            description="issue with failing tests",
-            color="#ffcc00")
-        # Scoped label
-        devops_create = gitlab.Label("devopsCreate",
-            project=gitlab_project["example"]["id"],
-            description="issue for creating infrastructure resources",
-            color="#ffa500")
-        ```
-
-        ## Import
-
-        Gitlab labels can be imported using an id made up of `{project_id}:{group_label_id}`, e.g.
-
-        ```sh
-         $ pulumi import gitlab:index/label:Label example 12345:fixme
-        ```
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/labels.html#project-labels)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] color: The color of the label given in 6-digit hex notation with leading '#' sign (e.g. #FFAABB) or one of the [CSS color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords).
         :param pulumi.Input[str] description: The description of the label.
         :param pulumi.Input[str] name: The name of the label.
         :param pulumi.Input[str] project: The name or id of the project to add the label to.
@@ -205,40 +198,17 @@
     def __init__(__self__,
                  resource_name: str,
                  args: LabelArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `Label` resource allows to manage the lifecycle of a project label.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/labels.html#project-labels)
-
-        ## Example Usage
+        > This resource is deprecated. use `ProjectLabel`instead!
 
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        fixme = gitlab.Label("fixme",
-            project="example",
-            description="issue with failing tests",
-            color="#ffcc00")
-        # Scoped label
-        devops_create = gitlab.Label("devopsCreate",
-            project=gitlab_project["example"]["id"],
-            description="issue for creating infrastructure resources",
-            color="#ffa500")
-        ```
-
-        ## Import
-
-        Gitlab labels can be imported using an id made up of `{project_id}:{group_label_id}`, e.g.
-
-        ```sh
-         $ pulumi import gitlab:index/label:Label example 12345:fixme
-        ```
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/labels.html#project-labels)
 
         :param str resource_name: The name of the resource.
         :param LabelArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -268,46 +238,50 @@
                 raise TypeError("Missing required property 'color'")
             __props__.__dict__["color"] = color
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
+            __props__.__dict__["label_id"] = None
         super(Label, __self__).__init__(
             'gitlab:index/label:Label',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             color: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
+            label_id: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None) -> 'Label':
         """
         Get an existing Label resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] color: The color of the label given in 6-digit hex notation with leading '#' sign (e.g. #FFAABB) or one of the [CSS color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords).
         :param pulumi.Input[str] description: The description of the label.
+        :param pulumi.Input[int] label_id: The id of the project label.
         :param pulumi.Input[str] name: The name of the label.
         :param pulumi.Input[str] project: The name or id of the project to add the label to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LabelState.__new__(_LabelState)
 
         __props__.__dict__["color"] = color
         __props__.__dict__["description"] = description
+        __props__.__dict__["label_id"] = label_id
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
         return Label(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def color(self) -> pulumi.Output[str]:
@@ -321,14 +295,22 @@
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         The description of the label.
         """
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="labelId")
+    def label_id(self) -> pulumi.Output[int]:
+        """
+        The id of the project label.
+        """
+        return pulumi.get(self, "label_id")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the label.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/managed_license.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_gpg_key.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,303 +5,319 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ManagedLicenseArgs', 'ManagedLicense']
+__all__ = ['UserGpgKeyArgs', 'UserGpgKey']
 
 @pulumi.input_type
-class ManagedLicenseArgs:
+class UserGpgKeyArgs:
     def __init__(__self__, *,
-                 approval_status: pulumi.Input[str],
-                 project: pulumi.Input[str],
-                 name: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a ManagedLicense resource.
-        :param pulumi.Input[str] approval_status: The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-               			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-               			Prior to version 15.0 and after 14.6, the values are equivalent.
-        :param pulumi.Input[str] project: The ID of the project under which the managed license will be created.
-        :param pulumi.Input[str] name: The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
-        """
-        pulumi.set(__self__, "approval_status", approval_status)
-        pulumi.set(__self__, "project", project)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter(name="approvalStatus")
-    def approval_status(self) -> pulumi.Input[str]:
+                 key: pulumi.Input[str],
+                 user_id: Optional[pulumi.Input[int]] = None):
         """
-        The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-        			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-        			Prior to version 15.0 and after 14.6, the values are equivalent.
-        """
-        return pulumi.get(self, "approval_status")
-
-    @approval_status.setter
-    def approval_status(self, value: pulumi.Input[str]):
-        pulumi.set(self, "approval_status", value)
+        The set of arguments for constructing a UserGpgKey resource.
+        :param pulumi.Input[str] key: The armored GPG public key.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        """
+        pulumi.set(__self__, "key", key)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Input[str]:
+    def key(self) -> pulumi.Input[str]:
         """
-        The ID of the project under which the managed license will be created.
+        The armored GPG public key.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "key")
 
-    @project.setter
-    def project(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project", value)
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "user_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "user_id", value)
 
 
 @pulumi.input_type
-class _ManagedLicenseState:
+class _UserGpgKeyState:
     def __init__(__self__, *,
-                 approval_status: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ManagedLicense resources.
-        :param pulumi.Input[str] approval_status: The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-               			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-               			Prior to version 15.0 and after 14.6, the values are equivalent.
-        :param pulumi.Input[str] name: The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
-        :param pulumi.Input[str] project: The ID of the project under which the managed license will be created.
-        """
-        if approval_status is not None:
-            pulumi.set(__self__, "approval_status", approval_status)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if project is not None:
-            pulumi.set(__self__, "project", project)
+                 created_at: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 key_id: Optional[pulumi.Input[int]] = None,
+                 user_id: Optional[pulumi.Input[int]] = None):
+        """
+        Input properties used for looking up and filtering UserGpgKey resources.
+        :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
+        :param pulumi.Input[str] key: The armored GPG public key.
+        :param pulumi.Input[int] key_id: The ID of the GPG key.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        """
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
+        if key_id is not None:
+            pulumi.set(__self__, "key_id", key_id)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
-    @pulumi.getter(name="approvalStatus")
-    def approval_status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The time when this key was created in GitLab.
         """
-        The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-        			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-        			Prior to version 15.0 and after 14.6, the values are equivalent.
-        """
-        return pulumi.get(self, "approval_status")
-
-    @approval_status.setter
-    def approval_status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "approval_status", value)
+        return pulumi.get(self, "created_at")
+
+    @created_at.setter
+    def created_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def key(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
+        The armored GPG public key.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "key")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
 
     @property
-    @pulumi.getter
-    def project(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="keyId")
+    def key_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of the GPG key.
         """
-        The ID of the project under which the managed license will be created.
+        return pulumi.get(self, "key_id")
+
+    @key_id.setter
+    def key_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "key_id", value)
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "user_id")
 
-    @project.setter
-    def project(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project", value)
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "user_id", value)
 
 
-class ManagedLicense(pulumi.CustomResource):
+class UserGpgKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 approval_status: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        The `ManagedLicense` resource allows to manage the lifecycle of a managed license.
+        The `UserGpgKey` resource allows to manage the lifecycle of a GPG key assigned to the current user or a specific user.
 
-        > This resource requires a GitLab Enterprise instance.
+        > Managing GPG keys for arbitrary users requires admin privileges.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/managed_licenses.html)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html#get-a-specific-gpg-key)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Project("foo",
-            description="Lorem Ipsum",
-            visibility_level="public")
-        mit = gitlab.ManagedLicense("mit",
-            project=foo.id,
-            approval_status="allowed")
+        example_user = gitlab.get_user(username="example-user")
+        # Manages a GPG key for the specified user. An admin token is required if `user_id` is specified.
+        example_user_gpg_key = gitlab.UserGpgKey("exampleUserGpgKey",
+            user_id=example_user.id,
+            key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
+        ...
+        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
+        # Manages a GPG key for the current user
+        example_user_user_gpg_key = gitlab.UserGpgKey("exampleUserUserGpgKey", key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
+        ...
+        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
         ```
 
         ## Import
 
-        You can import this resource with an id made up of `{project-id}:{license-id}`, e.g.
+        You can import a GPG key for a specific user using an id made up of `{user-id}:{key}`, e.g.
+
+        ```sh
+         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example 42:1
+        ```
+
+         Alternatively, you can import a GPG key for the current user using an id made up of `{key}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/managedLicense:ManagedLicense foo 1:2
+         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example_user 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] approval_status: The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-               			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-               			Prior to version 15.0 and after 14.6, the values are equivalent.
-        :param pulumi.Input[str] name: The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
-        :param pulumi.Input[str] project: The ID of the project under which the managed license will be created.
+        :param pulumi.Input[str] key: The armored GPG public key.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ManagedLicenseArgs,
+                 args: UserGpgKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ManagedLicense` resource allows to manage the lifecycle of a managed license.
+        The `UserGpgKey` resource allows to manage the lifecycle of a GPG key assigned to the current user or a specific user.
 
-        > This resource requires a GitLab Enterprise instance.
+        > Managing GPG keys for arbitrary users requires admin privileges.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/managed_licenses.html)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html#get-a-specific-gpg-key)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Project("foo",
-            description="Lorem Ipsum",
-            visibility_level="public")
-        mit = gitlab.ManagedLicense("mit",
-            project=foo.id,
-            approval_status="allowed")
+        example_user = gitlab.get_user(username="example-user")
+        # Manages a GPG key for the specified user. An admin token is required if `user_id` is specified.
+        example_user_gpg_key = gitlab.UserGpgKey("exampleUserGpgKey",
+            user_id=example_user.id,
+            key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
+        ...
+        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
+        # Manages a GPG key for the current user
+        example_user_user_gpg_key = gitlab.UserGpgKey("exampleUserUserGpgKey", key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
+        ...
+        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
         ```
 
         ## Import
 
-        You can import this resource with an id made up of `{project-id}:{license-id}`, e.g.
+        You can import a GPG key for a specific user using an id made up of `{user-id}:{key}`, e.g.
+
+        ```sh
+         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example 42:1
+        ```
+
+         Alternatively, you can import a GPG key for the current user using an id made up of `{key}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/managedLicense:ManagedLicense foo 1:2
+         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example_user 1
         ```
 
         :param str resource_name: The name of the resource.
-        :param ManagedLicenseArgs args: The arguments to use to populate this resource's properties.
+        :param UserGpgKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ManagedLicenseArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserGpgKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 approval_status: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ManagedLicenseArgs.__new__(ManagedLicenseArgs)
+            __props__ = UserGpgKeyArgs.__new__(UserGpgKeyArgs)
 
-            if approval_status is None and not opts.urn:
-                raise TypeError("Missing required property 'approval_status'")
-            __props__.__dict__["approval_status"] = approval_status
-            __props__.__dict__["name"] = name
-            if project is None and not opts.urn:
-                raise TypeError("Missing required property 'project'")
-            __props__.__dict__["project"] = project
-        super(ManagedLicense, __self__).__init__(
-            'gitlab:index/managedLicense:ManagedLicense',
+            if key is None and not opts.urn:
+                raise TypeError("Missing required property 'key'")
+            __props__.__dict__["key"] = key
+            __props__.__dict__["user_id"] = user_id
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["key_id"] = None
+        super(UserGpgKey, __self__).__init__(
+            'gitlab:index/userGpgKey:UserGpgKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            approval_status: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            project: Optional[pulumi.Input[str]] = None) -> 'ManagedLicense':
+            created_at: Optional[pulumi.Input[str]] = None,
+            key: Optional[pulumi.Input[str]] = None,
+            key_id: Optional[pulumi.Input[int]] = None,
+            user_id: Optional[pulumi.Input[int]] = None) -> 'UserGpgKey':
         """
-        Get an existing ManagedLicense resource's state with the given name, id, and optional extra
+        Get an existing UserGpgKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] approval_status: The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-               			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-               			Prior to version 15.0 and after 14.6, the values are equivalent.
-        :param pulumi.Input[str] name: The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
-        :param pulumi.Input[str] project: The ID of the project under which the managed license will be created.
+        :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
+        :param pulumi.Input[str] key: The armored GPG public key.
+        :param pulumi.Input[int] key_id: The ID of the GPG key.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ManagedLicenseState.__new__(_ManagedLicenseState)
+        __props__ = _UserGpgKeyState.__new__(_UserGpgKeyState)
 
-        __props__.__dict__["approval_status"] = approval_status
-        __props__.__dict__["name"] = name
-        __props__.__dict__["project"] = project
-        return ManagedLicense(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["key"] = key
+        __props__.__dict__["key_id"] = key_id
+        __props__.__dict__["user_id"] = user_id
+        return UserGpgKey(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="approvalStatus")
-    def approval_status(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[str]:
         """
-        The approval status of the license. Valid values are: `approved`, `blacklisted`, `allowed`, `denied`. "approved" and "blacklisted"
-        			have been deprecated in favor of "allowed" and "denied"; use "allowed" and "denied" for GitLab versions 15.0 and higher.
-        			Prior to version 15.0 and after 14.6, the values are equivalent.
+        The time when this key was created in GitLab.
         """
-        return pulumi.get(self, "approval_status")
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def key(self) -> pulumi.Output[str]:
         """
-        The name of the managed license (I.e., 'Apache License 2.0' or 'MIT license')
+        The armored GPG public key.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "key")
 
     @property
-    @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="keyId")
+    def key_id(self) -> pulumi.Output[int]:
+        """
+        The ID of the GPG key.
+        """
+        return pulumi.get(self, "key_id")
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[Optional[int]]:
         """
-        The ID of the project under which the managed license will be created.
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "user_id")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/outputs.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1677,25 +1677,27 @@
 class GetGroupVariablesVariableResult(dict):
     def __init__(__self__, *,
                  environment_scope: str,
                  group: str,
                  key: str,
                  masked: bool,
                  protected: bool,
+                 raw: bool,
                  value: str,
                  variable_type: str):
         """
         :param str environment_scope: The environment scope of the variable. Defaults to all environment (`*`).
         :param str group: The name or id of the group.
         """
         pulumi.set(__self__, "environment_scope", environment_scope)
         pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "masked", masked)
         pulumi.set(__self__, "protected", protected)
+        pulumi.set(__self__, "raw", raw)
         pulumi.set(__self__, "value", value)
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
@@ -1724,14 +1726,19 @@
     @property
     @pulumi.getter
     def protected(self) -> bool:
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> str:
         return pulumi.get(self, "variable_type")
@@ -1955,19 +1962,21 @@
 
 @pulumi.output_type
 class GetInstanceVariablesVariableResult(dict):
     def __init__(__self__, *,
                  key: str,
                  masked: bool,
                  protected: bool,
+                 raw: bool,
                  value: str,
                  variable_type: str):
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "masked", masked)
         pulumi.set(__self__, "protected", protected)
+        pulumi.set(__self__, "raw", raw)
         pulumi.set(__self__, "value", value)
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         return pulumi.get(self, "key")
@@ -1980,14 +1989,19 @@
     @property
     @pulumi.getter
     def protected(self) -> bool:
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> str:
         return pulumi.get(self, "variable_type")
@@ -3453,25 +3467,27 @@
 class GetProjectVariablesVariableResult(dict):
     def __init__(__self__, *,
                  environment_scope: str,
                  key: str,
                  masked: bool,
                  project: str,
                  protected: bool,
+                 raw: bool,
                  value: str,
                  variable_type: str):
         """
         :param str environment_scope: The environment scope of the variable. Defaults to all environment (`*`).
         :param str project: The name or id of the project.
         """
         pulumi.set(__self__, "environment_scope", environment_scope)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "masked", masked)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "protected", protected)
+        pulumi.set(__self__, "raw", raw)
         pulumi.set(__self__, "value", value)
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
@@ -3500,14 +3516,19 @@
     @property
     @pulumi.getter
     def protected(self) -> bool:
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> bool:
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> str:
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> str:
         return pulumi.get(self, "variable_type")
@@ -3574,15 +3595,14 @@
                  name: str,
                  name_with_namespace: str,
                  namespaces: Sequence['outputs.GetProjectsProjectNamespaceResult'],
                  only_allow_merge_if_all_discussions_are_resolved: bool,
                  only_allow_merge_if_pipeline_succeeds: bool,
                  only_mirror_protected_branches: bool,
                  open_issues_count: int,
-                 operations_access_level: str,
                  owners: Sequence['outputs.GetProjectsProjectOwnerResult'],
                  packages_enabled: bool,
                  path: str,
                  path_with_namespace: str,
                  permissions: Sequence['outputs.GetProjectsProjectPermissionResult'],
                  public: bool,
                  public_builds: bool,
@@ -3675,15 +3695,14 @@
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "name_with_namespace", name_with_namespace)
         pulumi.set(__self__, "namespaces", namespaces)
         pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         pulumi.set(__self__, "only_allow_merge_if_pipeline_succeeds", only_allow_merge_if_pipeline_succeeds)
         pulumi.set(__self__, "only_mirror_protected_branches", only_mirror_protected_branches)
         pulumi.set(__self__, "open_issues_count", open_issues_count)
-        pulumi.set(__self__, "operations_access_level", operations_access_level)
         pulumi.set(__self__, "owners", owners)
         pulumi.set(__self__, "packages_enabled", packages_enabled)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "path_with_namespace", path_with_namespace)
         pulumi.set(__self__, "permissions", permissions)
         pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "public_builds", public_builds)
@@ -4026,19 +4045,14 @@
 
     @property
     @pulumi.getter(name="openIssuesCount")
     def open_issues_count(self) -> int:
         return pulumi.get(self, "open_issues_count")
 
     @property
-    @pulumi.getter(name="operationsAccessLevel")
-    def operations_access_level(self) -> str:
-        return pulumi.get(self, "operations_access_level")
-
-    @property
     @pulumi.getter
     def owners(self) -> Sequence['outputs.GetProjectsProjectOwnerResult']:
         return pulumi.get(self, "owners")
 
     @property
     @pulumi.getter(name="packagesEnabled")
     def packages_enabled(self) -> bool:
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pages_domain.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pages_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/personal_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  user_id: pulumi.Input[int],
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PersonalAccessToken resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[int] user_id: The id of the user.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] name: The name of the personal access token.
         """
         pulumi.set(__self__, "scopes", scopes)
         pulumi.set(__self__, "user_id", user_id)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
         if name is not None:
@@ -56,15 +56,15 @@
     def user_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "user_id", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -92,15 +92,15 @@
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering PersonalAccessToken resources.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] name: The name of the personal access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[str] token: The personal access token. This is only populated when creating a new personal access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         if active is not None:
@@ -144,15 +144,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -258,15 +258,15 @@
          $ pulumi import gitlab:index/personalAccessToken:PersonalAccessToken example "12345:1"
         ```
 
          NOTEthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] name: The name of the personal access token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         ...
     @overload
     def __init__(__self__,
@@ -371,15 +371,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         :param pulumi.Input[str] name: The name of the personal access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[str] token: The personal access token. This is only populated when creating a new personal access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -410,17 +410,17 @@
         """
         Time the token has been created, RFC3339 format.
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> pulumi.Output[Optional[str]]:
+    def expires_at(self) -> pulumi.Output[str]:
         """
-        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
+        The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD.
         """
         return pulumi.get(self, "expires_at")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,33 +114,37 @@
 @pulumi.input_type
 class _PipelineScheduleState:
     def __init__(__self__, *,
                  active: Optional[pulumi.Input[bool]] = None,
                  cron: Optional[pulumi.Input[str]] = None,
                  cron_timezone: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 pipeline_schedule_id: Optional[pulumi.Input[int]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  ref: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PipelineSchedule resources.
         :param pulumi.Input[bool] active: The activation of pipeline schedule. If false is set, the pipeline schedule will deactivated initially.
         :param pulumi.Input[str] cron: The cron (e.g. `0 1 * * *`).
         :param pulumi.Input[str] cron_timezone: The timezone.
         :param pulumi.Input[str] description: The description of the pipeline schedule.
+        :param pulumi.Input[int] pipeline_schedule_id: The pipeline schedule id.
         :param pulumi.Input[str] project: The name or id of the project to add the schedule to.
         :param pulumi.Input[str] ref: The branch/tag name to be triggered.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if cron is not None:
             pulumi.set(__self__, "cron", cron)
         if cron_timezone is not None:
             pulumi.set(__self__, "cron_timezone", cron_timezone)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if pipeline_schedule_id is not None:
+            pulumi.set(__self__, "pipeline_schedule_id", pipeline_schedule_id)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if ref is not None:
             pulumi.set(__self__, "ref", ref)
 
     @property
     @pulumi.getter
@@ -187,14 +191,26 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="pipelineScheduleId")
+    def pipeline_schedule_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The pipeline schedule id.
+        """
+        return pulumi.get(self, "pipeline_schedule_id")
+
+    @pipeline_schedule_id.setter
+    def pipeline_schedule_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "pipeline_schedule_id", value)
+
+    @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
         The name or id of the project to add the schedule to.
         """
         return pulumi.get(self, "project")
 
@@ -334,52 +350,56 @@
             __props__.__dict__["description"] = description
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if ref is None and not opts.urn:
                 raise TypeError("Missing required property 'ref'")
             __props__.__dict__["ref"] = ref
+            __props__.__dict__["pipeline_schedule_id"] = None
         super(PipelineSchedule, __self__).__init__(
             'gitlab:index/pipelineSchedule:PipelineSchedule',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             active: Optional[pulumi.Input[bool]] = None,
             cron: Optional[pulumi.Input[str]] = None,
             cron_timezone: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
+            pipeline_schedule_id: Optional[pulumi.Input[int]] = None,
             project: Optional[pulumi.Input[str]] = None,
             ref: Optional[pulumi.Input[str]] = None) -> 'PipelineSchedule':
         """
         Get an existing PipelineSchedule resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: The activation of pipeline schedule. If false is set, the pipeline schedule will deactivated initially.
         :param pulumi.Input[str] cron: The cron (e.g. `0 1 * * *`).
         :param pulumi.Input[str] cron_timezone: The timezone.
         :param pulumi.Input[str] description: The description of the pipeline schedule.
+        :param pulumi.Input[int] pipeline_schedule_id: The pipeline schedule id.
         :param pulumi.Input[str] project: The name or id of the project to add the schedule to.
         :param pulumi.Input[str] ref: The branch/tag name to be triggered.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PipelineScheduleState.__new__(_PipelineScheduleState)
 
         __props__.__dict__["active"] = active
         __props__.__dict__["cron"] = cron
         __props__.__dict__["cron_timezone"] = cron_timezone
         __props__.__dict__["description"] = description
+        __props__.__dict__["pipeline_schedule_id"] = pipeline_schedule_id
         __props__.__dict__["project"] = project
         __props__.__dict__["ref"] = ref
         return PipelineSchedule(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[Optional[bool]]:
@@ -409,14 +429,22 @@
     def description(self) -> pulumi.Output[str]:
         """
         The description of the pipeline schedule.
         """
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="pipelineScheduleId")
+    def pipeline_schedule_id(self) -> pulumi.Output[int]:
+        """
+        The pipeline schedule id.
+        """
+        return pulumi.get(self, "pipeline_schedule_id")
+
+    @property
     @pulumi.getter
     def project(self) -> pulumi.Output[str]:
         """
         The name or id of the project to add the schedule to.
         """
         return pulumi.get(self, "project")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/pipeline_trigger.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,24 +49,28 @@
         pulumi.set(self, "project", value)
 
 
 @pulumi.input_type
 class _PipelineTriggerState:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
+                 pipeline_trigger_id: Optional[pulumi.Input[int]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PipelineTrigger resources.
         :param pulumi.Input[str] description: The description of the pipeline trigger.
+        :param pulumi.Input[int] pipeline_trigger_id: The pipeline trigger id.
         :param pulumi.Input[str] project: The name or id of the project to add the trigger to.
         :param pulumi.Input[str] token: The pipeline trigger token.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if pipeline_trigger_id is not None:
+            pulumi.set(__self__, "pipeline_trigger_id", pipeline_trigger_id)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -77,14 +81,26 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="pipelineTriggerId")
+    def pipeline_trigger_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The pipeline trigger id.
+        """
+        return pulumi.get(self, "pipeline_trigger_id")
+
+    @pipeline_trigger_id.setter
+    def pipeline_trigger_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "pipeline_trigger_id", value)
+
+    @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
         The name or id of the project to add the trigger to.
         """
         return pulumi.get(self, "project")
 
@@ -200,59 +216,71 @@
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
             __props__.__dict__["description"] = description
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
+            __props__.__dict__["pipeline_trigger_id"] = None
             __props__.__dict__["token"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["token"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(PipelineTrigger, __self__).__init__(
             'gitlab:index/pipelineTrigger:PipelineTrigger',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             description: Optional[pulumi.Input[str]] = None,
+            pipeline_trigger_id: Optional[pulumi.Input[int]] = None,
             project: Optional[pulumi.Input[str]] = None,
             token: Optional[pulumi.Input[str]] = None) -> 'PipelineTrigger':
         """
         Get an existing PipelineTrigger resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: The description of the pipeline trigger.
+        :param pulumi.Input[int] pipeline_trigger_id: The pipeline trigger id.
         :param pulumi.Input[str] project: The name or id of the project to add the trigger to.
         :param pulumi.Input[str] token: The pipeline trigger token.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PipelineTriggerState.__new__(_PipelineTriggerState)
 
         __props__.__dict__["description"] = description
+        __props__.__dict__["pipeline_trigger_id"] = pipeline_trigger_id
         __props__.__dict__["project"] = project
         __props__.__dict__["token"] = token
         return PipelineTrigger(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[str]:
         """
         The description of the pipeline trigger.
         """
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="pipelineTriggerId")
+    def pipeline_trigger_id(self) -> pulumi.Output[int]:
+        """
+        The pipeline trigger id.
+        """
+        return pulumi.get(self, "pipeline_trigger_id")
+
+    @property
     @pulumi.getter
     def project(self) -> pulumi.Output[str]:
         """
         The name or id of the project to add the trigger to.
         """
         return pulumi.get(self, "project")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
                  monitor_access_level: Optional[pulumi.Input[str]] = None,
                  mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
-                 operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input['ProjectPushRulesArgs']] = None,
@@ -173,15 +172,14 @@
         :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
-        :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input['ProjectPushRulesArgs'] push_rules: Push rules for the project.
@@ -332,16 +330,14 @@
             pulumi.set(__self__, "namespace_id", namespace_id)
         if only_allow_merge_if_all_discussions_are_resolved is not None:
             pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         if only_allow_merge_if_pipeline_succeeds is not None:
             pulumi.set(__self__, "only_allow_merge_if_pipeline_succeeds", only_allow_merge_if_pipeline_succeeds)
         if only_mirror_protected_branches is not None:
             pulumi.set(__self__, "only_mirror_protected_branches", only_mirror_protected_branches)
-        if operations_access_level is not None:
-            pulumi.set(__self__, "operations_access_level", operations_access_level)
         if packages_enabled is not None:
             pulumi.set(__self__, "packages_enabled", packages_enabled)
         if pages_access_level is not None:
             pulumi.set(__self__, "pages_access_level", pages_access_level)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if pipelines_enabled is not None:
@@ -1108,26 +1104,14 @@
         return pulumi.get(self, "only_mirror_protected_branches")
 
     @only_mirror_protected_branches.setter
     def only_mirror_protected_branches(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "only_mirror_protected_branches", value)
 
     @property
-    @pulumi.getter(name="operationsAccessLevel")
-    def operations_access_level(self) -> Optional[pulumi.Input[str]]:
-        """
-        Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
-        """
-        return pulumi.get(self, "operations_access_level")
-
-    @operations_access_level.setter
-    def operations_access_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "operations_access_level", value)
-
-    @property
     @pulumi.getter(name="packagesEnabled")
     def packages_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable packages repository for the project.
         """
         return pulumi.get(self, "packages_enabled")
 
@@ -1559,15 +1543,14 @@
                  monitor_access_level: Optional[pulumi.Input[str]] = None,
                  mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
-                 operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  path_with_namespace: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
@@ -1668,15 +1651,14 @@
         :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
-        :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[str] path_with_namespace: The path of the repository with namespace.
         :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
@@ -1835,16 +1817,14 @@
             pulumi.set(__self__, "namespace_id", namespace_id)
         if only_allow_merge_if_all_discussions_are_resolved is not None:
             pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         if only_allow_merge_if_pipeline_succeeds is not None:
             pulumi.set(__self__, "only_allow_merge_if_pipeline_succeeds", only_allow_merge_if_pipeline_succeeds)
         if only_mirror_protected_branches is not None:
             pulumi.set(__self__, "only_mirror_protected_branches", only_mirror_protected_branches)
-        if operations_access_level is not None:
-            pulumi.set(__self__, "operations_access_level", operations_access_level)
         if packages_enabled is not None:
             pulumi.set(__self__, "packages_enabled", packages_enabled)
         if pages_access_level is not None:
             pulumi.set(__self__, "pages_access_level", pages_access_level)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if path_with_namespace is not None:
@@ -2643,26 +2623,14 @@
         return pulumi.get(self, "only_mirror_protected_branches")
 
     @only_mirror_protected_branches.setter
     def only_mirror_protected_branches(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "only_mirror_protected_branches", value)
 
     @property
-    @pulumi.getter(name="operationsAccessLevel")
-    def operations_access_level(self) -> Optional[pulumi.Input[str]]:
-        """
-        Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
-        """
-        return pulumi.get(self, "operations_access_level")
-
-    @operations_access_level.setter
-    def operations_access_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "operations_access_level", value)
-
-    @property
     @pulumi.getter(name="packagesEnabled")
     def packages_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable packages repository for the project.
         """
         return pulumi.get(self, "packages_enabled")
 
@@ -3142,15 +3110,14 @@
                  monitor_access_level: Optional[pulumi.Input[str]] = None,
                  mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
-                 operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']]] = None,
@@ -3314,15 +3281,14 @@
         :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
-        :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']] push_rules: Push rules for the project.
@@ -3498,15 +3464,14 @@
                  monitor_access_level: Optional[pulumi.Input[str]] = None,
                  mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
-                 operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']]] = None,
@@ -3603,15 +3568,14 @@
             __props__.__dict__["monitor_access_level"] = monitor_access_level
             __props__.__dict__["mr_default_target_self"] = mr_default_target_self
             __props__.__dict__["name"] = name
             __props__.__dict__["namespace_id"] = namespace_id
             __props__.__dict__["only_allow_merge_if_all_discussions_are_resolved"] = only_allow_merge_if_all_discussions_are_resolved
             __props__.__dict__["only_allow_merge_if_pipeline_succeeds"] = only_allow_merge_if_pipeline_succeeds
             __props__.__dict__["only_mirror_protected_branches"] = only_mirror_protected_branches
-            __props__.__dict__["operations_access_level"] = operations_access_level
             __props__.__dict__["packages_enabled"] = packages_enabled
             __props__.__dict__["pages_access_level"] = pages_access_level
             __props__.__dict__["path"] = path
             if pipelines_enabled is not None and not opts.urn:
                 warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
                 pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
             __props__.__dict__["pipelines_enabled"] = pipelines_enabled
@@ -3716,15 +3680,14 @@
             monitor_access_level: Optional[pulumi.Input[str]] = None,
             mr_default_target_self: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace_id: Optional[pulumi.Input[int]] = None,
             only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
             only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
             only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
-            operations_access_level: Optional[pulumi.Input[str]] = None,
             packages_enabled: Optional[pulumi.Input[bool]] = None,
             pages_access_level: Optional[pulumi.Input[str]] = None,
             path: Optional[pulumi.Input[str]] = None,
             path_with_namespace: Optional[pulumi.Input[str]] = None,
             pipelines_enabled: Optional[pulumi.Input[bool]] = None,
             printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
             public_builds: Optional[pulumi.Input[bool]] = None,
@@ -3830,15 +3793,14 @@
         :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
-        :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[str] path_with_namespace: The path of the repository with namespace.
         :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
@@ -3935,15 +3897,14 @@
         __props__.__dict__["monitor_access_level"] = monitor_access_level
         __props__.__dict__["mr_default_target_self"] = mr_default_target_self
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace_id"] = namespace_id
         __props__.__dict__["only_allow_merge_if_all_discussions_are_resolved"] = only_allow_merge_if_all_discussions_are_resolved
         __props__.__dict__["only_allow_merge_if_pipeline_succeeds"] = only_allow_merge_if_pipeline_succeeds
         __props__.__dict__["only_mirror_protected_branches"] = only_mirror_protected_branches
-        __props__.__dict__["operations_access_level"] = operations_access_level
         __props__.__dict__["packages_enabled"] = packages_enabled
         __props__.__dict__["pages_access_level"] = pages_access_level
         __props__.__dict__["path"] = path
         __props__.__dict__["path_with_namespace"] = path_with_namespace
         __props__.__dict__["pipelines_enabled"] = pipelines_enabled
         __props__.__dict__["printing_merge_request_link_enabled"] = printing_merge_request_link_enabled
         __props__.__dict__["public_builds"] = public_builds
@@ -4465,22 +4426,14 @@
     def only_mirror_protected_branches(self) -> pulumi.Output[bool]:
         """
         Enable only mirror protected branches for a mirrored project.
         """
         return pulumi.get(self, "only_mirror_protected_branches")
 
     @property
-    @pulumi.getter(name="operationsAccessLevel")
-    def operations_access_level(self) -> pulumi.Output[str]:
-        """
-        Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
-        """
-        return pulumi.get(self, "operations_access_level")
-
-    @property
     @pulumi.getter(name="packagesEnabled")
     def packages_enabled(self) -> pulumi.Output[bool]:
         """
         Enable packages repository for the project.
         """
         return pulumi.get(self, "packages_enabled")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_access_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectAccessToken resource.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
-        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format.
         :param pulumi.Input[str] name: A name to describe the project access token.
         """
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "scopes", scopes)
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if expires_at is not None:
@@ -72,15 +72,15 @@
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        Time the token will expire it, YYYY-MM-DD format.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -111,15 +111,15 @@
                  token: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering ProjectAccessToken resources.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] token: The secret token. **Note**: the token is not available for imported resources.
         :param pulumi.Input[int] user_id: The user_id associated to the token.
         """
@@ -180,15 +180,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="expiresAt")
     def expires_at(self) -> Optional[pulumi.Input[str]]:
         """
-        Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        Time the token will expire it, YYYY-MM-DD format.
         """
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
@@ -307,15 +307,15 @@
         ```
 
          NOTEthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
-        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         """
         ...
     @overload
     def __init__(__self__,
@@ -425,15 +425,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
-        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] token: The secret token. **Note**: the token is not available for imported resources.
         :param pulumi.Input[int] user_id: The user_id associated to the token.
         """
@@ -475,17 +475,17 @@
         """
         Time the token has been created, RFC3339 format.
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> pulumi.Output[Optional[str]]:
+    def expires_at(self) -> pulumi.Output[str]:
         """
-        Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
+        Time the token will expire it, YYYY-MM-DD format.
         """
         return pulumi.get(self, "expires_at")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_approval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_freeze_period.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 __all__ = ['ProjectFreezePeriodArgs', 'ProjectFreezePeriod']
 
 @pulumi.input_type
 class ProjectFreezePeriodArgs:
     def __init__(__self__, *,
                  freeze_end: pulumi.Input[str],
                  freeze_start: pulumi.Input[str],
-                 project_id: pulumi.Input[str],
+                 project: pulumi.Input[str],
                  cron_timezone: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectFreezePeriod resource.
         :param pulumi.Input[str] freeze_end: End of the Freeze Period in cron format (e.g. `0 2 * * *`).
         :param pulumi.Input[str] freeze_start: Start of the Freeze Period in cron format (e.g. `0 1 * * *`).
-        :param pulumi.Input[str] project_id: The id of the project to add the schedule to.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project to add the schedule to.
         :param pulumi.Input[str] cron_timezone: The timezone.
         """
         pulumi.set(__self__, "freeze_end", freeze_end)
         pulumi.set(__self__, "freeze_start", freeze_start)
-        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "project", project)
         if cron_timezone is not None:
             pulumi.set(__self__, "cron_timezone", cron_timezone)
 
     @property
     @pulumi.getter(name="freezeEnd")
     def freeze_end(self) -> pulumi.Input[str]:
         """
@@ -52,24 +52,24 @@
         return pulumi.get(self, "freeze_start")
 
     @freeze_start.setter
     def freeze_start(self, value: pulumi.Input[str]):
         pulumi.set(self, "freeze_start", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The id of the project to add the schedule to.
+        The ID or URL-encoded path of the project to add the schedule to.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="cronTimezone")
     def cron_timezone(self) -> Optional[pulumi.Input[str]]:
         """
         The timezone.
         """
@@ -82,30 +82,30 @@
 
 @pulumi.input_type
 class _ProjectFreezePeriodState:
     def __init__(__self__, *,
                  cron_timezone: Optional[pulumi.Input[str]] = None,
                  freeze_end: Optional[pulumi.Input[str]] = None,
                  freeze_start: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None):
+                 project: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectFreezePeriod resources.
         :param pulumi.Input[str] cron_timezone: The timezone.
         :param pulumi.Input[str] freeze_end: End of the Freeze Period in cron format (e.g. `0 2 * * *`).
         :param pulumi.Input[str] freeze_start: Start of the Freeze Period in cron format (e.g. `0 1 * * *`).
-        :param pulumi.Input[str] project_id: The id of the project to add the schedule to.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project to add the schedule to.
         """
         if cron_timezone is not None:
             pulumi.set(__self__, "cron_timezone", cron_timezone)
         if freeze_end is not None:
             pulumi.set(__self__, "freeze_end", freeze_end)
         if freeze_start is not None:
             pulumi.set(__self__, "freeze_start", freeze_start)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
 
     @property
     @pulumi.getter(name="cronTimezone")
     def cron_timezone(self) -> Optional[pulumi.Input[str]]:
         """
         The timezone.
         """
@@ -136,49 +136,49 @@
         return pulumi.get(self, "freeze_start")
 
     @freeze_start.setter
     def freeze_start(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "freeze_start", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the project to add the schedule to.
+        The ID or URL-encoded path of the project to add the schedule to.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
 
 class ProjectFreezePeriod(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cron_timezone: Optional[pulumi.Input[str]] = None,
                  freeze_end: Optional[pulumi.Input[str]] = None,
                  freeze_start: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ProjectFreezePeriod` resource allows to manage the lifecycle of a freeze period for a project.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/freeze_periods.html)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         schedule = gitlab.ProjectFreezePeriod("schedule",
-            project_id=gitlab_project["foo"]["id"],
+            project=gitlab_project["foo"]["id"],
             freeze_start="0 23 * * 5",
             freeze_end="0 7 * * 1",
             cron_timezone="UTC")
         ```
 
         ## Import
 
@@ -189,15 +189,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cron_timezone: The timezone.
         :param pulumi.Input[str] freeze_end: End of the Freeze Period in cron format (e.g. `0 2 * * *`).
         :param pulumi.Input[str] freeze_start: Start of the Freeze Period in cron format (e.g. `0 1 * * *`).
-        :param pulumi.Input[str] project_id: The id of the project to add the schedule to.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project to add the schedule to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectFreezePeriodArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -209,15 +209,15 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         schedule = gitlab.ProjectFreezePeriod("schedule",
-            project_id=gitlab_project["foo"]["id"],
+            project=gitlab_project["foo"]["id"],
             freeze_start="0 23 * * 5",
             freeze_end="0 7 * * 1",
             cron_timezone="UTC")
         ```
 
         ## Import
 
@@ -241,15 +241,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cron_timezone: Optional[pulumi.Input[str]] = None,
                  freeze_end: Optional[pulumi.Input[str]] = None,
                  freeze_start: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -258,51 +258,51 @@
             __props__.__dict__["cron_timezone"] = cron_timezone
             if freeze_end is None and not opts.urn:
                 raise TypeError("Missing required property 'freeze_end'")
             __props__.__dict__["freeze_end"] = freeze_end
             if freeze_start is None and not opts.urn:
                 raise TypeError("Missing required property 'freeze_start'")
             __props__.__dict__["freeze_start"] = freeze_start
-            if project_id is None and not opts.urn:
-                raise TypeError("Missing required property 'project_id'")
-            __props__.__dict__["project_id"] = project_id
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
         super(ProjectFreezePeriod, __self__).__init__(
             'gitlab:index/projectFreezePeriod:ProjectFreezePeriod',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             cron_timezone: Optional[pulumi.Input[str]] = None,
             freeze_end: Optional[pulumi.Input[str]] = None,
             freeze_start: Optional[pulumi.Input[str]] = None,
-            project_id: Optional[pulumi.Input[str]] = None) -> 'ProjectFreezePeriod':
+            project: Optional[pulumi.Input[str]] = None) -> 'ProjectFreezePeriod':
         """
         Get an existing ProjectFreezePeriod resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cron_timezone: The timezone.
         :param pulumi.Input[str] freeze_end: End of the Freeze Period in cron format (e.g. `0 2 * * *`).
         :param pulumi.Input[str] freeze_start: Start of the Freeze Period in cron format (e.g. `0 1 * * *`).
-        :param pulumi.Input[str] project_id: The id of the project to add the schedule to.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project to add the schedule to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectFreezePeriodState.__new__(_ProjectFreezePeriodState)
 
         __props__.__dict__["cron_timezone"] = cron_timezone
         __props__.__dict__["freeze_end"] = freeze_end
         __props__.__dict__["freeze_start"] = freeze_start
-        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["project"] = project
         return ProjectFreezePeriod(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="cronTimezone")
     def cron_timezone(self) -> pulumi.Output[Optional[str]]:
         """
         The timezone.
@@ -322,14 +322,14 @@
     def freeze_start(self) -> pulumi.Output[str]:
         """
         Start of the Freeze Period in cron format (e.g. `0 1 * * *`).
         """
         return pulumi.get(self, "freeze_start")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        The id of the project to add the schedule to.
+        The ID or URL-encoded path of the project to add the schedule to.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_issue_board.py`

 * *Files 8% similar despite different names*

```diff
@@ -268,58 +268,14 @@
         """
         The `ProjectIssueBoard` resource allows to manage the lifecycle of a Project Issue Board.
 
         > **NOTE:** If the board lists are changed all lists will be recreated.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/boards.html)
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_project = gitlab.Project("exampleProject",
-            description="Lorem Ipsum",
-            visibility_level="public")
-        example_user = gitlab.User("exampleUser",
-            username="example",
-            email="example@example.com",
-            password="example1$$$")
-        example_project_membership = gitlab.ProjectMembership("exampleProjectMembership",
-            project_id=example_project.id,
-            user_id=example_user.id,
-            access_level="developer")
-        example_project_milestone = gitlab.ProjectMilestone("exampleProjectMilestone",
-            project=example_project.id,
-            title="m1")
-        this = gitlab.ProjectIssueBoard("this",
-            project=example_project.id,
-            lists=[
-                gitlab.ProjectIssueBoardListArgs(
-                    assignee_id=example_user.id,
-                ),
-                gitlab.ProjectIssueBoardListArgs(
-                    milestone_id=example_project_milestone.milestone_id,
-                ),
-            ],
-            opts=pulumi.ResourceOptions(depends_on=[example_project_membership]))
-        list_syntax = gitlab.ProjectIssueBoard("listSyntax",
-            project=example_project.id,
-            lists=[
-                gitlab.ProjectIssueBoardListArgs(
-                    assignee_id=example_user.id,
-                ),
-                gitlab.ProjectIssueBoardListArgs(
-                    milestone_id=example_project_milestone.milestone_id,
-                ),
-            ],
-            opts=pulumi.ResourceOptions(depends_on=[example_project_membership]))
-        ```
-
         ## Import
 
         You can import this resource with an id made up of `{project-id}:{issue-board-id}`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/projectIssueBoard:ProjectIssueBoard kanban 42:1
         ```
@@ -343,58 +299,14 @@
         """
         The `ProjectIssueBoard` resource allows to manage the lifecycle of a Project Issue Board.
 
         > **NOTE:** If the board lists are changed all lists will be recreated.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/boards.html)
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_project = gitlab.Project("exampleProject",
-            description="Lorem Ipsum",
-            visibility_level="public")
-        example_user = gitlab.User("exampleUser",
-            username="example",
-            email="example@example.com",
-            password="example1$$$")
-        example_project_membership = gitlab.ProjectMembership("exampleProjectMembership",
-            project_id=example_project.id,
-            user_id=example_user.id,
-            access_level="developer")
-        example_project_milestone = gitlab.ProjectMilestone("exampleProjectMilestone",
-            project=example_project.id,
-            title="m1")
-        this = gitlab.ProjectIssueBoard("this",
-            project=example_project.id,
-            lists=[
-                gitlab.ProjectIssueBoardListArgs(
-                    assignee_id=example_user.id,
-                ),
-                gitlab.ProjectIssueBoardListArgs(
-                    milestone_id=example_project_milestone.milestone_id,
-                ),
-            ],
-            opts=pulumi.ResourceOptions(depends_on=[example_project_membership]))
-        list_syntax = gitlab.ProjectIssueBoard("listSyntax",
-            project=example_project.id,
-            lists=[
-                gitlab.ProjectIssueBoardListArgs(
-                    assignee_id=example_user.id,
-                ),
-                gitlab.ProjectIssueBoardListArgs(
-                    milestone_id=example_project_milestone.milestone_id,
-                ),
-            ],
-            opts=pulumi.ResourceOptions(depends_on=[example_project_membership]))
-        ```
-
         ## Import
 
         You can import this resource with an id made up of `{project-id}:{issue-board-id}`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/projectIssueBoard:ProjectIssueBoard kanban 42:1
         ```
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,52 +10,52 @@
 from . import _utilities
 
 __all__ = ['ProjectLevelMrApprovalsArgs', 'ProjectLevelMrApprovals']
 
 @pulumi.input_type
 class ProjectLevelMrApprovalsArgs:
     def __init__(__self__, *,
-                 project_id: pulumi.Input[int],
+                 project: pulumi.Input[str],
                  disable_overriding_approvers_per_merge_request: Optional[pulumi.Input[bool]] = None,
                  merge_requests_author_approval: Optional[pulumi.Input[bool]] = None,
                  merge_requests_disable_committers_approval: Optional[pulumi.Input[bool]] = None,
                  require_password_to_approve: Optional[pulumi.Input[bool]] = None,
                  reset_approvals_on_push: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ProjectLevelMrApprovals resource.
-        :param pulumi.Input[int] project_id: The ID of the project to change MR approval configuration.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of a project to change MR approval configuration.
         :param pulumi.Input[bool] disable_overriding_approvers_per_merge_request: By default, users are able to edit the approval rules in merge requests. If set to true,
         :param pulumi.Input[bool] merge_requests_author_approval: Set to `true` if you want to allow merge request authors to self-approve merge requests. Authors
         :param pulumi.Input[bool] merge_requests_disable_committers_approval: Set to `true` if you want to prevent approval of merge requests by merge request committers.
         :param pulumi.Input[bool] require_password_to_approve: Set to `true` if you want to require authentication when approving a merge request.
         :param pulumi.Input[bool] reset_approvals_on_push: Set to `true` if you want to remove all approvals in a merge request when new commits are pushed to its source branch. Default is `true`.
         """
-        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "project", project)
         if disable_overriding_approvers_per_merge_request is not None:
             pulumi.set(__self__, "disable_overriding_approvers_per_merge_request", disable_overriding_approvers_per_merge_request)
         if merge_requests_author_approval is not None:
             pulumi.set(__self__, "merge_requests_author_approval", merge_requests_author_approval)
         if merge_requests_disable_committers_approval is not None:
             pulumi.set(__self__, "merge_requests_disable_committers_approval", merge_requests_disable_committers_approval)
         if require_password_to_approve is not None:
             pulumi.set(__self__, "require_password_to_approve", require_password_to_approve)
         if reset_approvals_on_push is not None:
             pulumi.set(__self__, "reset_approvals_on_push", reset_approvals_on_push)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[int]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The ID of the project to change MR approval configuration.
+        The ID or URL-encoded path of a project to change MR approval configuration.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[int]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="disableOverridingApproversPerMergeRequest")
     def disable_overriding_approvers_per_merge_request(self) -> Optional[pulumi.Input[bool]]:
         """
         By default, users are able to edit the approval rules in merge requests. If set to true,
         """
@@ -116,34 +116,34 @@
 
 @pulumi.input_type
 class _ProjectLevelMrApprovalsState:
     def __init__(__self__, *,
                  disable_overriding_approvers_per_merge_request: Optional[pulumi.Input[bool]] = None,
                  merge_requests_author_approval: Optional[pulumi.Input[bool]] = None,
                  merge_requests_disable_committers_approval: Optional[pulumi.Input[bool]] = None,
-                 project_id: Optional[pulumi.Input[int]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  require_password_to_approve: Optional[pulumi.Input[bool]] = None,
                  reset_approvals_on_push: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ProjectLevelMrApprovals resources.
         :param pulumi.Input[bool] disable_overriding_approvers_per_merge_request: By default, users are able to edit the approval rules in merge requests. If set to true,
         :param pulumi.Input[bool] merge_requests_author_approval: Set to `true` if you want to allow merge request authors to self-approve merge requests. Authors
         :param pulumi.Input[bool] merge_requests_disable_committers_approval: Set to `true` if you want to prevent approval of merge requests by merge request committers.
-        :param pulumi.Input[int] project_id: The ID of the project to change MR approval configuration.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of a project to change MR approval configuration.
         :param pulumi.Input[bool] require_password_to_approve: Set to `true` if you want to require authentication when approving a merge request.
         :param pulumi.Input[bool] reset_approvals_on_push: Set to `true` if you want to remove all approvals in a merge request when new commits are pushed to its source branch. Default is `true`.
         """
         if disable_overriding_approvers_per_merge_request is not None:
             pulumi.set(__self__, "disable_overriding_approvers_per_merge_request", disable_overriding_approvers_per_merge_request)
         if merge_requests_author_approval is not None:
             pulumi.set(__self__, "merge_requests_author_approval", merge_requests_author_approval)
         if merge_requests_disable_committers_approval is not None:
             pulumi.set(__self__, "merge_requests_disable_committers_approval", merge_requests_disable_committers_approval)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
         if require_password_to_approve is not None:
             pulumi.set(__self__, "require_password_to_approve", require_password_to_approve)
         if reset_approvals_on_push is not None:
             pulumi.set(__self__, "reset_approvals_on_push", reset_approvals_on_push)
 
     @property
     @pulumi.getter(name="disableOverridingApproversPerMergeRequest")
@@ -178,24 +178,24 @@
         return pulumi.get(self, "merge_requests_disable_committers_approval")
 
     @merge_requests_disable_committers_approval.setter
     def merge_requests_disable_committers_approval(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "merge_requests_disable_committers_approval", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the project to change MR approval configuration.
+        The ID or URL-encoded path of a project to change MR approval configuration.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="requirePasswordToApprove")
     def require_password_to_approve(self) -> Optional[pulumi.Input[bool]]:
         """
         Set to `true` if you want to require authentication when approving a merge request.
         """
@@ -222,15 +222,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  disable_overriding_approvers_per_merge_request: Optional[pulumi.Input[bool]] = None,
                  merge_requests_author_approval: Optional[pulumi.Input[bool]] = None,
                  merge_requests_disable_committers_approval: Optional[pulumi.Input[bool]] = None,
-                 project_id: Optional[pulumi.Input[int]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  require_password_to_approve: Optional[pulumi.Input[bool]] = None,
                  reset_approvals_on_push: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The `gitlab_project_level_mr_approval_rule` resource allows to manage the lifecycle of a Merge Request-level approval rule.
 
         > This resource requires a GitLab Enterprise instance.
@@ -241,15 +241,15 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         foo_project = gitlab.Project("fooProject", description="My example project")
         foo_project_level_mr_approvals = gitlab.ProjectLevelMrApprovals("fooProjectLevelMrApprovals",
-            project_id=foo_project.id,
+            project=foo_project.id,
             reset_approvals_on_push=True,
             disable_overriding_approvers_per_merge_request=False,
             merge_requests_author_approval=False,
             merge_requests_disable_committers_approval=True)
         ```
 
         ## Import
@@ -265,15 +265,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disable_overriding_approvers_per_merge_request: By default, users are able to edit the approval rules in merge requests. If set to true,
         :param pulumi.Input[bool] merge_requests_author_approval: Set to `true` if you want to allow merge request authors to self-approve merge requests. Authors
         :param pulumi.Input[bool] merge_requests_disable_committers_approval: Set to `true` if you want to prevent approval of merge requests by merge request committers.
-        :param pulumi.Input[int] project_id: The ID of the project to change MR approval configuration.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of a project to change MR approval configuration.
         :param pulumi.Input[bool] require_password_to_approve: Set to `true` if you want to require authentication when approving a merge request.
         :param pulumi.Input[bool] reset_approvals_on_push: Set to `true` if you want to remove all approvals in a merge request when new commits are pushed to its source branch. Default is `true`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -290,15 +290,15 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         foo_project = gitlab.Project("fooProject", description="My example project")
         foo_project_level_mr_approvals = gitlab.ProjectLevelMrApprovals("fooProjectLevelMrApprovals",
-            project_id=foo_project.id,
+            project=foo_project.id,
             reset_approvals_on_push=True,
             disable_overriding_approvers_per_merge_request=False,
             merge_requests_author_approval=False,
             merge_requests_disable_committers_approval=True)
         ```
 
         ## Import
@@ -327,32 +327,32 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  disable_overriding_approvers_per_merge_request: Optional[pulumi.Input[bool]] = None,
                  merge_requests_author_approval: Optional[pulumi.Input[bool]] = None,
                  merge_requests_disable_committers_approval: Optional[pulumi.Input[bool]] = None,
-                 project_id: Optional[pulumi.Input[int]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  require_password_to_approve: Optional[pulumi.Input[bool]] = None,
                  reset_approvals_on_push: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectLevelMrApprovalsArgs.__new__(ProjectLevelMrApprovalsArgs)
 
             __props__.__dict__["disable_overriding_approvers_per_merge_request"] = disable_overriding_approvers_per_merge_request
             __props__.__dict__["merge_requests_author_approval"] = merge_requests_author_approval
             __props__.__dict__["merge_requests_disable_committers_approval"] = merge_requests_disable_committers_approval
-            if project_id is None and not opts.urn:
-                raise TypeError("Missing required property 'project_id'")
-            __props__.__dict__["project_id"] = project_id
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
             __props__.__dict__["require_password_to_approve"] = require_password_to_approve
             __props__.__dict__["reset_approvals_on_push"] = reset_approvals_on_push
         super(ProjectLevelMrApprovals, __self__).__init__(
             'gitlab:index/projectLevelMrApprovals:ProjectLevelMrApprovals',
             resource_name,
             __props__,
             opts)
@@ -360,39 +360,39 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             disable_overriding_approvers_per_merge_request: Optional[pulumi.Input[bool]] = None,
             merge_requests_author_approval: Optional[pulumi.Input[bool]] = None,
             merge_requests_disable_committers_approval: Optional[pulumi.Input[bool]] = None,
-            project_id: Optional[pulumi.Input[int]] = None,
+            project: Optional[pulumi.Input[str]] = None,
             require_password_to_approve: Optional[pulumi.Input[bool]] = None,
             reset_approvals_on_push: Optional[pulumi.Input[bool]] = None) -> 'ProjectLevelMrApprovals':
         """
         Get an existing ProjectLevelMrApprovals resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disable_overriding_approvers_per_merge_request: By default, users are able to edit the approval rules in merge requests. If set to true,
         :param pulumi.Input[bool] merge_requests_author_approval: Set to `true` if you want to allow merge request authors to self-approve merge requests. Authors
         :param pulumi.Input[bool] merge_requests_disable_committers_approval: Set to `true` if you want to prevent approval of merge requests by merge request committers.
-        :param pulumi.Input[int] project_id: The ID of the project to change MR approval configuration.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of a project to change MR approval configuration.
         :param pulumi.Input[bool] require_password_to_approve: Set to `true` if you want to require authentication when approving a merge request.
         :param pulumi.Input[bool] reset_approvals_on_push: Set to `true` if you want to remove all approvals in a merge request when new commits are pushed to its source branch. Default is `true`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectLevelMrApprovalsState.__new__(_ProjectLevelMrApprovalsState)
 
         __props__.__dict__["disable_overriding_approvers_per_merge_request"] = disable_overriding_approvers_per_merge_request
         __props__.__dict__["merge_requests_author_approval"] = merge_requests_author_approval
         __props__.__dict__["merge_requests_disable_committers_approval"] = merge_requests_disable_committers_approval
-        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["project"] = project
         __props__.__dict__["require_password_to_approve"] = require_password_to_approve
         __props__.__dict__["reset_approvals_on_push"] = reset_approvals_on_push
         return ProjectLevelMrApprovals(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="disableOverridingApproversPerMergeRequest")
     def disable_overriding_approvers_per_merge_request(self) -> pulumi.Output[Optional[bool]]:
@@ -414,20 +414,20 @@
     def merge_requests_disable_committers_approval(self) -> pulumi.Output[Optional[bool]]:
         """
         Set to `true` if you want to prevent approval of merge requests by merge request committers.
         """
         return pulumi.get(self, "merge_requests_disable_committers_approval")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[int]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        The ID of the project to change MR approval configuration.
+        The ID or URL-encoded path of a project to change MR approval configuration.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
     @property
     @pulumi.getter(name="requirePasswordToApprove")
     def require_password_to_approve(self) -> pulumi.Output[Optional[bool]]:
         """
         Set to `true` if you want to require authentication when approving a merge request.
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 __all__ = ['ProjectMembershipArgs', 'ProjectMembership']
 
 @pulumi.input_type
 class ProjectMembershipArgs:
     def __init__(__self__, *,
                  access_level: pulumi.Input[str],
-                 project_id: pulumi.Input[str],
+                 project: pulumi.Input[str],
                  user_id: pulumi.Input[int],
                  expires_at: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectMembership resource.
         :param pulumi.Input[str] access_level: The access level for the member. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         :param pulumi.Input[int] user_id: The id of the user.
         :param pulumi.Input[str] expires_at: Expiration date for the project membership. Format: `YYYY-MM-DD`
         """
         pulumi.set(__self__, "access_level", access_level)
-        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "user_id", user_id)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Input[str]:
@@ -40,24 +40,24 @@
         return pulumi.get(self, "access_level")
 
     @access_level.setter
     def access_level(self, value: pulumi.Input[str]):
         pulumi.set(self, "access_level", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> pulumi.Input[int]:
         """
         The id of the user.
         """
@@ -81,29 +81,29 @@
 
 
 @pulumi.input_type
 class _ProjectMembershipState:
     def __init__(__self__, *,
                  access_level: Optional[pulumi.Input[str]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering ProjectMembership resources.
         :param pulumi.Input[str] access_level: The access level for the member. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] expires_at: Expiration date for the project membership. Format: `YYYY-MM-DD`
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
         if user_id is not None:
             pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
@@ -124,24 +124,24 @@
         return pulumi.get(self, "expires_at")
 
     @expires_at.setter
     def expires_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_at", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[int]]:
         """
         The id of the user.
         """
@@ -155,15 +155,15 @@
 class ProjectMembership(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         The `ProjectMembership` resource allows to manage the lifecycle of a users project membership.
 
         > If a project should grant membership to an entire group use the `ProjectShareGroup` resource instead.
 
@@ -173,20 +173,20 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         test = gitlab.ProjectMembership("test",
             access_level="guest",
-            project_id="12345",
+            project="12345",
             user_id=1337)
         example = gitlab.ProjectMembership("example",
             access_level="guest",
             expires_at="2022-12-31",
-            project_id="67890",
+            project="67890",
             user_id=1234)
         ```
 
         ## Import
 
         GitLab project membership can be imported using an id made up of `project_id:user_id`, e.g.
 
@@ -194,15 +194,15 @@
          $ pulumi import gitlab:index/projectMembership:ProjectMembership test "12345:1337"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the member. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] expires_at: Expiration date for the project membership. Format: `YYYY-MM-DD`
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectMembershipArgs,
@@ -218,20 +218,20 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         test = gitlab.ProjectMembership("test",
             access_level="guest",
-            project_id="12345",
+            project="12345",
             user_id=1337)
         example = gitlab.ProjectMembership("example",
             access_level="guest",
             expires_at="2022-12-31",
-            project_id="67890",
+            project="67890",
             user_id=1234)
         ```
 
         ## Import
 
         GitLab project membership can be imported using an id made up of `project_id:user_id`, e.g.
 
@@ -252,32 +252,32 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectMembershipArgs.__new__(ProjectMembershipArgs)
 
             if access_level is None and not opts.urn:
                 raise TypeError("Missing required property 'access_level'")
             __props__.__dict__["access_level"] = access_level
             __props__.__dict__["expires_at"] = expires_at
-            if project_id is None and not opts.urn:
-                raise TypeError("Missing required property 'project_id'")
-            __props__.__dict__["project_id"] = project_id
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
             if user_id is None and not opts.urn:
                 raise TypeError("Missing required property 'user_id'")
             __props__.__dict__["user_id"] = user_id
         super(ProjectMembership, __self__).__init__(
             'gitlab:index/projectMembership:ProjectMembership',
             resource_name,
             __props__,
@@ -285,35 +285,35 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_level: Optional[pulumi.Input[str]] = None,
             expires_at: Optional[pulumi.Input[str]] = None,
-            project_id: Optional[pulumi.Input[str]] = None,
+            project: Optional[pulumi.Input[str]] = None,
             user_id: Optional[pulumi.Input[int]] = None) -> 'ProjectMembership':
         """
         Get an existing ProjectMembership resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the member. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] expires_at: Expiration date for the project membership. Format: `YYYY-MM-DD`
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectMembershipState.__new__(_ProjectMembershipState)
 
         __props__.__dict__["access_level"] = access_level
         __props__.__dict__["expires_at"] = expires_at
-        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["project"] = project
         __props__.__dict__["user_id"] = user_id
         return ProjectMembership(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Output[str]:
         """
@@ -326,20 +326,20 @@
     def expires_at(self) -> pulumi.Output[Optional[str]]:
         """
         Expiration date for the project membership. Format: `YYYY-MM-DD`
         """
         return pulumi.get(self, "expires_at")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> pulumi.Output[int]:
         """
         The id of the user.
         """
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_mirror.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_share_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 __all__ = ['ProjectShareGroupArgs', 'ProjectShareGroup']
 
 @pulumi.input_type
 class ProjectShareGroupArgs:
     def __init__(__self__, *,
                  group_id: pulumi.Input[int],
-                 project_id: pulumi.Input[str],
+                 project: pulumi.Input[str],
                  access_level: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectShareGroup resource.
         :param pulumi.Input[int] group_id: The id of the group.
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         :param pulumi.Input[str] access_level: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] group_access: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
         pulumi.set(__self__, "group_id", group_id)
-        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "project", project)
         if access_level is not None:
             warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
             pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if group_access is not None:
             pulumi.set(__self__, "group_access", group_access)
@@ -44,24 +44,24 @@
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
@@ -86,33 +86,33 @@
 
 @pulumi.input_type
 class _ProjectShareGroupState:
     def __init__(__self__, *,
                  access_level: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[int]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None):
+                 project: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectShareGroup resources.
         :param pulumi.Input[str] access_level: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] group_access: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[int] group_id: The id of the group.
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         """
         if access_level is not None:
             warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
             pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if group_access is not None:
             pulumi.set(__self__, "group_access", group_access)
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
@@ -143,35 +143,35 @@
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
 
 class ProjectShareGroup(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[int]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ProjectShareGroup` resource allows to manage the lifecycle of project shared with a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/projects.html#share-project-with-group)
 
         ## Example Usage
@@ -179,15 +179,15 @@
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         test = gitlab.ProjectShareGroup("test",
             group_access="guest",
             group_id=1337,
-            project_id="12345")
+            project="12345")
         ```
 
         ## Import
 
         GitLab project group shares can be imported using an id made up of `projectid:groupid`, e.g.
 
         ```sh
@@ -195,15 +195,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] group_access: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[int] group_id: The id of the group.
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectShareGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -217,15 +217,15 @@
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         test = gitlab.ProjectShareGroup("test",
             group_access="guest",
             group_id=1337,
-            project_id="12345")
+            project="12345")
         ```
 
         ## Import
 
         GitLab project group shares can be imported using an id made up of `projectid:groupid`, e.g.
 
         ```sh
@@ -246,15 +246,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  group_access: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[int]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -264,51 +264,51 @@
                 warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
                 pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
             __props__.__dict__["access_level"] = access_level
             __props__.__dict__["group_access"] = group_access
             if group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'group_id'")
             __props__.__dict__["group_id"] = group_id
-            if project_id is None and not opts.urn:
-                raise TypeError("Missing required property 'project_id'")
-            __props__.__dict__["project_id"] = project_id
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
         super(ProjectShareGroup, __self__).__init__(
             'gitlab:index/projectShareGroup:ProjectShareGroup',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_level: Optional[pulumi.Input[str]] = None,
             group_access: Optional[pulumi.Input[str]] = None,
             group_id: Optional[pulumi.Input[int]] = None,
-            project_id: Optional[pulumi.Input[str]] = None) -> 'ProjectShareGroup':
+            project: Optional[pulumi.Input[str]] = None) -> 'ProjectShareGroup':
         """
         Get an existing ProjectShareGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[str] group_access: The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         :param pulumi.Input[int] group_id: The id of the group.
-        :param pulumi.Input[str] project_id: The id of the project.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectShareGroupState.__new__(_ProjectShareGroupState)
 
         __props__.__dict__["access_level"] = access_level
         __props__.__dict__["group_access"] = group_access
         __props__.__dict__["group_id"] = group_id
-        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["project"] = project
         return ProjectShareGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Output[Optional[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
@@ -328,14 +328,14 @@
     def group_id(self) -> pulumi.Output[int]:
         """
         The id of the group.
         """
         return pulumi.get(self, "group_id")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "project")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_tag.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/project_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,38 @@
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  project: pulumi.Input[str],
                  value: pulumi.Input[str],
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectVariable resource.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "value", value)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
@@ -112,14 +116,26 @@
         return pulumi.get(self, "protected")
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
+    @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         return pulumi.get(self, "variable_type")
 
@@ -132,36 +148,40 @@
 class _ProjectVariableState:
     def __init__(__self__, *,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectVariable resources.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
+        if raw is not None:
+            pulumi.set(__self__, "raw", raw)
         if value is not None:
             pulumi.set(__self__, "value", value)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
     @pulumi.getter(name="environmentScope")
@@ -221,14 +241,26 @@
 
     @protected.setter
     def protected(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "protected", value)
 
     @property
     @pulumi.getter
+    def raw(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @raw.setter
+    def raw(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "raw", value)
+
+    @property
+    @pulumi.getter
     def value(self) -> Optional[pulumi.Input[str]]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @value.setter
@@ -254,14 +286,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ProjectVariable` resource allows to manage the lifecycle of a CI/CD variable for a project.
 
         > **Important:** If your GitLab version is older than 13.4, you may see nondeterministic behavior when updating or deleting ProjectVariable resources with non-unique keys, for example if there is another variable with the same key and different environment scope. See [this GitLab issue](https://gitlab.com/gitlab-org/gitlab/-/issues/9912).
@@ -292,14 +325,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -349,14 +383,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
+                 raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -369,20 +404,19 @@
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["masked"] = masked
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             __props__.__dict__["protected"] = protected
+            __props__.__dict__["raw"] = raw
             if value is None and not opts.urn:
                 raise TypeError("Missing required property 'value'")
-            __props__.__dict__["value"] = None if value is None else pulumi.Output.secret(value)
+            __props__.__dict__["value"] = value
             __props__.__dict__["variable_type"] = variable_type
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["value"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(ProjectVariable, __self__).__init__(
             'gitlab:index/projectVariable:ProjectVariable',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -390,40 +424,43 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             environment_scope: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             masked: Optional[pulumi.Input[bool]] = None,
             project: Optional[pulumi.Input[str]] = None,
             protected: Optional[pulumi.Input[bool]] = None,
+            raw: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None,
             variable_type: Optional[pulumi.Input[str]] = None) -> 'ProjectVariable':
         """
         Get an existing ProjectVariable resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
+        :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectVariableState.__new__(_ProjectVariableState)
 
         __props__.__dict__["environment_scope"] = environment_scope
         __props__.__dict__["key"] = key
         __props__.__dict__["masked"] = masked
         __props__.__dict__["project"] = project
         __props__.__dict__["protected"] = protected
+        __props__.__dict__["raw"] = raw
         __props__.__dict__["value"] = value
         __props__.__dict__["variable_type"] = variable_type
         return ProjectVariable(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> pulumi.Output[Optional[str]]:
@@ -462,14 +499,22 @@
         """
         If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         """
         return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
+    def raw(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
+        """
+        return pulumi.get(self, "raw")
+
+    @property
+    @pulumi.getter
     def value(self) -> pulumi.Output[str]:
         """
         The value of the variable.
         """
         return pulumi.get(self, "value")
 
     @property
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/provider.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/release_link.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/runner.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_custom_issue_tracker.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_custom_issue_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,16 @@
                  issues_url: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  project_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ServiceCustomIssueTracker` resource allows to manage the lifecycle of a project integration with Custom Issue Tracker.
 
+        > This resource is deprecated. use `IntegrationCustomIssueTracker`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#custom-issue-tracker)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -211,15 +213,15 @@
             project=awesome_project.id,
             project_url="https://customtracker.com/issues",
             issues_url="https://customtracker.com/TEST-:id")
         ```
 
         ## Import
 
-        You can import a gitlab_service_external_wiki state using the project ID, e.g.
+        You can import a gitlab_service_custom_issue_tracker state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceCustomIssueTracker:ServiceCustomIssueTracker tracker 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -232,14 +234,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceCustomIssueTrackerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceCustomIssueTracker` resource allows to manage the lifecycle of a project integration with Custom Issue Tracker.
 
+        > This resource is deprecated. use `IntegrationCustomIssueTracker`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#custom-issue-tracker)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -251,15 +255,15 @@
             project=awesome_project.id,
             project_url="https://customtracker.com/issues",
             issues_url="https://customtracker.com/TEST-:id")
         ```
 
         ## Import
 
-        You can import a gitlab_service_external_wiki state using the project ID, e.g.
+        You can import a gitlab_service_custom_issue_tracker state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceCustomIssueTracker:ServiceCustomIssueTracker tracker 1
         ```
 
         :param str resource_name: The name of the resource.
         :param ServiceCustomIssueTrackerArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_emails_on_push.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_emails_on_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,14 +341,16 @@
                  recipients: Optional[pulumi.Input[str]] = None,
                  send_from_committer_email: Optional[pulumi.Input[bool]] = None,
                  tag_push_events: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The `ServiceEmailsOnPush` resource allows to manage the lifecycle of a project integration with Emails on Push Service.
 
+        > This resource is deprecated. Please use `IntegrationEmailsOnPush` instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#emails-on-push)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -384,14 +386,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceEmailsOnPushArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceEmailsOnPush` resource allows to manage the lifecycle of a project integration with Emails on Push Service.
 
+        > This resource is deprecated. Please use `IntegrationEmailsOnPush` instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#emails-on-push)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_external_wiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,16 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  external_wiki_url: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ServiceExternalWiki` resource allows to manage the lifecycle of a project integration with External Wiki Service.
 
+        > This resource is deprecated. use `IntegrationExternalWiki`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#external-wiki)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -214,14 +216,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceExternalWikiArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceExternalWiki` resource allows to manage the lifecycle of a project integration with External Wiki Service.
 
+        > This resource is deprecated. use `IntegrationExternalWiki`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#external-wiki)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_github.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_github.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,16 @@
                  token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ServiceGithub` resource allows to manage the lifecycle of a project integration with GitHub.
 
         > This resource requires a GitLab Enterprise instance.
 
+        > This resource is deprecated. use `IntegrationGithub`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#github)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -247,15 +249,15 @@
             token="REDACTED",
             repository_url="https://github.com/gitlabhq/terraform-provider-gitlab")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import gitlab:index/serviceGithub:ServiceGithub You can import a service_github state using `<resource> <project_id>`
+         $ pulumi import gitlab:index/serviceGithub:ServiceGithub You can import a gitlab_service_github state using `<resource> <project_id>`
         ```
 
         ```sh
          $ pulumi import gitlab:index/serviceGithub:ServiceGithub github 1
         ```
 
         :param str resource_name: The name of the resource.
@@ -272,14 +274,16 @@
                  args: ServiceGithubArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceGithub` resource allows to manage the lifecycle of a project integration with GitHub.
 
         > This resource requires a GitLab Enterprise instance.
 
+        > This resource is deprecated. use `IntegrationGithub`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#github)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -292,15 +296,15 @@
             token="REDACTED",
             repository_url="https://github.com/gitlabhq/terraform-provider-gitlab")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import gitlab:index/serviceGithub:ServiceGithub You can import a service_github state using `<resource> <project_id>`
+         $ pulumi import gitlab:index/serviceGithub:ServiceGithub You can import a gitlab_service_github state using `<resource> <project_id>`
         ```
 
         ```sh
          $ pulumi import gitlab:index/serviceGithub:ServiceGithub github 1
         ```
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_jira.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,14 +620,16 @@
                  tag_push_events: Optional[pulumi.Input[bool]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `ServiceJira` resource allows to manage the lifecycle of a project integration with Jira.
 
+        > This resource is deprecated. use `IntegrationJira`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/services.html#jira)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -640,15 +642,15 @@
             url="https://jira.example.com",
             username="user",
             password="mypass")
         ```
 
         ## Import
 
-        You can import a service_jira state using the project ID, e.g.
+        You can import a gitlab_service_jira state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceJira:ServiceJira jira 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -674,14 +676,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceJiraArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceJira` resource allows to manage the lifecycle of a project integration with Jira.
 
+        > This resource is deprecated. use `IntegrationJira`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/services.html#jira)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -694,15 +698,15 @@
             url="https://jira.example.com",
             username="user",
             password="mypass")
         ```
 
         ## Import
 
-        You can import a service_jira state using the project ID, e.g.
+        You can import a gitlab_service_jira state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceJira:ServiceJira jira 1
         ```
 
         :param str resource_name: The name of the resource.
         :param ServiceJiraArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_microsoft_teams.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,14 +507,16 @@
                  tag_push_events: Optional[pulumi.Input[bool]] = None,
                  webhook: Optional[pulumi.Input[str]] = None,
                  wiki_page_events: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The `ServiceMicrosoftTeams` resource allows to manage the lifecycle of a project integration with Microsoft Teams.
 
+        > This resource is deprecated. use `IntegrationMicrosoftTeams`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#microsoft-teams)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -526,15 +528,15 @@
             project=awesome_project.id,
             webhook="https://testurl.com/?token=XYZ",
             push_events=True)
         ```
 
         ## Import
 
-        You can import a service_microsoft_teams state using the project ID, e.g.
+        You can import a gitlab_service_microsoft_teams state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceMicrosoftTeams:ServiceMicrosoftTeams teams 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -557,14 +559,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceMicrosoftTeamsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceMicrosoftTeams` resource allows to manage the lifecycle of a project integration with Microsoft Teams.
 
+        > This resource is deprecated. use `IntegrationMicrosoftTeams`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#microsoft-teams)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -576,15 +580,15 @@
             project=awesome_project.id,
             webhook="https://testurl.com/?token=XYZ",
             push_events=True)
         ```
 
         ## Import
 
-        You can import a service_microsoft_teams state using the project ID, e.g.
+        You can import a gitlab_service_microsoft_teams state using the project ID, e.g.
 
         ```sh
          $ pulumi import gitlab:index/serviceMicrosoftTeams:ServiceMicrosoftTeams teams 1
         ```
 
         :param str resource_name: The name of the resource.
         :param ServiceMicrosoftTeamsArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_pipelines_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
                  notify_only_broken_pipelines: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  recipients: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         The `ServicePipelinesEmail` resource allows to manage the lifecycle of a project integration with Pipeline Emails Service.
 
+        > This resource is deprecated. use `IntegrationPipelinesEmail`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#pipeline-emails)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -204,14 +206,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServicePipelinesEmailArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServicePipelinesEmail` resource allows to manage the lifecycle of a project integration with Pipeline Emails Service.
 
+        > This resource is deprecated. use `IntegrationPipelinesEmail`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#pipeline-emails)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/service_slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -811,14 +811,16 @@
                  webhook: Optional[pulumi.Input[str]] = None,
                  wiki_page_channel: Optional[pulumi.Input[str]] = None,
                  wiki_page_events: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The `ServiceSlack` resource allows to manage the lifecycle of a project integration with Slack.
 
+        > This resource is deprecated. use `IntegrationSlack`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#slack-notifications)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
@@ -873,14 +875,16 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceSlackArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `ServiceSlack` resource allows to manage the lifecycle of a project integration with Slack.
 
+        > This resource is deprecated. use `IntegrationSlack`instead!
+
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#slack-notifications)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/topic.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/user_ssh_key.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,75 +5,113 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['UserGpgKeyArgs', 'UserGpgKey']
+__all__ = ['UserSshKeyArgs', 'UserSshKey']
 
 @pulumi.input_type
-class UserGpgKeyArgs:
+class UserSshKeyArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
-                 user_id: Optional[pulumi.Input[int]] = None):
-        """
-        The set of arguments for constructing a UserGpgKey resource.
-        :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+                 title: pulumi.Input[str],
+                 user_id: pulumi.Input[int],
+                 expires_at: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a UserSshKey resource.
+        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        :param pulumi.Input[str] title: The title of the ssh key.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
+        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
         """
         pulumi.set(__self__, "key", key)
-        if user_id is not None:
-            pulumi.set(__self__, "user_id", user_id)
+        pulumi.set(__self__, "title", title)
+        pulumi.set(__self__, "user_id", user_id)
+        if expires_at is not None:
+            pulumi.set(__self__, "expires_at", expires_at)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
-        The armored GPG public key.
+        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        """
+        The title of the ssh key.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+    @property
     @pulumi.getter(name="userId")
-    def user_id(self) -> Optional[pulumi.Input[int]]:
+    def user_id(self) -> pulumi.Input[int]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
-    def user_id(self, value: Optional[pulumi.Input[int]]):
+    def user_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "user_id", value)
 
+    @property
+    @pulumi.getter(name="expiresAt")
+    def expires_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        """
+        return pulumi.get(self, "expires_at")
+
+    @expires_at.setter
+    def expires_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expires_at", value)
+
 
 @pulumi.input_type
-class _UserGpgKeyState:
+class _UserSshKeyState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
+                 expires_at: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  key_id: Optional[pulumi.Input[int]] = None,
+                 title: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
-        Input properties used for looking up and filtering UserGpgKey resources.
+        Input properties used for looking up and filtering UserSshKey resources.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
-        :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] key_id: The ID of the GPG key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        :param pulumi.Input[int] key_id: The ID of the ssh key.
+        :param pulumi.Input[str] title: The title of the ssh key.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
+        if expires_at is not None:
+            pulumi.set(__self__, "expires_at", expires_at)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if key_id is not None:
             pulumi.set(__self__, "key_id", key_id)
+        if title is not None:
+            pulumi.set(__self__, "title", title)
         if user_id is not None:
             pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         """
@@ -82,242 +120,274 @@
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
+    @pulumi.getter(name="expiresAt")
+    def expires_at(self) -> Optional[pulumi.Input[str]]:
+        """
+        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        """
+        return pulumi.get(self, "expires_at")
+
+    @expires_at.setter
+    def expires_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expires_at", value)
+
+    @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
-        The armored GPG public key.
+        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter(name="keyId")
     def key_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The ID of the GPG key.
+        The ID of the ssh key.
         """
         return pulumi.get(self, "key_id")
 
     @key_id.setter
     def key_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "key_id", value)
 
     @property
+    @pulumi.getter
+    def title(self) -> Optional[pulumi.Input[str]]:
+        """
+        The title of the ssh key.
+        """
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "title", value)
+
+    @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "user_id", value)
 
 
-class UserGpgKey(pulumi.CustomResource):
+class UserSshKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 expires_at: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
+                 title: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        The `UserGpgKey` resource allows to manage the lifecycle of a GPG key assigned to the current user or a specific user.
+        The `UserSshKey` resource allows to manage the lifecycle of an SSH key assigned to a user.
 
-        > Managing GPG keys for arbitrary users requires admin privileges.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html#get-a-specific-gpg-key)
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/users.html#single-ssh-key)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example_user = gitlab.get_user(username="example-user")
-        # Manages a GPG key for the specified user. An admin token is required if `user_id` is specified.
-        example_user_gpg_key = gitlab.UserGpgKey("exampleUserGpgKey",
+        example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
             user_id=example_user.id,
-            key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
-        ...
-        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
-        # Manages a GPG key for the current user
-        example_user_user_gpg_key = gitlab.UserGpgKey("exampleUserUserGpgKey", key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
-        ...
-        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
+            title="example-key",
+            key="ssh-ed25519 AAAA...",
+            expires_at="2016-01-21T00:00:00.000Z")
         ```
 
         ## Import
 
-        You can import a GPG key for a specific user using an id made up of `{user-id}:{key}`, e.g.
+        You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example 42:1
-        ```
-
-         Alternatively, you can import a GPG key for the current user using an id made up of `{key}`, e.g.
-
-        ```sh
-         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example_user 1
+         $ pulumi import gitlab:index/userSshKey:UserSshKey example 42:1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        :param pulumi.Input[str] title: The title of the ssh key.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UserGpgKeyArgs,
+                 args: UserSshKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `UserGpgKey` resource allows to manage the lifecycle of a GPG key assigned to the current user or a specific user.
-
-        > Managing GPG keys for arbitrary users requires admin privileges.
+        The `UserSshKey` resource allows to manage the lifecycle of an SSH key assigned to a user.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html#get-a-specific-gpg-key)
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/users.html#single-ssh-key)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example_user = gitlab.get_user(username="example-user")
-        # Manages a GPG key for the specified user. An admin token is required if `user_id` is specified.
-        example_user_gpg_key = gitlab.UserGpgKey("exampleUserGpgKey",
+        example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
             user_id=example_user.id,
-            key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
-        ...
-        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
-        # Manages a GPG key for the current user
-        example_user_user_gpg_key = gitlab.UserGpgKey("exampleUserUserGpgKey", key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
-        ...
-        -----END PGP PUBLIC KEY BLOCK-----\"\"\")
+            title="example-key",
+            key="ssh-ed25519 AAAA...",
+            expires_at="2016-01-21T00:00:00.000Z")
         ```
 
         ## Import
 
-        You can import a GPG key for a specific user using an id made up of `{user-id}:{key}`, e.g.
+        You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example 42:1
-        ```
-
-         Alternatively, you can import a GPG key for the current user using an id made up of `{key}`, e.g.
-
-        ```sh
-         $ pulumi import gitlab:index/userGpgKey:UserGpgKey example_user 1
+         $ pulumi import gitlab:index/userSshKey:UserSshKey example 42:1
         ```
 
         :param str resource_name: The name of the resource.
-        :param UserGpgKeyArgs args: The arguments to use to populate this resource's properties.
+        :param UserSshKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UserGpgKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserSshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 expires_at: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
+                 title: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UserGpgKeyArgs.__new__(UserGpgKeyArgs)
+            __props__ = UserSshKeyArgs.__new__(UserSshKeyArgs)
 
+            __props__.__dict__["expires_at"] = expires_at
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
+            if title is None and not opts.urn:
+                raise TypeError("Missing required property 'title'")
+            __props__.__dict__["title"] = title
+            if user_id is None and not opts.urn:
+                raise TypeError("Missing required property 'user_id'")
             __props__.__dict__["user_id"] = user_id
             __props__.__dict__["created_at"] = None
             __props__.__dict__["key_id"] = None
-        super(UserGpgKey, __self__).__init__(
-            'gitlab:index/userGpgKey:UserGpgKey',
+        super(UserSshKey, __self__).__init__(
+            'gitlab:index/userSshKey:UserSshKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created_at: Optional[pulumi.Input[str]] = None,
+            expires_at: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             key_id: Optional[pulumi.Input[int]] = None,
-            user_id: Optional[pulumi.Input[int]] = None) -> 'UserGpgKey':
+            title: Optional[pulumi.Input[str]] = None,
+            user_id: Optional[pulumi.Input[int]] = None) -> 'UserSshKey':
         """
-        Get an existing UserGpgKey resource's state with the given name, id, and optional extra
+        Get an existing UserSshKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
-        :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] key_id: The ID of the GPG key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        :param pulumi.Input[int] key_id: The ID of the ssh key.
+        :param pulumi.Input[str] title: The title of the ssh key.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UserGpgKeyState.__new__(_UserGpgKeyState)
+        __props__ = _UserSshKeyState.__new__(_UserSshKeyState)
 
         __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["expires_at"] = expires_at
         __props__.__dict__["key"] = key
         __props__.__dict__["key_id"] = key_id
+        __props__.__dict__["title"] = title
         __props__.__dict__["user_id"] = user_id
-        return UserGpgKey(resource_name, opts=opts, __props__=__props__)
+        return UserSshKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
         The time when this key was created in GitLab.
         """
         return pulumi.get(self, "created_at")
 
     @property
+    @pulumi.getter(name="expiresAt")
+    def expires_at(self) -> pulumi.Output[Optional[str]]:
+        """
+        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        """
+        return pulumi.get(self, "expires_at")
+
+    @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
         """
-        The armored GPG public key.
+        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter(name="keyId")
     def key_id(self) -> pulumi.Output[int]:
         """
-        The ID of the GPG key.
+        The ID of the ssh key.
         """
         return pulumi.get(self, "key_id")
 
     @property
+    @pulumi.getter
+    def title(self) -> pulumi.Output[str]:
+        """
+        The title of the ssh key.
+        """
+        return pulumi.get(self, "title")
+
+    @property
     @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Output[Optional[int]]:
+    def user_id(self) -> pulumi.Output[int]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab/integration_custom_issue_tracker.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,389 +5,400 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['UserSshKeyArgs', 'UserSshKey']
+__all__ = ['IntegrationCustomIssueTrackerArgs', 'IntegrationCustomIssueTracker']
 
 @pulumi.input_type
-class UserSshKeyArgs:
+class IntegrationCustomIssueTrackerArgs:
     def __init__(__self__, *,
-                 key: pulumi.Input[str],
-                 title: pulumi.Input[str],
-                 user_id: pulumi.Input[int],
-                 expires_at: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a UserSshKey resource.
-        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
-        :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID or username of the user.
-        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
-        """
-        pulumi.set(__self__, "key", key)
-        pulumi.set(__self__, "title", title)
-        pulumi.set(__self__, "user_id", user_id)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-
-    @property
-    @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
+                 issues_url: pulumi.Input[str],
+                 project: pulumi.Input[str],
+                 project_url: pulumi.Input[str]):
         """
-        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        The set of arguments for constructing a IntegrationCustomIssueTracker resource.
+        :param pulumi.Input[str] issues_url: The URL to view an issue in the external issue tracker. Must contain :id.
+        :param pulumi.Input[str] project: The ID or full path of the project for the custom issue tracker.
+        :param pulumi.Input[str] project_url: The URL to the project in the external issue tracker.
         """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
+        pulumi.set(__self__, "issues_url", issues_url)
+        pulumi.set(__self__, "project", project)
+        pulumi.set(__self__, "project_url", project_url)
 
     @property
-    @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="issuesUrl")
+    def issues_url(self) -> pulumi.Input[str]:
         """
-        The title of the ssh key.
+        The URL to view an issue in the external issue tracker. Must contain :id.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "issues_url")
 
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
+    @issues_url.setter
+    def issues_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "issues_url", value)
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Input[int]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The ID or username of the user.
+        The ID or full path of the project for the custom issue tracker.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "project")
 
-    @user_id.setter
-    def user_id(self, value: pulumi.Input[int]):
-        pulumi.set(self, "user_id", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="projectUrl")
+    def project_url(self) -> pulumi.Input[str]:
         """
-        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        The URL to the project in the external issue tracker.
         """
-        return pulumi.get(self, "expires_at")
+        return pulumi.get(self, "project_url")
 
-    @expires_at.setter
-    def expires_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expires_at", value)
+    @project_url.setter
+    def project_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_url", value)
 
 
 @pulumi.input_type
-class _UserSshKeyState:
+class _IntegrationCustomIssueTrackerState:
     def __init__(__self__, *,
+                 active: Optional[pulumi.Input[bool]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
-                 expires_at: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 key_id: Optional[pulumi.Input[int]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[int]] = None):
-        """
-        Input properties used for looking up and filtering UserSshKey resources.
-        :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
-        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
-        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
-        :param pulumi.Input[int] key_id: The ID of the ssh key.
-        :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID or username of the user.
+                 issues_url: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 project_url: Optional[pulumi.Input[str]] = None,
+                 slug: Optional[pulumi.Input[str]] = None,
+                 updated_at: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering IntegrationCustomIssueTracker resources.
+        :param pulumi.Input[bool] active: Whether the integration is active.
+        :param pulumi.Input[str] created_at: The ISO8601 date/time that this integration was activated at in UTC.
+        :param pulumi.Input[str] issues_url: The URL to view an issue in the external issue tracker. Must contain :id.
+        :param pulumi.Input[str] project: The ID or full path of the project for the custom issue tracker.
+        :param pulumi.Input[str] project_url: The URL to the project in the external issue tracker.
+        :param pulumi.Input[str] slug: The name of the integration in lowercase, shortened to 63 bytes, and with everything except 0-9 and a-z replaced with -. No leading / trailing -. Use in URLs, host names and domain names.
+        :param pulumi.Input[str] updated_at: The ISO8601 date/time that this integration was last updated at in UTC.
         """
+        if active is not None:
+            pulumi.set(__self__, "active", active)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
-        if expires_at is not None:
-            pulumi.set(__self__, "expires_at", expires_at)
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if key_id is not None:
-            pulumi.set(__self__, "key_id", key_id)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if user_id is not None:
-            pulumi.set(__self__, "user_id", user_id)
+        if issues_url is not None:
+            pulumi.set(__self__, "issues_url", issues_url)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
+        if project_url is not None:
+            pulumi.set(__self__, "project_url", project_url)
+        if slug is not None:
+            pulumi.set(__self__, "slug", slug)
+        if updated_at is not None:
+            pulumi.set(__self__, "updated_at", updated_at)
+
+    @property
+    @pulumi.getter
+    def active(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the integration is active.
+        """
+        return pulumi.get(self, "active")
+
+    @active.setter
+    def active(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "active", value)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The time when this key was created in GitLab.
+        The ISO8601 date/time that this integration was activated at in UTC.
         """
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="issuesUrl")
+    def issues_url(self) -> Optional[pulumi.Input[str]]:
         """
-        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        The URL to view an issue in the external issue tracker. Must contain :id.
         """
-        return pulumi.get(self, "expires_at")
+        return pulumi.get(self, "issues_url")
 
-    @expires_at.setter
-    def expires_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expires_at", value)
+    @issues_url.setter
+    def issues_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "issues_url", value)
 
     @property
     @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        The ID or full path of the project for the custom issue tracker.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "project")
 
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="keyId")
-    def key_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="projectUrl")
+    def project_url(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the ssh key.
+        The URL to the project in the external issue tracker.
         """
-        return pulumi.get(self, "key_id")
+        return pulumi.get(self, "project_url")
 
-    @key_id.setter
-    def key_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "key_id", value)
+    @project_url.setter
+    def project_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_url", value)
 
     @property
     @pulumi.getter
-    def title(self) -> Optional[pulumi.Input[str]]:
+    def slug(self) -> Optional[pulumi.Input[str]]:
         """
-        The title of the ssh key.
+        The name of the integration in lowercase, shortened to 63 bytes, and with everything except 0-9 and a-z replaced with -. No leading / trailing -. Use in URLs, host names and domain names.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "slug")
 
-    @title.setter
-    def title(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "title", value)
+    @slug.setter
+    def slug(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "slug", value)
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID or username of the user.
+        The ISO8601 date/time that this integration was last updated at in UTC.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "updated_at")
 
-    @user_id.setter
-    def user_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "user_id", value)
+    @updated_at.setter
+    def updated_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "updated_at", value)
 
 
-class UserSshKey(pulumi.CustomResource):
+class IntegrationCustomIssueTracker(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 expires_at: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[int]] = None,
+                 issues_url: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 project_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `UserSshKey` resource allows to manage the lifecycle of an SSH key assigned to a user.
+        The `IntegrationCustomIssueTracker` resource allows to manage the lifecycle of a project integration with Custom Issue Tracker.
 
-        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/users.html#single-ssh-key)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#custom-issue-tracker)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        example_user = gitlab.get_user(username="example-user")
-        example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
-            user_id=example_user.id,
-            title="example-key",
-            key="ssh-ed25519 AAAA...",
-            expires_at="2016-01-21T00:00:00.000Z")
+        awesome_project = gitlab.Project("awesomeProject",
+            description="My awesome project.",
+            visibility_level="public")
+        tracker = gitlab.IntegrationCustomIssueTracker("tracker",
+            project=awesome_project.id,
+            project_url="https://customtracker.com/issues",
+            issues_url="https://customtracker.com/TEST-:id")
         ```
 
         ## Import
 
-        You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
+        You can import a gitlab_integration_custom_issue_tracker state using the project ID, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/userSshKey:UserSshKey example 42:1
+         $ pulumi import gitlab:index/integrationCustomIssueTracker:IntegrationCustomIssueTracker tracker 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
-        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
-        :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID or username of the user.
+        :param pulumi.Input[str] issues_url: The URL to view an issue in the external issue tracker. Must contain :id.
+        :param pulumi.Input[str] project: The ID or full path of the project for the custom issue tracker.
+        :param pulumi.Input[str] project_url: The URL to the project in the external issue tracker.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UserSshKeyArgs,
+                 args: IntegrationCustomIssueTrackerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `UserSshKey` resource allows to manage the lifecycle of an SSH key assigned to a user.
+        The `IntegrationCustomIssueTracker` resource allows to manage the lifecycle of a project integration with Custom Issue Tracker.
 
-        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/users.html#single-ssh-key)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/integrations.html#custom-issue-tracker)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        example_user = gitlab.get_user(username="example-user")
-        example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
-            user_id=example_user.id,
-            title="example-key",
-            key="ssh-ed25519 AAAA...",
-            expires_at="2016-01-21T00:00:00.000Z")
+        awesome_project = gitlab.Project("awesomeProject",
+            description="My awesome project.",
+            visibility_level="public")
+        tracker = gitlab.IntegrationCustomIssueTracker("tracker",
+            project=awesome_project.id,
+            project_url="https://customtracker.com/issues",
+            issues_url="https://customtracker.com/TEST-:id")
         ```
 
         ## Import
 
-        You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
+        You can import a gitlab_integration_custom_issue_tracker state using the project ID, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/userSshKey:UserSshKey example 42:1
+         $ pulumi import gitlab:index/integrationCustomIssueTracker:IntegrationCustomIssueTracker tracker 1
         ```
 
         :param str resource_name: The name of the resource.
-        :param UserSshKeyArgs args: The arguments to use to populate this resource's properties.
+        :param IntegrationCustomIssueTrackerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UserSshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(IntegrationCustomIssueTrackerArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 expires_at: Optional[pulumi.Input[str]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[int]] = None,
+                 issues_url: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 project_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UserSshKeyArgs.__new__(UserSshKeyArgs)
+            __props__ = IntegrationCustomIssueTrackerArgs.__new__(IntegrationCustomIssueTrackerArgs)
 
-            __props__.__dict__["expires_at"] = expires_at
-            if key is None and not opts.urn:
-                raise TypeError("Missing required property 'key'")
-            __props__.__dict__["key"] = key
-            if title is None and not opts.urn:
-                raise TypeError("Missing required property 'title'")
-            __props__.__dict__["title"] = title
-            if user_id is None and not opts.urn:
-                raise TypeError("Missing required property 'user_id'")
-            __props__.__dict__["user_id"] = user_id
+            if issues_url is None and not opts.urn:
+                raise TypeError("Missing required property 'issues_url'")
+            __props__.__dict__["issues_url"] = issues_url
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
+            if project_url is None and not opts.urn:
+                raise TypeError("Missing required property 'project_url'")
+            __props__.__dict__["project_url"] = project_url
+            __props__.__dict__["active"] = None
             __props__.__dict__["created_at"] = None
-            __props__.__dict__["key_id"] = None
-        super(UserSshKey, __self__).__init__(
-            'gitlab:index/userSshKey:UserSshKey',
+            __props__.__dict__["slug"] = None
+            __props__.__dict__["updated_at"] = None
+        super(IntegrationCustomIssueTracker, __self__).__init__(
+            'gitlab:index/integrationCustomIssueTracker:IntegrationCustomIssueTracker',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            active: Optional[pulumi.Input[bool]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
-            expires_at: Optional[pulumi.Input[str]] = None,
-            key: Optional[pulumi.Input[str]] = None,
-            key_id: Optional[pulumi.Input[int]] = None,
-            title: Optional[pulumi.Input[str]] = None,
-            user_id: Optional[pulumi.Input[int]] = None) -> 'UserSshKey':
+            issues_url: Optional[pulumi.Input[str]] = None,
+            project: Optional[pulumi.Input[str]] = None,
+            project_url: Optional[pulumi.Input[str]] = None,
+            slug: Optional[pulumi.Input[str]] = None,
+            updated_at: Optional[pulumi.Input[str]] = None) -> 'IntegrationCustomIssueTracker':
         """
-        Get an existing UserSshKey resource's state with the given name, id, and optional extra
+        Get an existing IntegrationCustomIssueTracker resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
-        :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
-        :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
-        :param pulumi.Input[int] key_id: The ID of the ssh key.
-        :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID or username of the user.
+        :param pulumi.Input[bool] active: Whether the integration is active.
+        :param pulumi.Input[str] created_at: The ISO8601 date/time that this integration was activated at in UTC.
+        :param pulumi.Input[str] issues_url: The URL to view an issue in the external issue tracker. Must contain :id.
+        :param pulumi.Input[str] project: The ID or full path of the project for the custom issue tracker.
+        :param pulumi.Input[str] project_url: The URL to the project in the external issue tracker.
+        :param pulumi.Input[str] slug: The name of the integration in lowercase, shortened to 63 bytes, and with everything except 0-9 and a-z replaced with -. No leading / trailing -. Use in URLs, host names and domain names.
+        :param pulumi.Input[str] updated_at: The ISO8601 date/time that this integration was last updated at in UTC.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UserSshKeyState.__new__(_UserSshKeyState)
+        __props__ = _IntegrationCustomIssueTrackerState.__new__(_IntegrationCustomIssueTrackerState)
 
+        __props__.__dict__["active"] = active
         __props__.__dict__["created_at"] = created_at
-        __props__.__dict__["expires_at"] = expires_at
-        __props__.__dict__["key"] = key
-        __props__.__dict__["key_id"] = key_id
-        __props__.__dict__["title"] = title
-        __props__.__dict__["user_id"] = user_id
-        return UserSshKey(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["issues_url"] = issues_url
+        __props__.__dict__["project"] = project
+        __props__.__dict__["project_url"] = project_url
+        __props__.__dict__["slug"] = slug
+        __props__.__dict__["updated_at"] = updated_at
+        return IntegrationCustomIssueTracker(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter
+    def active(self) -> pulumi.Output[bool]:
+        """
+        Whether the integration is active.
+        """
+        return pulumi.get(self, "active")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
-        The time when this key was created in GitLab.
+        The ISO8601 date/time that this integration was activated at in UTC.
         """
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter(name="expiresAt")
-    def expires_at(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="issuesUrl")
+    def issues_url(self) -> pulumi.Output[str]:
         """
-        The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
+        The URL to view an issue in the external issue tracker. Must contain :id.
         """
-        return pulumi.get(self, "expires_at")
+        return pulumi.get(self, "issues_url")
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Output[str]:
+    def project(self) -> pulumi.Output[str]:
         """
-        The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
+        The ID or full path of the project for the custom issue tracker.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter(name="keyId")
-    def key_id(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="projectUrl")
+    def project_url(self) -> pulumi.Output[str]:
         """
-        The ID of the ssh key.
+        The URL to the project in the external issue tracker.
         """
-        return pulumi.get(self, "key_id")
+        return pulumi.get(self, "project_url")
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Output[str]:
+    def slug(self) -> pulumi.Output[str]:
         """
-        The title of the ssh key.
+        The name of the integration in lowercase, shortened to 63 bytes, and with everything except 0-9 and a-z replaced with -. No leading / trailing -. Use in URLs, host names and domain names.
         """
-        return pulumi.get(self, "title")
+        return pulumi.get(self, "slug")
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="updatedAt")
+    def updated_at(self) -> pulumi.Output[str]:
         """
-        The ID or username of the user.
+        The ISO8601 date/time that this integration was last updated at in UTC.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "updated_at")
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pulumi-gitlab
-Version: 5.1.0a1685165842
+Version: 6.0.0a1685643149
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -43,15 +43,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
 
@@ -60,15 +60,15 @@
 The `@pulumi/gitlab` package provides a strongly-typed means to create cloud applications that create and interact
 closely with GitLab resources.
 
 ## Configuration
 
 The following configuration points are available:
 
-* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`. 
+* token (Optional) - This is the GitLab personal access token. It must be provided but can also be sourced via `GITLAB_TOKEN`.
 
 * base_url (Optional) - This is the target GitLab base API endpoint. Providing a value is a requirement when working with GitLab CE or GitLab Enterprise e.g. https://my.gitlab.server/api/v4/. It is optional to provide this value and it can also be sourced from the GITLAB_BASE_URL environment variable. The value must end with a slash.
 
 * cacert_file (Optional) - This is a file containing the ca cert to verify the gitlab instance. This is available for use when working with GitLab CE or Gitlab Enterprise with a locally-issued or self-signed certificate chain.
 
 * insecure (Optional) - When set to true this disables SSL verification of the connection to the GitLab instance. Defaults to `false`.
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-6.0.0a1685643149/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,23 @@
 pulumi_gitlab/group_membership.py
 pulumi_gitlab/group_project_file_template.py
 pulumi_gitlab/group_saml_link.py
 pulumi_gitlab/group_share_group.py
 pulumi_gitlab/group_variable.py
 pulumi_gitlab/instance_cluster.py
 pulumi_gitlab/instance_variable.py
+pulumi_gitlab/integration_custom_issue_tracker.py
+pulumi_gitlab/integration_emails_on_push.py
+pulumi_gitlab/integration_external_wiki.py
+pulumi_gitlab/integration_github.py
+pulumi_gitlab/integration_jira.py
+pulumi_gitlab/integration_microsoft_teams.py
+pulumi_gitlab/integration_pipelines_email.py
+pulumi_gitlab/integration_slack.py
 pulumi_gitlab/label.py
-pulumi_gitlab/managed_license.py
 pulumi_gitlab/outputs.py
 pulumi_gitlab/pages_domain.py
 pulumi_gitlab/personal_access_token.py
 pulumi_gitlab/pipeline_schedule.py
 pulumi_gitlab/pipeline_schedule_variable.py
 pulumi_gitlab/pipeline_trigger.py
 pulumi_gitlab/project.py
@@ -82,14 +89,15 @@
 pulumi_gitlab/project_cluster.py
 pulumi_gitlab/project_custom_attribute.py
 pulumi_gitlab/project_environment.py
 pulumi_gitlab/project_freeze_period.py
 pulumi_gitlab/project_hook.py
 pulumi_gitlab/project_issue.py
 pulumi_gitlab/project_issue_board.py
+pulumi_gitlab/project_label.py
 pulumi_gitlab/project_level_mr_approvals.py
 pulumi_gitlab/project_membership.py
 pulumi_gitlab/project_milestone.py
 pulumi_gitlab/project_mirror.py
 pulumi_gitlab/project_protected_environment.py
 pulumi_gitlab/project_runner_enablement.py
 pulumi_gitlab/project_share_group.py
```

### Comparing `pulumi_gitlab-5.1.0a1685165842/setup.py` & `pulumi_gitlab-6.0.0a1685643149/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1685165842"
-PLUGIN_VERSION = "5.1.0-alpha.1685165842+6a8f4690"
+VERSION = "6.0.0a1685643149"
+PLUGIN_VERSION = "6.0.0-alpha.1685643149+9f77f727"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'gitlab', PLUGIN_VERSION])
         except OSError as error:
```


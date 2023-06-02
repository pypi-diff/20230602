# Comparing `tmp/gardener-cicd-libs-1.2065.0.tar.gz` & `tmp/gardener-cicd-libs-1.2066.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2065.0.tar", last modified: Fri May 26 13:23:41 2023, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2066.0.tar", last modified: Fri Jun  2 05:01:03 2023, max compression
```

## Comparing `gardener-cicd-libs-1.2065.0.tar` & `gardener-cicd-libs-1.2066.0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.648912 gardener-cicd-libs-1.2065.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10735 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/jira.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.652912 gardener-cicd-libs-1.2065.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)     9811 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    16096 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)     9393 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.652912 gardener-cicd-libs-1.2065.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/replicate.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)    19528 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.652912 gardener-cicd-libs-1.2065.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.652912 gardener-cicd-libs-1.2065.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14969 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.656912 gardener-cicd-libs-1.2065.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    17522 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.656912 gardener-cicd-libs-1.2065.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     2587 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5217 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    18964 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    17352 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)    10994 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27053 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.660913 gardener-cicd-libs-1.2065.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-26 13:23:37.000000 gardener-cicd-libs-1.2065.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4192 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      639 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.664913 gardener-cicd-libs-1.2065.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/alter_container_images.py
--rw-r--r--   0 root         (0) root         (0)     9157 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    11982 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     5609 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     3439 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8822 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     5271 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     3660 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)     4201 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    37200 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     4902 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     7028 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/scan_container_images.mako
--rw-r--r--   0 root         (0) root         (0)     6837 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6804 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    20511 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1165 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.664913 gardener-cicd-libs-1.2065.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23433 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5362 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.664913 gardener-cicd-libs-1.2065.0/container/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16315 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.664913 gardener-cicd-libs-1.2065.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      735 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/cosign.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/platform.py
--rwxr-xr-x   0 root         (0) root         (0)    26860 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/rbsc_bom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9639 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     5163 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 13:23:41.000000 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6165 2023-05-26 13:23:41.000000 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:23:41.000000 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-26 13:23:41.000000 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-26 13:23:41.000000 gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.668913 gardener-cicd-libs-1.2065.0/github/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11313 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)     9092 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    34570 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/compliance/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/release_notes/renderer.py
--rw-r--r--   0 root         (0) root         (0)    19222 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/release_notes/util.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    33961 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    15039 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6926 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/kube/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/kube/ctx.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/kube/helm.py
--rw-r--r--   0 root         (0) root         (0)    26693 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/kube/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/mail/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/makoutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/product/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/product/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/product/util.py
--rw-r--r--   0 root         (0) root         (0)    22448 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/product/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11275 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     4645 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/release_notes/markdown.py
--rw-r--r--   0 root         (0) root         (0)    10869 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     7272 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/reutil.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.672913 gardener-cicd-libs-1.2065.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/container/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.676913 gardener-cicd-libs-1.2065.0/test/github/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6142 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/github_util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/test/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/release_notes/default_util.py
--rw-r--r--   0 root         (0) root         (0)    18172 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/release_notes/renderer_test.py
--rw-r--r--   0 root         (0) root         (0)    21822 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/github/release_notes/util_test.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/kubeutil_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:41.680913 gardener-cicd-libs-1.2065.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    15220 2023-05-26 13:22:41.000000 gardener-cicd-libs-1.2065.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.186242 gardener-cicd-libs-1.2066.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10735 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/jira.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.186242 gardener-cicd-libs-1.2066.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    16096 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     9393 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/replicate.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)    17536 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14969 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.190242 gardener-cicd-libs-1.2066.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.194242 gardener-cicd-libs-1.2066.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    18964 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    17352 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)    10994 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27053 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.194242 gardener-cicd-libs-1.2066.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-02 05:00:59.000000 gardener-cicd-libs-1.2066.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.198242 gardener-cicd-libs-1.2066.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/alter_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    10914 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     3385 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8822 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    36446 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.mako
+-rw-r--r--   0 root         (0) root         (0)     6837 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6804 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    19298 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23433 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/container/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16315 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/cosign.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/platform.py
+-rwxr-xr-x   0 root         (0) root         (0)    26860 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/rbsc_bom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.202242 gardener-cicd-libs-1.2066.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9639 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-02 05:01:03.000000 gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11313 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)     9092 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    34570 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/compliance/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/renderer.py
+-rw-r--r--   0 root         (0) root         (0)    19222 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/release_notes/util.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    33961 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    15039 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/kube/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/helm.py
+-rw-r--r--   0 root         (0) root         (0)    26693 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/kube/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.206242 gardener-cicd-libs-1.2066.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/makoutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/product/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/util.py
+-rw-r--r--   0 root         (0) root         (0)    22350 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/product/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11275 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     7272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/reutil.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7482 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.210242 gardener-cicd-libs-1.2066.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6142 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/github_util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/default_util.py
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/renderer_test.py
+-rw-r--r--   0 root         (0) root         (0)    21822 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/github/release_notes/util_test.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/kubeutil_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:03.214242 gardener-cicd-libs-1.2066.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-06-02 05:00:06.000000 gardener-cicd-libs-1.2066.0/version.py
```

### Comparing `gardener-cicd-libs-1.2065.0/LICENSE.md` & `gardener-cicd-libs-1.2066.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/README.md` & `gardener-cicd-libs-1.2066.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/__init__.py` & `gardener-cicd-libs-1.2066.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2066.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/aws.py` & `gardener-cicd-libs-1.2066.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/clamav.py` & `gardener-cicd-libs-1.2066.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/concourse.py` & `gardener-cicd-libs-1.2066.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/delivery.py` & `gardener-cicd-libs-1.2066.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2066.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/gcp.py` & `gardener-cicd-libs-1.2066.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/github.py` & `gardener-cicd-libs-1.2066.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2066.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/jira.py` & `gardener-cicd-libs-1.2066.0/ccc/jira.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/oci.py` & `gardener-cicd-libs-1.2066.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/protecode.py` & `gardener-cicd-libs-1.2066.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2066.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2066.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cli.py` & `gardener-cicd-libs-1.2066.0/cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/access.py` & `gardener-cicd-libs-1.2066.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/iter.py` & `gardener-cicd-libs-1.2066.0/cnudie/iter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/purge.py` & `gardener-cicd-libs-1.2066.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/replicate.py` & `gardener-cicd-libs-1.2066.0/cnudie/replicate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2066.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/util.py` & `gardener-cicd-libs-1.2066.0/cnudie/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import dataclasses
-import io
 import graphlib
-import os
-import tarfile
 import typing
 
 import deprecated
 
 import ci.util
 import gci.componentmodel as cm
 import oci.model as om
@@ -469,49 +466,7 @@
         for i in left_resource:
             _add_if_not_duplicate(resource_diff.resource_refs_only_left, i)
 
         for i in right_resource:
             _add_if_not_duplicate(resource_diff.resource_refs_only_right, i)
 
     return resource_diff
-
-
-def component_descriptors_from_ctf_archive(
-    ctf_archive: typing.Union[str, typing.IO[bytes]],
-) -> typing.Generator[cm.ComponentDescriptor, None, None]:
-    if isinstance(ctf_archive, str):
-        if os.path.isdir(ctf_archive):
-            # TODO Implement after clarifying with @Schrodit
-            raise NotImplementedError(f'{ctf_archive=}')
-        elif os.path.isfile(ctf_archive):
-            yield from _component_descriptors_from_ctf_archive_file(ctf_file_path=ctf_archive)
-        else:
-            raise NotImplementedError(f'{ctf_archive=}')
-    elif isinstance(ctf_archive, io.IOBase):
-        yield from _component_descriptors_from_ctf_archive_file(ctf_file_path=ctf_archive)
-    else:
-        raise NotImplementedError(f'{ctf_archive=}')
-
-
-def _component_descriptors_from_ctf_archive_file(
-    ctf_file_path: str = None,
-    ctf_fileobj: typing.IO[bytes] = None,
-) -> typing.Generator[cm.ComponentDescriptor, None, None]:
-
-    if not (bool(ctf_fileobj) ^ bool(ctf_file_path)):
-        raise ValueError('One of ctf_file_path or ctf_file_path must be given')
-
-    with tarfile.open(name=ctf_file_path, fileobj=ctf_fileobj, mode='r|') as ctf_tar:
-        for member in ctf_tar:
-            # manually check whether member is a file to be able to generate a more expressive
-            # error-msg
-            if not member.isfile():
-                raise RuntimeError('Content of the CTF archive is not a file')
-
-            with tarfile.open(fileobj=ctf_tar.extractfile(member), mode='r|') as component_tar:
-                first_entry = component_tar.next()
-                if not first_entry.name == 'component-descriptor.yaml':
-                    raise RuntimeError(
-                        'First entry in the component archive MUST be the component descriptor'
-                    )
-                cd_dict = ci.util.load_yaml(component_tar.extractfile(first_entry))
-                yield cm.ComponentDescriptor.from_dict(cd_dict)
```

### Comparing `gardener-cicd-libs-1.2065.0/cnudie/validate.py` & `gardener-cicd-libs-1.2066.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/client/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/client/api.py` & `gardener-cicd-libs-1.2066.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/client/model.py` & `gardener-cicd-libs-1.2066.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2066.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/client/util.py` & `gardener-cicd-libs-1.2066.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2066.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/factory.py` & `gardener-cicd-libs-1.2066.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/base.py` & `gardener-cicd-libs-1.2066.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/job.py` & `gardener-cicd-libs-1.2066.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2066.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2066.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/step.py` & `gardener-cicd-libs-1.2066.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/draft_release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/update_component_deps.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2066.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/replicator.py` & `gardener-cicd-libs-1.2066.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2066.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2066.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2066.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2066.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2066.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/alter_container_images.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/alter_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.mako`

 * *Files 7% similar despite different names*

```diff
@@ -147,30 +147,22 @@
 descriptor_out_dir = os.path.abspath('${job_step.output("component_descriptor_dir")}')
 
 v2_outfile = os.path.join(
   descriptor_out_dir,
   component_descriptor_fname(schema_version=gci.componentmodel.SchemaVersion.V2),
 )
 
-ctf_out_path = os.path.abspath(
-  os.path.join(descriptor_out_dir, product.v2.CTF_OUT_DIR_NAME)
-)
-
 descriptor_script = os.path.abspath(
   '${job_variant.main_repository().resource_name()}/.ci/component_descriptor'
 )
 if os.path.isfile(descriptor_script):
   is_executable = bool(os.stat(descriptor_script)[stat.ST_MODE] & stat.S_IEXEC)
   if not is_executable:
     fail(f'descriptor script file exists but is not executable: {descriptor_script}')
 
-  # dump base_ctf_v2 as valid component archive and pass it to descriptor script
-  base_ctf_dir = os.path.join(descriptor_out_dir, 'base_component_ctf')
-  os.makedirs(base_ctf_dir, exist_ok=False)
-
   # dump base_descriptor_v2 and pass it to descriptor script
   base_component_descriptor_fname = (
     f'base_{component_descriptor_fname(schema_version=gci.componentmodel.SchemaVersion.V2)}'
   )
   base_descriptor_file_v2 = os.path.join(
     descriptor_out_dir,
     base_component_descriptor_fname,
@@ -178,17 +170,15 @@
   with open(base_descriptor_file_v2, 'w') as f:
     f.write(dump_component_descriptor_v2(base_descriptor_v2))
 
   subproc_env = os.environ.copy()
   subproc_env['${main_repo_path_env_var}'] = main_repo_path
   subproc_env['MAIN_REPO_DIR'] = main_repo_path
   subproc_env['BASE_DEFINITION_PATH'] = base_descriptor_file_v2
-  subproc_env['BASE_CTF_PATH'] = base_ctf_dir
   subproc_env['COMPONENT_DESCRIPTOR_PATH'] = v2_outfile
-  subproc_env['CTF_PATH'] = ctf_out_path
   subproc_env['COMPONENT_NAME'] = component_name
   subproc_env['COMPONENT_VERSION'] = effective_version
   subproc_env['EFFECTIVE_VERSION'] = effective_version
   subproc_env['CURRENT_COMPONENT_REPOSITORY'] = ctx_repository_base_url
 
   # pass predefined command to add dependencies for convenience purposes
   add_dependencies_cmd = ' '.join((
@@ -218,31 +208,29 @@
   logger.info(
     f'no component_descriptor script found at {descriptor_script} - will use default'
   )
   with open(v2_outfile, 'w') as f:
     f.write(dump_component_descriptor_v2(base_descriptor_v2))
   logger.info(f'wrote component descriptor (v2): {v2_outfile=}')
 
-have_ctf = os.path.exists(ctf_out_path)
 have_cd = os.path.exists(v2_outfile)
 
-if not have_ctf ^ have_cd:
-    fail(f'exactly one of {ctf_out_path=}, {v2_outfile=} must exist')
-elif have_cd:
+if have_cd:
   # ensure the script actually created an output
   if not os.path.isfile(v2_outfile):
     fail(f'no descriptor file was found at: {v2_outfile=}')
 
   descriptor_v2 = cm.ComponentDescriptor.from_dict(
     ci.util.parse_yaml_file(v2_outfile)
   )
   logger.info(f'found component-descriptor (v2) at {v2_outfile=}:\n')
   print(dump_component_descriptor_v2(descriptor_v2))
-elif have_ctf:
-  logger.info(f'found ctf-archive at {ctf_out_path=}')
+else:
+  print(f'XXX: did not find a component-descriptor at {v2_outfile=}')
+  exit(1)
 
 % if not (job_variant.has_trait('release') or job_variant.has_trait('update_component_deps')):
 if snapshot_ctx_repository_base_url:
   if have_cd:
     snapshot_descriptor = cm.ComponentDescriptor.from_dict(
       ci.util.parse_yaml_file(v2_outfile)
     )
@@ -256,34 +244,15 @@
     product.v2.upload_component_descriptor_v2_to_oci_registry(
       component_descriptor_v2=snapshot_descriptor,
     )
     logger.info(
       'Successfully uploaded snapshot Component Descriptor to '
       f'{product.v2._target_oci_ref(snapshot_descriptor.component)}'
     )
-  elif have_ctf:
-    subprocess_args = [
-      'component-cli',
-      'ctf',
-      'push',
-      ctf_out_path,
-    ]
-    if ctx_repository_base_url != snapshot_ctx_repository_base_url:
-      subprocess_args.extend(['--repo-ctx', snapshot_ctx_repository_base_url])
-
-    subprocess.run(
-      subprocess_args,
-      check=True,
-      env=subproc_env,
-    )
 % endif
-if have_ctf:
-  logger.info(f'processed ctf-archive at {ctf_out_path=} - exiting')
-  # XXX TODO: also calculate bom-diff!
-  exit(0)
 
 # determine "bom-diff" (changed component references)
 try:
   bom_diff = component_diff_since_last_release(
       component_descriptor=descriptor_v2,
       ctx_repo_url=ctx_repository_base_url,
   )
@@ -301,17 +270,14 @@
   write_component_diff(
     component_diff=bom_diff,
     out_path=dependencies_path,
   )
   with open(dependencies_path) as f:
     print(f.read())
 % if retention_policy:
-if have_ctf:
-  logger.warning('purging not implemented for ctf')
-  exit(0)
 
 logger.info('will honour retention-policy')
 retention_policy = dacite.from_dict(
   data_class=version.VersionRetentionPolicies,
   data=${retention_policy},
   config=dacite.Config(cast=(enum.Enum,)),
 )
```

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/draft_release.mako`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 component_descriptor_trait = job_variant.trait('component_descriptor')
 component_name = component_descriptor_trait.component_name()
 version_operation = draft_release_trait._preprocess()
 component_descriptor_path = os.path.join(
     job_step.input('component_descriptor_dir'),
     cdu.component_descriptor_fname(gci.componentmodel.SchemaVersion.V2),
 )
-ctf_path = os.path.join(
-  job_step.input('component_descriptor_dir'),
-  product.v2.CTF_OUT_DIR_NAME,
-)
 %>
 import version
 import os
 
 import ci.util
 import ccc.github
 import cnudie.util
@@ -53,34 +49,26 @@
 processed_version = version.process_version(
     version_str=version_str,
     operation='${version_operation}',
 )
 
 repo_dir = ci.util.existing_dir('${repo.resource_name()}')
 
-have_ctf = os.path.exists(ctf_path := '${ctf_path}')
 have_cd = os.path.exists(component_descriptor_path := '${component_descriptor_path}')
 
-if not have_ctf ^ have_cd:
-    ci.util.fail('exactly one of component-descriptor, or ctf-archive must exist')
-
 if have_cd:
     component = cm.ComponentDescriptor.from_dict(
             component_descriptor_dict=ci.util.parse_yaml_file(
                 component_descriptor_path,
             ),
             validation_mode=cm.ValidationMode.WARN,
     ).component
-elif have_ctf:
-    for component_descriptor in cnudie.util.component_descriptors_from_ctf_archive(ctf_path):
-        component = component_descriptor.component
-        if component.name == '${component_name}':
-            break
-    else:
-        ci.util.fail(f'did not find component-descriptor for ${component_name}')
+else:
+   print('did not find component-descriptor')
+   exit(1)
 
 github_cfg = ccc.github.github_cfg_for_repo_url(
   ci.util.urljoin(
     '${repo.repo_hostname()}',
     '${repo.repo_path()}'
   ),
 )
```

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/os_id.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/release.mako`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 
 repo = job_variant.main_repository()
 
 component_descriptor_path = os.path.join(
   job_step.input('component_descriptor_dir'),
   cdu.component_descriptor_fname(gci.componentmodel.SchemaVersion.V2),
 )
-ctf_path = os.path.join(
-  job_step.input('component_descriptor_dir'),
-  product.v2.CTF_OUT_DIR_NAME,
-)
 
 component_descriptor_trait = job_variant.trait('component_descriptor')
 component_name = component_descriptor_trait.component_name()
 
 release_callback_path = release_trait.release_callback_path()
 next_version_callback_path = release_trait.next_version_callback_path()
 %>
@@ -85,15 +81,14 @@
 % else:
 release_commit_callback_image_reference = None
 % endif
 
 concourse.steps.release.release_and_prepare_next_dev_cycle(
   component_name=component_name,
   component_descriptor_path='${component_descriptor_path}',
-  ctf_path='${ctf_path}',
   % if has_slack_trait:
   slack_channel_configs=${slack_channel_cfgs},
   % endif
   % if release_callback_path:
   release_commit_callback='${release_callback_path}',
   % endif
   % if next_version_callback_path:
```

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,34 +50,28 @@
 import oci.model
 
 logger = logging.getLogger('step.release')
 
 
 def component_descriptors(
     component_descriptor_path: str,
-    ctf_path: str,
 ):
-    have_ctf = os.path.exists(ctf_path)
     have_cd = os.path.exists(component_descriptor_path)
 
-    if not have_ctf ^ have_cd:
-        ci.util.fail('exactly one of component-descriptor, or ctf-archive must exist')
-
     if have_cd:
         component_descriptor = cm.ComponentDescriptor.from_dict(
                 component_descriptor_dict=ci.util.parse_yaml_file(
                     component_descriptor_path,
                 ),
                 validation_mode=cm.ValidationMode.WARN,
         )
         yield component_descriptor.component
         return
-    elif have_ctf:
-        for component_descriptor in cnudie.util.component_descriptors_from_ctf_archive(ctf_path):
-            yield component_descriptor.component
+    else:
+        raise RuntimeError('did not find component-descriptor')
 
 
 class TransactionContext:
     def __init__(self):
         self._step_outputs = {}
 
     def has_output(self, step_name: str):
@@ -539,28 +533,23 @@
 
 
 class UploadComponentDescriptorStep(TransactionalStep):
     def __init__(
         self,
         github_helper: GitHubRepositoryHelper,
         components: tuple[cm.Component],
-        ctf_path:str,
         release_on_github: bool,
     ):
         self.github_helper = not_none(github_helper)
         self.components = components
-        self.ctf_path = ctf_path
         self.release_on_github = release_on_github
 
     def name(self):
         return "Upload Component Descriptor"
 
-    def _have_ctf(self) -> bool:
-        return os.path.exists(self.ctf_path)
-
     def validate(self):
         components: tuple[cm.Component] = tuple(
             cnudie.util.iter_sorted(
                 self.components,
             )
         )
 
@@ -620,24 +609,15 @@
                 tgt_ref = product.v2._target_oci_ref(component=component)
 
                 logger.info(f'publishing CNUDIE-Component-Descriptor to {tgt_ref=}')
                 product.v2.upload_component_descriptor_v2_to_oci_registry(
                     component_descriptor_v2=component,
                 )
 
-        def upload_ctf(ctf_path: str):
-            subprocess.run(
-                ('component-cli', 'ctf', 'push', ctf_path),
-                check=True,
-            )
-
-        if not self._have_ctf():
-            upload_component_descriptors(components=components)
-        else:
-            upload_ctf(ctf_path=self.ctf_path)
+        upload_component_descriptors(components=components)
 
         def upload_component_descriptor_as_release_asset():
             try:
                 release = self.github_helper.repository.release_from_tag(release_tag_name)
 
                 for component in components:
                     component_descriptor = cm.ComponentDescriptor(
@@ -872,29 +852,27 @@
     repo_dir: str,
     repository_version_file_path: str,
     git_tags: list,
     github_release_tag: dict,
     release_commit_callback_image_reference: str,
     release_notes_handling: str,
     component_descriptor_path: str=None,
-    ctf_path: str=None,
     next_cycle_commit_message_prefix: str=None,
     next_version_callback: str=None,
     prerelease_suffix: str="dev",
     rebase_before_release: bool=False,
     release_on_github: bool=True,
     release_commit_callback: str=None,
     release_commit_message_prefix: str=None,
     slack_channel_configs: list=[],
     version_operation: str='bump_minor',
 ):
     components = tuple(
         component_descriptors(
             component_descriptor_path=component_descriptor_path,
-            ctf_path=ctf_path,
         )
     )
     if len(components) == 1:
         component = components[0]
     elif len(components) == 0:
         logger.fatal('no component-descriptors could be found - aborting release')
         exit(1)
@@ -977,15 +955,14 @@
             release_version=release_version,
         )
         step_list.append(github_release_step)
 
     upload_component_descriptor_step = UploadComponentDescriptorStep(
         github_helper=github_helper,
         components=components,
-        ctf_path=ctf_path,
         release_on_github=release_on_github,
     )
 
     step_list.append(upload_component_descriptor_step)
 
     release_transaction = Transaction(
         ctx=transaction_ctx,
```

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/scan_container_images.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/update_component_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,52 +45,22 @@
     return cnudie.retrieve.create_default_component_descriptor_lookup()
 
 
 def current_product_descriptor():
     component_descriptor_file_path = cdu.component_descriptor_path(
         schema_version=gci.componentmodel.SchemaVersion.V2,
     )
-    ctf_out_file_path = os.path.join(
-      ci.util.check_env('COMPONENT_DESCRIPTOR_DIR'),
-      product.v2.CTF_OUT_DIR_NAME,
-    )
 
     # cd is supplied via component-descriptor file. Parse and return
     if os.path.isfile(component_descriptor_file_path):
         return gci.componentmodel.ComponentDescriptor.from_dict(
             component_descriptor_dict=ci.util.parse_yaml_file(component_descriptor_file_path,)
         )
-
-    # cd is supplied via CTF archive. Parse ctf archive and return correct one
-    elif os.path.isfile(ctf_out_file_path):
-        component_name = ci.util.check_env('COMPONENT_NAME')
-        component_descriptors = [
-            cd
-            for cd in cnudie.util.component_descriptors_from_ctf_archive(ctf_out_file_path)
-            if cd.component.name == component_name
-        ]
-        if (cds_len := len(component_descriptors)) == 0:
-            raise RuntimeError(
-                f"No component descriptor for component '{component_name}' found in ctf archive "
-                f"at '{ctf_out_file_path}'"
-            )
-        elif cds_len > 1:
-            raise RuntimeError(
-                f"More than one component descriptor for component '{component_name}' found in ctf "
-                f"archive at '{ctf_out_file_path}'"
-            )
-        else:
-            return component_descriptors[0]
-
-    # either ctf or cd-file _must_ exist (enforced by component-descriptor-trait)
     else:
-        raise RuntimeError(
-            f'Neither component-descriptor file at {component_descriptor_file_path=} or '
-            f'ctf-archive at {ctf_out_file_path=} exist'
-        )
+        raise RuntimeError(f'did not find component-descriptor at {component_descriptor_file_path=}')
 
 
 def current_component():
     return current_product_descriptor().component
 
 
 def close_obsolete_pull_requests(
```

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2066.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2066.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/templates/__init__.py` & `gardener-cicd-libs-1.2066.0/concourse/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2066.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/util.py` & `gardener-cicd-libs-1.2066.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/concourse/validator.py` & `gardener-cicd-libs-1.2066.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/container/__init__.py` & `gardener-cicd-libs-1.2066.0/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/container/util.py` & `gardener-cicd-libs-1.2066.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cosign/__init__.py` & `gardener-cicd-libs-1.2066.0/cosign/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/cosign/payload.py` & `gardener-cicd-libs-1.2066.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/cosign.py` & `gardener-cicd-libs-1.2066.0/ctt/cosign.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/filters.py` & `gardener-cicd-libs-1.2066.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/platform.py` & `gardener-cicd-libs-1.2066.0/ctt/platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2066.0/ctt/process_dependencies.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2066.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/processors.py` & `gardener-cicd-libs-1.2066.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2066.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2066.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2066.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2066.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2066.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2066.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2066.0/ctt/uploaders.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/ctt/util.py` & `gardener-cicd-libs-1.2066.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/delivery/client.py` & `gardener-cicd-libs-1.2066.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/delivery/model.py` & `gardener-cicd-libs-1.2066.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/delivery/util.py` & `gardener-cicd-libs-1.2066.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/dockerutil.py` & `gardener-cicd-libs-1.2066.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/dso/cvss.py` & `gardener-cicd-libs-1.2066.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/dso/labels.py` & `gardener-cicd-libs-1.2066.0/dso/labels.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/dso/model.py` & `gardener-cicd-libs-1.2066.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2066.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-gardener-cicd-base>=1.2065.0
-gardener-oci>=1.2065.0
+gardener-cicd-base>=1.2066.0
+gardener-oci>=1.2066.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.13.36
-aliyun-python-sdk-ecs==4.24.62
+aliyun-python-sdk-ecs==4.24.63
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
 bcrypt<5.0.0
 boto3
 cachecontrol<1
 cachetools
 cryptography
```

### Comparing `gardener-cicd-libs-1.2065.0/github/__init__.py` & `gardener-cicd-libs-1.2066.0/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/codeowners.py` & `gardener-cicd-libs-1.2066.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2066.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2066.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/compliance/model.py` & `gardener-cicd-libs-1.2066.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/compliance/report.py` & `gardener-cicd-libs-1.2066.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2066.0/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/release_notes/model.py` & `gardener-cicd-libs-1.2066.0/github/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/release_notes/renderer.py` & `gardener-cicd-libs-1.2066.0/github/release_notes/renderer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/release_notes/util.py` & `gardener-cicd-libs-1.2066.0/github/release_notes/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/retry.py` & `gardener-cicd-libs-1.2066.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/user.py` & `gardener-cicd-libs-1.2066.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/util.py` & `gardener-cicd-libs-1.2066.0/github/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/github/webhook.py` & `gardener-cicd-libs-1.2066.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/gitutil.py` & `gardener-cicd-libs-1.2066.0/gitutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/gziputil.py` & `gardener-cicd-libs-1.2066.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/http_requests.py` & `gardener-cicd-libs-1.2066.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/kube/__init__.py` & `gardener-cicd-libs-1.2066.0/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/kube/ctx.py` & `gardener-cicd-libs-1.2066.0/kube/ctx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/kube/helm.py` & `gardener-cicd-libs-1.2066.0/kube/helm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/kube/helper.py` & `gardener-cicd-libs-1.2066.0/kube/helper.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/mail/__init__.py` & `gardener-cicd-libs-1.2066.0/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2066.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/mailutil.py` & `gardener-cicd-libs-1.2066.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/product/__init__.py` & `gardener-cicd-libs-1.2066.0/product/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/product/util.py` & `gardener-cicd-libs-1.2066.0/product/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/product/v2.py` & `gardener-cicd-libs-1.2066.0/product/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,14 @@
 import ci.util
 import oci.model as om
 import version
 
 logger = logging.getLogger(__name__)
 
 
-CTF_OUT_DIR_NAME = 'cnudie-transport-format.out'
-
-
 COMPONENT_TYPE_NAME = 'component'
 
 
 def _normalise_component_name(component_name:str) -> str:
     return component_name.lower()  # oci-spec allows only lowercase
 
 
@@ -522,23 +519,23 @@
 def enumerate_oci_resources(
     component_descriptor,
     cache_dir: str=None,
 ):
     for component in components(component_descriptor, cache_dir=cache_dir):
         for resource in resources(
             component=component,
-            resource_types=[gci.componentmodel.ResourceType.OCI_IMAGE],
-            resource_access_types=[gci.componentmodel.AccessType.OCI_REGISTRY],
+            resource_types=[cm.ResourceType.OCI_IMAGE],
+            resource_access_types=[cm.AccessType.OCI_REGISTRY],
         ):
             yield (component, resource)
 
 
 def greatest_references(
-    references: typing.Iterable[gci.componentmodel.ComponentReference],
-) -> gci.componentmodel.ComponentReference:
+    references: typing.Iterable[cm.ComponentReference],
+) -> typing.Iterable[cm.ComponentReference]:
     '''
     yields the component references from the specified iterable of ComponentReference that
     have the greatest version (grouped by component name).
     Id est: if the sequence contains exactly one version of each contained component name,
     the sequence is returned unchanged.
     '''
     references = tuple(references)
```

### Comparing `gardener-cicd-libs-1.2065.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2066.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2066.0/release_notes/fetch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/release_notes/markdown.py` & `gardener-cicd-libs-1.2066.0/release_notes/markdown.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/release_notes/model.py` & `gardener-cicd-libs-1.2066.0/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/release_notes/utils.py` & `gardener-cicd-libs-1.2066.0/release_notes/utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/reutil.py` & `gardener-cicd-libs-1.2066.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/setup.py` & `gardener-cicd-libs-1.2066.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/slackclient/__init__.py` & `gardener-cicd-libs-1.2066.0/slackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/slackclient/util.py` & `gardener-cicd-libs-1.2066.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/tarutil.py` & `gardener-cicd-libs-1.2066.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/__init__.py` & `gardener-cicd-libs-1.2066.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/_test_utils.py` & `gardener-cicd-libs-1.2066.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/__init__.py` & `gardener-cicd-libs-1.2066.0/test/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/filter_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2066.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/release_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2066.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/container/__init__.py` & `gardener-cicd-libs-1.2066.0/test/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/__init__.py` & `gardener-cicd-libs-1.2066.0/test/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2066.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2066.0/test/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/release_notes/default_util.py` & `gardener-cicd-libs-1.2066.0/test/github/release_notes/default_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/release_notes/renderer_test.py` & `gardener-cicd-libs-1.2066.0/test/github/release_notes/renderer_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/github/release_notes/util_test.py` & `gardener-cicd-libs-1.2066.0/test/github/release_notes/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/kubeutil_test.py` & `gardener-cicd-libs-1.2066.0/test/kubeutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/product_/__init__.py` & `gardener-cicd-libs-1.2066.0/test/product_/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/reutil_test.py` & `gardener-cicd-libs-1.2066.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/test/version_test.py` & `gardener-cicd-libs-1.2066.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/unixutil/model.py` & `gardener-cicd-libs-1.2066.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/unixutil/scan.py` & `gardener-cicd-libs-1.2066.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2065.0/version.py` & `gardener-cicd-libs-1.2066.0/version.py`

 * *Files identical despite different names*


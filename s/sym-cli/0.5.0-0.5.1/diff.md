# Comparing `tmp/sym_cli-0.5.0.tar.gz` & `tmp/sym_cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_cli-0.5.0.tar", max compression
+gzip compressed data, was "sym_cli-0.5.1.tar", max compression
```

## Comparing `sym_cli-0.5.0.tar` & `sym_cli-0.5.1.tar`

### file list

```diff
@@ -1,118 +1,113 @@
--rw-r--r--   0        0        0      147 2023-05-31 14:20:47.903977 sym_cli-0.5.0/DESCRIPTION.md
--rw-r--r--   0        0        0     2054 2023-05-31 14:20:49.647979 sym_cli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/__init__.py
--rw-r--r--   0        0        0     2175 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/action_registry.py
--rw-r--r--   0        0        0     1463 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ansible_action.py
--rw-r--r--   0        0        0     1614 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ansible_playbook_action.py
--rw-r--r--   0        0        0     1438 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ssh_session_action.py
--rw-r--r--   0        0        0     1299 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/sym_action.py
--rw-r--r--   0        0        0     1675 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/write_creds_action.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/__init__.py
--rw-r--r--   0        0        0    18609 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/connection/__init__.py
--rw-r--r--   0        0        0    13933 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/connection/sym_aws_ssm.py
--rw-r--r--   0        0        0       90 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/__init__.py
--rw-r--r--   0        0        0     1897 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ansible.py
--rw-r--r--   0        0        0     2179 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ansible_playbook.py
--rw-r--r--   0        0        0      664 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/check.py
--rw-r--r--   0        0        0     2073 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/config.py
--rw-r--r--   0        0        0     1016 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/defaults.py
--rw-r--r--   0        0        0     3503 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/doctor.py
--rw-r--r--   0        0        0      798 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/exec.py
--rw-r--r--   0        0        0     1098 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/host_to_instance.py
--rw-r--r--   0        0        0      683 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/login.py
--rw-r--r--   0        0        0     1040 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/resources.py
--rw-r--r--   0        0        0     7895 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh.py
--rw-r--r--   0        0        0     1224 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh_session.py
--rw-r--r--   0        0        0     1767 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh_tunnel.py
--rw-r--r--   0        0        0      894 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssm.py
--rw-r--r--   0        0        0     2750 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/sym.py
--rw-r--r--   0        0        0      204 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/version.py
--rw-r--r--   0        0        0     1894 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/write_creds.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/constants/__init__.py
--rw-r--r--   0        0        0      746 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/constants/env.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/__init__.py
--rw-r--r--   0        0        0      310 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/ansible_options.py
--rw-r--r--   0        0        0     1376 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/request_data.py
--rw-r--r--   0        0        0      142 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/target_options.py
--rw-r--r--   0        0        0     5000 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/decorators.py
--rw-r--r--   0        0        0     5573 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/errors.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/__init__.py
--rw-r--r--   0        0        0     6376 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ansible.py
--rw-r--r--   0        0        0     5142 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/boto.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/__init__.py
--rw-r--r--   0        0        0     1614 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/core.py
--rw-r--r--   0        0        0     1827 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/ec2.py
--rw-r--r--   0        0        0     1088 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/model.py
--rw-r--r--   0        0        0     1694 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/runner.py
--rw-r--r--   0        0        0     2202 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/ssh.py
--rw-r--r--   0        0        0     3938 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/config.py
--rw-r--r--   0        0        0      626 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/constants.py
--rw-r--r--   0        0        0     8538 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/doctor.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/__init__.py
--rw-r--r--   0        0        0     2086 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/cache.py
--rw-r--r--   0        0        0     7538 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/client.py
--rw-r--r--   0        0        0      214 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/factory.py
--rw-r--r--   0        0        0     2867 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/multiregion.py
--rw-r--r--   0        0        0      912 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/global_options.py
--rw-r--r--   0        0        0     4865 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/options.py
--rw-r--r--   0        0        0      287 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/org.py
--rw-r--r--   0        0        0     8756 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/params.py
--rw-r--r--   0        0        0      946 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/pty.py
--rw-r--r--   0        0        0    10719 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/ssh.py
--rw-r--r--   0        0        0     1543 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/sym_group.py
--rw-r--r--   0        0        0      812 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/threading.py
--rw-r--r--   0        0        0      262 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/validations.py
--rw-r--r--   0        0        0     1722 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/version.py
--rw-r--r--   0        0        0       90 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/__init__.py
--rw-r--r--   0        0        0     3256 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_config.py
--rw-r--r--   0        0        0     5733 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_okta.py
--rw-r--r--   0        0        0     2887 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_profile.py
--rw-r--r--   0        0        0     1168 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/chooser.py
--rw-r--r--   0        0        0     6699 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml2aws.py
--rw-r--r--   0        0        0     8989 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml_client.py
--rw-r--r--   0        0        0     1247 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml_client_factory.py
--rw-r--r--   0        0        0      277 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/sym.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/__init__.py
--rw-r--r--   0        0        0     3834 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/conftest.py
--rw-r--r--   0        0        0    10471 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ansible.py
--rw-r--r--   0        0        0      677 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_host_to_instance.py
--rw-r--r--   0        0        0     6642 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ssh.py
--rw-r--r--   0        0        0     1685 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ssh_session.py
--rw-r--r--   0        0        0    11563 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_write_creds.py
--rw-r--r--   0        0        0     4423 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/__init__.py
--rw-r--r--   0        0        0      635 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_intercept_error.py
--rw-r--r--   0        0        0      425 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_retry.py
--rw-r--r--   0        0        0     1108 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_setup_sentry.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/__init__.py
--rw-r--r--   0        0        0      957 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/conftest.py
--rw-r--r--   0        0        0     3642 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_caching.py
--rw-r--r--   0        0        0     6985 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_client.py
--rw-r--r--   0        0        0     2084 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_multiregion.py
--rw-r--r--   0        0        0      846 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/sandbox.py
--rw-r--r--   0        0        0     1702 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_ansible.py
--rw-r--r--   0        0        0     2383 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_boto.py
--rw-r--r--   0        0        0     3087 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_config.py
--rw-r--r--   0        0        0      581 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_has_command.py
--rw-r--r--   0        0        0      563 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_params.py
--rw-r--r--   0        0        0     2786 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_ssh.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/conftest.py
--rw-r--r--   0        0        0   267688 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli-0.2.7.json
--rw-r--r--   0        0        0   267688 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli.json
--rw-r--r--   0        0        0     5329 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/test_updater.py
--rw-r--r--   0        0        0     1497 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/integration/conftest.py
--rw-r--r--   0        0        0     2832 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/integration/test_ld.py
--rw-r--r--   0        0        0      944 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/matchers.py
--rw-r--r--   0        0        0        0 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/__init__.py
--rw-r--r--   0        0        0     3886 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/conftest.py
--rw-r--r--   0        0        0     2187 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_okta.py
--rw-r--r--   0        0        0     1224 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_profile.py
--rw-r--r--   0        0        0     1365 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_chooser.py
--rw-r--r--   0        0        0     3722 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml2aws.py
--rw-r--r--   0        0        0     1333 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml_client.py
--rw-r--r--   0        0        0     3730 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/test_sym.py
--rw-r--r--   0        0        0       22 2023-05-31 14:20:49.695979 sym_cli-0.5.0/sym/cli/version.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 sym_cli-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-06-02 17:33:47.085867 sym_cli-0.5.1/DESCRIPTION.md
+-rw-r--r--   0        0        0     2054 2023-06-02 17:33:48.821861 sym_cli-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/__init__.py
+-rw-r--r--   0        0        0     2175 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/action_registry.py
+-rw-r--r--   0        0        0     1463 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/ansible_action.py
+-rw-r--r--   0        0        0     1614 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/ansible_playbook_action.py
+-rw-r--r--   0        0        0     1438 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/ssh_session_action.py
+-rw-r--r--   0        0        0     1299 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/sym_action.py
+-rw-r--r--   0        0        0     1675 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/actions/write_creds_action.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/ansible/__init__.py
+-rw-r--r--   0        0        0    18609 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/ansible/connection/__init__.py
+-rw-r--r--   0        0        0    13933 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/ansible/connection/sym_aws_ssm.py
+-rw-r--r--   0        0        0       90 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1897 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ansible.py
+-rw-r--r--   0        0        0     2179 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ansible_playbook.py
+-rw-r--r--   0        0        0      664 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/check.py
+-rw-r--r--   0        0        0     2073 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/config.py
+-rw-r--r--   0        0        0     1016 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/defaults.py
+-rw-r--r--   0        0        0     3503 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/doctor.py
+-rw-r--r--   0        0        0      798 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/exec.py
+-rw-r--r--   0        0        0     1098 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/host_to_instance.py
+-rw-r--r--   0        0        0      683 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/login.py
+-rw-r--r--   0        0        0     1040 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/resources.py
+-rw-r--r--   0        0        0     7895 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ssh.py
+-rw-r--r--   0        0        0     1224 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ssh_session.py
+-rw-r--r--   0        0        0     1767 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ssh_tunnel.py
+-rw-r--r--   0        0        0      894 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/ssm.py
+-rw-r--r--   0        0        0     2750 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/sym.py
+-rw-r--r--   0        0        0      204 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/version.py
+-rw-r--r--   0        0        0     1894 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/commands/write_creds.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/constants/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/constants/env.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/data/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/data/ansible_options.py
+-rw-r--r--   0        0        0     1376 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/data/request_data.py
+-rw-r--r--   0        0        0      142 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/data/target_options.py
+-rw-r--r--   0        0        0     5000 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/decorators.py
+-rw-r--r--   0        0        0     5573 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/errors.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     6376 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ansible.py
+-rw-r--r--   0        0        0     5241 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/boto.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/__init__.py
+-rw-r--r--   0        0        0     1614 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/core.py
+-rw-r--r--   0        0        0     1827 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/ec2.py
+-rw-r--r--   0        0        0     1088 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/model.py
+-rw-r--r--   0        0        0     1694 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/runner.py
+-rw-r--r--   0        0        0     2202 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/check/ssh.py
+-rw-r--r--   0        0        0     3938 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/config.py
+-rw-r--r--   0        0        0      626 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/constants.py
+-rw-r--r--   0        0        0     8538 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/doctor.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0     2086 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ec2/cache.py
+-rw-r--r--   0        0        0     7538 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ec2/client.py
+-rw-r--r--   0        0        0      214 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ec2/factory.py
+-rw-r--r--   0        0        0     2867 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ec2/multiregion.py
+-rw-r--r--   0        0        0      912 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/global_options.py
+-rw-r--r--   0        0        0     4865 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/options.py
+-rw-r--r--   0        0        0      287 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/org.py
+-rw-r--r--   0        0        0     8756 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/params.py
+-rw-r--r--   0        0        0      946 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/pty.py
+-rw-r--r--   0        0        0    10719 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/ssh.py
+-rw-r--r--   0        0        0     1543 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/sym_group.py
+-rw-r--r--   0        0        0      812 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/threading.py
+-rw-r--r--   0        0        0      262 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/validations.py
+-rw-r--r--   0        0        0     1722 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/helpers/version.py
+-rw-r--r--   0        0        0       90 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3399 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/aws_config.py
+-rw-r--r--   0        0        0     5733 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/aws_okta.py
+-rw-r--r--   0        0        0     2887 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/aws_profile.py
+-rw-r--r--   0        0        0     1168 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/chooser.py
+-rw-r--r--   0        0        0     6699 2023-06-02 17:33:47.093866 sym_cli-0.5.1/sym/cli/saml_clients/saml2aws.py
+-rw-r--r--   0        0        0     8989 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/saml_clients/saml_client.py
+-rw-r--r--   0        0        0     1247 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/saml_clients/saml_client_factory.py
+-rw-r--r--   0        0        0      277 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/sym.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/__init__.py
+-rw-r--r--   0        0        0     3834 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/conftest.py
+-rw-r--r--   0        0        0    10471 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/test_ansible.py
+-rw-r--r--   0        0        0      677 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/test_host_to_instance.py
+-rw-r--r--   0        0        0     6642 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/test_ssh.py
+-rw-r--r--   0        0        0     1685 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/test_ssh_session.py
+-rw-r--r--   0        0        0    11563 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/commands/test_write_creds.py
+-rw-r--r--   0        0        0     4423 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/decorators/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/decorators/test_intercept_error.py
+-rw-r--r--   0        0        0      425 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/decorators/test_retry.py
+-rw-r--r--   0        0        0     1108 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/decorators/test_setup_sentry.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/ec2/conftest.py
+-rw-r--r--   0        0        0     3642 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_caching.py
+-rw-r--r--   0        0        0     6985 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_client.py
+-rw-r--r--   0        0        0     2084 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_multiregion.py
+-rw-r--r--   0        0        0      846 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/sandbox.py
+-rw-r--r--   0        0        0     1702 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_ansible.py
+-rw-r--r--   0        0        0     2383 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_boto.py
+-rw-r--r--   0        0        0     3087 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_config.py
+-rw-r--r--   0        0        0      581 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_has_command.py
+-rw-r--r--   0        0        0      563 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_params.py
+-rw-r--r--   0        0        0     2786 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/helpers/test_ssh.py
+-rw-r--r--   0        0        0     1497 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2832 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/integration/test_ld.py
+-rw-r--r--   0        0        0      944 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/matchers.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3886 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/conftest.py
+-rw-r--r--   0        0        0     2187 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/test_aws_okta.py
+-rw-r--r--   0        0        0     1224 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/test_aws_profile.py
+-rw-r--r--   0        0        0     1365 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/test_chooser.py
+-rw-r--r--   0        0        0     3722 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/test_saml2aws.py
+-rw-r--r--   0        0        0     1333 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/saml_clients/test_saml_client.py
+-rw-r--r--   0        0        0     3730 2023-06-02 17:33:47.097866 sym_cli-0.5.1/sym/cli/tests/test_sym.py
+-rw-r--r--   0        0        0       22 2023-06-02 17:33:48.869861 sym_cli-0.5.1/sym/cli/version.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 sym_cli-0.5.1/PKG-INFO
```

### Comparing `sym_cli-0.5.0/pyproject.toml` & `sym_cli-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-cli"
-version = "0.5.0"
+version = "0.5.1"
 description = "Sym's Official CLI for Users"
 authors = ["SymOps, Inc. <pypi@symops.io>"]
 packages = [{ include = "sym/*" }]
 readme = "DESCRIPTION.md"
 homepage = "https://symops.com/"
 documentation = "https://docs.symops.com/docs/install-sym-cli"
 classifiers = [
```

### Comparing `sym_cli-0.5.0/sym/cli/actions/action_registry.py` & `sym_cli-0.5.1/sym/cli/actions/action_registry.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/actions/ansible_action.py` & `sym_cli-0.5.1/sym/cli/actions/ansible_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/actions/ansible_playbook_action.py` & `sym_cli-0.5.1/sym/cli/actions/ansible_playbook_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/actions/ssh_session_action.py` & `sym_cli-0.5.1/sym/cli/actions/ssh_session_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/actions/sym_action.py` & `sym_cli-0.5.1/sym/cli/actions/sym_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/actions/write_creds_action.py` & `sym_cli-0.5.1/sym/cli/actions/write_creds_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/ansible/connection/__init__.py` & `sym_cli-0.5.1/sym/cli/ansible/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/ansible/connection/sym_aws_ssm.py` & `sym_cli-0.5.1/sym/cli/ansible/connection/sym_aws_ssm.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ansible.py` & `sym_cli-0.5.1/sym/cli/commands/ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ansible_playbook.py` & `sym_cli-0.5.1/sym/cli/commands/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/check.py` & `sym_cli-0.5.1/sym/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/config.py` & `sym_cli-0.5.1/sym/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/defaults.py` & `sym_cli-0.5.1/sym/cli/commands/defaults.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/doctor.py` & `sym_cli-0.5.1/sym/cli/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/exec.py` & `sym_cli-0.5.1/sym/cli/commands/exec.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/host_to_instance.py` & `sym_cli-0.5.1/sym/cli/commands/host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/login.py` & `sym_cli-0.5.1/sym/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/resources.py` & `sym_cli-0.5.1/sym/cli/commands/resources.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ssh.py` & `sym_cli-0.5.1/sym/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ssh_session.py` & `sym_cli-0.5.1/sym/cli/commands/ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ssh_tunnel.py` & `sym_cli-0.5.1/sym/cli/commands/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/ssm.py` & `sym_cli-0.5.1/sym/cli/commands/ssm.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/sym.py` & `sym_cli-0.5.1/sym/cli/commands/sym.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/commands/write_creds.py` & `sym_cli-0.5.1/sym/cli/commands/write_creds.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/constants/env.py` & `sym_cli-0.5.1/sym/cli/constants/env.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/data/request_data.py` & `sym_cli-0.5.1/sym/cli/data/request_data.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/decorators.py` & `sym_cli-0.5.1/sym/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/errors.py` & `sym_cli-0.5.1/sym/cli/errors.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/ansible.py` & `sym_cli-0.5.1/sym/cli/helpers/ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/boto.py` & `sym_cli-0.5.1/sym/cli/helpers/boto.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,27 @@
         AccessDeniedPattern: AccessDenied,
         RequestExpired: ExpiredCredentials,
     }
 )
 
 
 def boto_client(saml_client, service):
+    # For the AwsConfig SAML Client, we want to continue to use
+    # the boto session that has the aws profile name configured in it
+    # there could be more better ways to do this if necessary in the future
+    if hasattr(saml_client, "boto_session"):
+        return saml_client.boto_session.client(service)
     creds = saml_client.get_creds()
-    if access_key_id := creds.get("AWS_ACCESS_KEY_ID"):
-        return boto3.client(
-            service,
-            config=BotoConfig(region_name=get_region(saml_client, creds)),
-            aws_access_key_id=access_key_id,
-            aws_secret_access_key=creds["AWS_SECRET_ACCESS_KEY"],
-            aws_session_token=creds.get("AWS_SESSION_TOKEN"),
-        )
-    # If there is no access key id, then assume that the boto3 default session is set up
-    return boto3.client(service)
+    return boto3.client(
+        service,
+        region_name=get_region(saml_client, creds),
+        aws_access_key_id=creds["AWS_ACCESS_KEY_ID"],
+        aws_secret_access_key=creds["AWS_SECRET_ACCESS_KEY"],
+        aws_session_token=creds.get("AWS_SESSION_TOKEN"),
+    )
 
 
 def get_region(saml_client, creds=None) -> str:
     override = saml_client.options.aws_region
     return override or (creds or saml_client.get_creds()).get("AWS_REGION")
```

### Comparing `sym_cli-0.5.0/sym/cli/helpers/check/core.py` & `sym_cli-0.5.1/sym/cli/helpers/check/core.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/check/ec2.py` & `sym_cli-0.5.1/sym/cli/helpers/check/ec2.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/check/model.py` & `sym_cli-0.5.1/sym/cli/helpers/check/model.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/check/runner.py` & `sym_cli-0.5.1/sym/cli/helpers/check/runner.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/check/ssh.py` & `sym_cli-0.5.1/sym/cli/helpers/check/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/config.py` & `sym_cli-0.5.1/sym/cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/constants.py` & `sym_cli-0.5.1/sym/cli/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/doctor.py` & `sym_cli-0.5.1/sym/cli/helpers/doctor.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/ec2/cache.py` & `sym_cli-0.5.1/sym/cli/helpers/ec2/cache.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/ec2/client.py` & `sym_cli-0.5.1/sym/cli/helpers/ec2/client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/ec2/multiregion.py` & `sym_cli-0.5.1/sym/cli/helpers/ec2/multiregion.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/global_options.py` & `sym_cli-0.5.1/sym/cli/helpers/global_options.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/options.py` & `sym_cli-0.5.1/sym/cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/params.py` & `sym_cli-0.5.1/sym/cli/helpers/params.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/pty.py` & `sym_cli-0.5.1/sym/cli/helpers/pty.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/ssh.py` & `sym_cli-0.5.1/sym/cli/helpers/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/sym_group.py` & `sym_cli-0.5.1/sym/cli/helpers/sym_group.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/threading.py` & `sym_cli-0.5.1/sym/cli/helpers/threading.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/helpers/version.py` & `sym_cli-0.5.1/sym/cli/helpers/version.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/aws_config.py` & `sym_cli-0.5.1/sym/cli/saml_clients/aws_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 import os
 from configparser import ConfigParser
 from functools import cached_property
 from pathlib import Path
 from typing import Iterator, Tuple
 
-from boto3 import setup_default_session
 from sym.shared.cli.helpers.contexts import push_env
 from sym.shared.cli.helpers.keywords_to_options import Argument
 
 from sym.cli.helpers.boto import get_identity
 
 from ..decorators import command_require_bins, intercept_errors, run_subprocess
 from ..errors import InvalidResource
 from ..helpers.params import Profile
 from .saml_client import SAMLClient
 
-# The docs say that the credentials file is for sensitive values like actual access keys etc
-# and the config file for less sensitive things like role names, SSO configs.
-AwsConfigPath = Path(os.getenv("AWS_CONFIG_FILE", Path.home() / ".aws" / "config"))
-
-
-class AwsConfig(SAMLClient):
+AwsCredentialsPath = Path(
+    os.getenv("AWS_CREDENTIAL_FILE", Path.home() / ".aws" / "credentials")
+)
+
+# This client assumes that access key and secret are defined in the credentials file.
+# If you want to use a named profile that works with SSO or some other supported AWS credential
+# process, use AwsConfig
+class AwsProfile(SAMLClient):
     binary = "aws"
-    option_value = "aws-config"
+    option_value = "aws-profile"
     priority = 0
-    setup_help = f"Set up your profile in `{str(AwsConfigPath)}`."
+    setup_help = f"Set up your profile in `{str(AwsCredentialsPath)}`."
 
     resource: str
     options: "GlobalOptions"
 
-    def __init__(self, resource: str, *, options: "GlobalOptions") -> None:
-        super().__init__(resource, options=options)
-        # Make the default session use our AWS profile so we don't need to manage sessions in
-        # whatever other call chains there are to get AWS creds
-        setup_default_session(profile_name=resource)
-
     @classmethod
     def _read_creds_config(cls):
         config = ConfigParser(strict=False)
-        if AwsConfigPath.exists():
-            config.read(AwsConfigPath)
+        config.read(AwsCredentialsPath)
         return config
 
     @classmethod
     def validate_resource(cls, resource: str):
         config = cls._read_creds_config()
-        return config.has_section(cls._profile_name(resource))
+        return config.has_section(resource)
 
     @cached_property
     def _section(self):
         config = self.__class__._read_creds_config()
-        return config[self.__class__._profile_name(self.resource)]
-
-    @classmethod
-    def _profile_name(cls, resource: str):
-        return f"profile {resource}"
+        return config[self.resource]
 
     def raise_if_invalid(self):
         if self.__class__.validate_resource(self.resource):
             return
         raise InvalidResource(
             self.resource, self.__class__._read_creds_config().sections()
         )
 
-    # Returning an empty dict here because we set up a default boto session above, so no need
-    # for creds here
     def get_creds(self):
-        return {}
+        creds = {k.upper(): v for k, v in self._section.items() if k.startswith("aws")}
+        creds["AWS_REGION"] = self._section.get("region")
+        creds["AWS_CREDENTIAL_EXPIRATION"] = self._section.get("x_security_token_expires")
+        return creds
 
     @intercept_errors()
     @run_subprocess
     @command_require_bins(binary)
     def _exec(self, *args: str, **opts: str) -> Iterator[Tuple[Argument, ...]]:
         with push_env("AWS_PROFILE", self.resource):
             yield (*args, opts)
 
     def is_setup(self) -> bool:
-        return AwsConfigPath.exists()
+        return AwsCredentialsPath.exists()
 
     def _ensure_config(self, profile: Profile) -> ConfigParser:
         return ConfigParser(strict=False)
 
     def _ensure_session(self, *, force: bool):
         if not force and not self._creds_expiring():
             return
```

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/aws_okta.py` & `sym_cli-0.5.1/sym/cli/saml_clients/aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/aws_profile.py` & `sym_cli-0.5.1/sym/cli/saml_clients/aws_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,91 @@
 import os
 from configparser import ConfigParser
 from functools import cached_property
 from pathlib import Path
 from typing import Iterator, Tuple
 
+from boto3.session import Session
 from sym.shared.cli.helpers.contexts import push_env
 from sym.shared.cli.helpers.keywords_to_options import Argument
 
 from sym.cli.helpers.boto import get_identity
 
 from ..decorators import command_require_bins, intercept_errors, run_subprocess
 from ..errors import InvalidResource
 from ..helpers.params import Profile
 from .saml_client import SAMLClient
 
-AwsCredentialsPath = Path(
-    os.getenv("AWS_CREDENTIAL_FILE", Path.home() / ".aws" / "credentials")
-)
-
-# This client assumes that access key and secret are defined in the credentials file.
-# If you want to use a named profile that works with SSO or some other supported AWS credential
-# process, use AwsConfig
-class AwsProfile(SAMLClient):
+# The docs say that the credentials file is for sensitive values like actual access keys etc
+# and the config file for less sensitive things like role names, SSO configs.
+AwsConfigPath = Path(os.getenv("AWS_CONFIG_FILE", Path.home() / ".aws" / "config"))
+
+
+class AwsConfig(SAMLClient):
     binary = "aws"
-    option_value = "aws-profile"
+    option_value = "aws-config"
     priority = 0
-    setup_help = f"Set up your profile in `{str(AwsCredentialsPath)}`."
+    setup_help = f"Set up your profile in `{str(AwsConfigPath)}`."
 
     resource: str
     options: "GlobalOptions"
+    boto_session: Session
+
+    def __init__(self, resource: str, *, options: "GlobalOptions") -> None:
+        super().__init__(resource, options=options)
+        self.raise_if_invalid()
+        self.boto_session = Session(profile_name=self.resource)
 
     @classmethod
     def _read_creds_config(cls):
         config = ConfigParser(strict=False)
-        config.read(AwsCredentialsPath)
+        if AwsConfigPath.exists():
+            config.read(AwsConfigPath)
         return config
 
     @classmethod
     def validate_resource(cls, resource: str):
         config = cls._read_creds_config()
-        return config.has_section(resource)
+        return config.has_section(cls._profile_name(resource))
 
     @cached_property
     def _section(self):
         config = self.__class__._read_creds_config()
-        return config[self.resource]
+        return config[self.__class__._profile_name(self.resource)]
+
+    @classmethod
+    def _profile_name(cls, resource: str):
+        return f"profile {resource}"
 
     def raise_if_invalid(self):
         if self.__class__.validate_resource(self.resource):
             return
         raise InvalidResource(
             self.resource, self.__class__._read_creds_config().sections()
         )
 
+    # Returning an empty dict here because we set up a default boto session above, so no need
+    # for creds here
     def get_creds(self):
-        creds = {k.upper(): v for k, v in self._section.items() if k.startswith("aws")}
-        creds["AWS_REGION"] = self._section.get("region")
-        creds["AWS_CREDENTIAL_EXPIRATION"] = self._section.get("x_security_token_expires")
-        return creds
+        creds = self.boto_session.get_credentials().get_frozen_credentials()
+        return {
+            "AWS_ACCESS_KEY_ID": creds.access_key,
+            "AWS_SECRET_ACCESS_KEY": creds.secret_key,
+            "AWS_SESSION_TOKEN": creds.token,
+        }
 
     @intercept_errors()
     @run_subprocess
     @command_require_bins(binary)
     def _exec(self, *args: str, **opts: str) -> Iterator[Tuple[Argument, ...]]:
         with push_env("AWS_PROFILE", self.resource):
             yield (*args, opts)
 
     def is_setup(self) -> bool:
-        return AwsCredentialsPath.exists()
+        return AwsConfigPath.exists()
 
     def _ensure_config(self, profile: Profile) -> ConfigParser:
         return ConfigParser(strict=False)
 
     def _ensure_session(self, *, force: bool):
         if not force and not self._creds_expiring():
             return
```

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/chooser.py` & `sym_cli-0.5.1/sym/cli/saml_clients/chooser.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/saml2aws.py` & `sym_cli-0.5.1/sym/cli/saml_clients/saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/saml_client.py` & `sym_cli-0.5.1/sym/cli/saml_clients/saml_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/saml_clients/saml_client_factory.py` & `sym_cli-0.5.1/sym/cli/saml_clients/saml_client_factory.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/conftest.py` & `sym_cli-0.5.1/sym/cli/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/test_ansible.py` & `sym_cli-0.5.1/sym/cli/tests/commands/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/test_host_to_instance.py` & `sym_cli-0.5.1/sym/cli/tests/commands/test_host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/test_ssh.py` & `sym_cli-0.5.1/sym/cli/tests/commands/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/test_ssh_session.py` & `sym_cli-0.5.1/sym/cli/tests/commands/test_ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/commands/test_write_creds.py` & `sym_cli-0.5.1/sym/cli/tests/commands/test_write_creds.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/conftest.py` & `sym_cli-0.5.1/sym/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/decorators/test_intercept_error.py` & `sym_cli-0.5.1/sym/cli/tests/decorators/test_intercept_error.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/decorators/test_setup_sentry.py` & `sym_cli-0.5.1/sym/cli/tests/decorators/test_setup_sentry.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/conftest.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/ec2/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_caching.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_caching.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_client.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_multiregion.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/ec2/test_multiregion.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/sandbox.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/sandbox.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_ansible.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_boto.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_boto.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_config.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_has_command.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_has_command.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_params.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_params.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/helpers/test_ssh.py` & `sym_cli-0.5.1/sym/cli/tests/helpers/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/integration/conftest.py` & `sym_cli-0.5.1/sym/cli/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/integration/test_ld.py` & `sym_cli-0.5.1/sym/cli/tests/integration/test_ld.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/matchers.py` & `sym_cli-0.5.1/sym/cli/tests/matchers.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/conftest.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_okta.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/test_aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_profile.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/test_aws_profile.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_chooser.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/test_chooser.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml2aws.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/test_saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml_client.py` & `sym_cli-0.5.1/sym/cli/tests/saml_clients/test_saml_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/sym/cli/tests/test_sym.py` & `sym_cli-0.5.1/sym/cli/tests/test_sym.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.5.0/PKG-INFO` & `sym_cli-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sym's Official CLI for Users
 Home-page: https://symops.com/
 Author: SymOps, Inc.
 Author-email: pypi@symops.io
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


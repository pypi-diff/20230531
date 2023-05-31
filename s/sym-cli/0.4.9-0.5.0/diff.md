# Comparing `tmp/sym-cli-0.4.9.tar.gz` & `tmp/sym_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym-cli-0.4.9.tar", max compression
+gzip compressed data, was "sym_cli-0.5.0.tar", max compression
```

## Comparing `sym-cli-0.4.9.tar` & `sym_cli-0.5.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0      147 2023-01-24 15:28:52.206332 sym-cli-0.4.9/DESCRIPTION.md
--rw-r--r--   0        0        0     2054 2023-01-24 15:35:56.565781 sym-cli-0.4.9/pyproject.toml
--rw-r--r--   0        0        0       60 2023-01-24 15:28:52.217312 sym-cli-0.4.9/sym/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.217558 sym-cli-0.4.9/sym/cli/actions/__init__.py
--rw-r--r--   0        0        0     2175 2023-01-24 15:28:52.217790 sym-cli-0.4.9/sym/cli/actions/action_registry.py
--rw-r--r--   0        0        0     1463 2023-01-24 15:28:52.218048 sym-cli-0.4.9/sym/cli/actions/ansible_action.py
--rw-r--r--   0        0        0     1614 2023-01-24 15:28:52.218347 sym-cli-0.4.9/sym/cli/actions/ansible_playbook_action.py
--rw-r--r--   0        0        0     1438 2023-01-24 15:28:52.218641 sym-cli-0.4.9/sym/cli/actions/ssh_session_action.py
--rw-r--r--   0        0        0     1299 2023-01-24 15:28:52.218915 sym-cli-0.4.9/sym/cli/actions/sym_action.py
--rw-r--r--   0        0        0     1675 2023-01-24 15:28:52.219184 sym-cli-0.4.9/sym/cli/actions/write_creds_action.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.219481 sym-cli-0.4.9/sym/cli/ansible/__init__.py
--rw-r--r--   0        0        0    18609 2023-01-24 15:28:52.219911 sym-cli-0.4.9/sym/cli/ansible/connection/__init__.py
--rw-r--r--   0        0        0    13652 2023-01-24 15:28:52.220327 sym-cli-0.4.9/sym/cli/ansible/connection/sym_aws_ssm.py
--rw-r--r--   0        0        0       90 2023-01-24 15:28:52.220674 sym-cli-0.4.9/sym/cli/commands/__init__.py
--rw-r--r--   0        0        0     1897 2023-01-24 15:28:52.220941 sym-cli-0.4.9/sym/cli/commands/ansible.py
--rw-r--r--   0        0        0     2179 2023-01-24 15:28:52.221226 sym-cli-0.4.9/sym/cli/commands/ansible_playbook.py
--rw-r--r--   0        0        0      664 2023-01-24 15:28:52.221511 sym-cli-0.4.9/sym/cli/commands/check.py
--rw-r--r--   0        0        0     2073 2023-01-24 15:28:52.221766 sym-cli-0.4.9/sym/cli/commands/config.py
--rw-r--r--   0        0        0     1016 2023-01-24 15:28:52.222047 sym-cli-0.4.9/sym/cli/commands/defaults.py
--rw-r--r--   0        0        0     3503 2023-01-24 15:28:52.222366 sym-cli-0.4.9/sym/cli/commands/doctor.py
--rw-r--r--   0        0        0      798 2023-01-24 15:28:52.222773 sym-cli-0.4.9/sym/cli/commands/exec.py
--rw-r--r--   0        0        0     1098 2023-01-24 15:28:52.223066 sym-cli-0.4.9/sym/cli/commands/host_to_instance.py
--rw-r--r--   0        0        0      683 2023-01-24 15:28:52.223333 sym-cli-0.4.9/sym/cli/commands/login.py
--rw-r--r--   0        0        0     1040 2023-01-24 15:28:52.223574 sym-cli-0.4.9/sym/cli/commands/resources.py
--rw-r--r--   0        0        0     7895 2023-01-24 15:28:52.223873 sym-cli-0.4.9/sym/cli/commands/ssh.py
--rw-r--r--   0        0        0     1224 2023-01-24 15:28:52.224117 sym-cli-0.4.9/sym/cli/commands/ssh_session.py
--rw-r--r--   0        0        0     1767 2023-01-24 15:28:52.224368 sym-cli-0.4.9/sym/cli/commands/ssh_tunnel.py
--rw-r--r--   0        0        0      894 2023-01-24 15:28:52.224614 sym-cli-0.4.9/sym/cli/commands/ssm.py
--rw-r--r--   0        0        0     2750 2023-01-24 15:28:52.224863 sym-cli-0.4.9/sym/cli/commands/sym.py
--rw-r--r--   0        0        0      204 2023-01-24 15:28:52.225232 sym-cli-0.4.9/sym/cli/commands/version.py
--rw-r--r--   0        0        0     1894 2023-01-24 15:28:52.225552 sym-cli-0.4.9/sym/cli/commands/write_creds.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.225889 sym-cli-0.4.9/sym/cli/constants/__init__.py
--rw-r--r--   0        0        0      746 2023-01-24 15:28:52.226132 sym-cli-0.4.9/sym/cli/constants/env.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.226395 sym-cli-0.4.9/sym/cli/data/__init__.py
--rw-r--r--   0        0        0      310 2023-01-24 15:28:52.226598 sym-cli-0.4.9/sym/cli/data/ansible_options.py
--rw-r--r--   0        0        0     1376 2023-01-24 15:28:52.226869 sym-cli-0.4.9/sym/cli/data/request_data.py
--rw-r--r--   0        0        0      142 2023-01-24 15:28:52.227131 sym-cli-0.4.9/sym/cli/data/target_options.py
--rw-r--r--   0        0        0     5000 2023-01-24 15:28:52.227505 sym-cli-0.4.9/sym/cli/decorators.py
--rw-r--r--   0        0        0     5573 2023-01-24 15:28:52.227796 sym-cli-0.4.9/sym/cli/errors.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.228027 sym-cli-0.4.9/sym/cli/helpers/__init__.py
--rw-r--r--   0        0        0     6376 2023-01-24 15:28:52.228280 sym-cli-0.4.9/sym/cli/helpers/ansible.py
--rw-r--r--   0        0        0     4949 2023-01-24 15:28:52.228559 sym-cli-0.4.9/sym/cli/helpers/boto.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.228791 sym-cli-0.4.9/sym/cli/helpers/check/__init__.py
--rw-r--r--   0        0        0     1614 2023-01-24 15:28:52.229002 sym-cli-0.4.9/sym/cli/helpers/check/core.py
--rw-r--r--   0        0        0     1827 2023-01-24 15:28:52.229260 sym-cli-0.4.9/sym/cli/helpers/check/ec2.py
--rw-r--r--   0        0        0     1088 2023-01-24 15:28:52.229488 sym-cli-0.4.9/sym/cli/helpers/check/model.py
--rw-r--r--   0        0        0     1694 2023-01-24 15:28:52.229731 sym-cli-0.4.9/sym/cli/helpers/check/runner.py
--rw-r--r--   0        0        0     2202 2023-01-24 15:28:52.229995 sym-cli-0.4.9/sym/cli/helpers/check/ssh.py
--rw-r--r--   0        0        0     3938 2023-01-24 15:28:52.230239 sym-cli-0.4.9/sym/cli/helpers/config.py
--rw-r--r--   0        0        0      626 2023-01-24 15:28:52.230469 sym-cli-0.4.9/sym/cli/helpers/constants.py
--rw-r--r--   0        0        0     8538 2023-01-24 15:28:52.230731 sym-cli-0.4.9/sym/cli/helpers/doctor.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.230947 sym-cli-0.4.9/sym/cli/helpers/ec2/__init__.py
--rw-r--r--   0        0        0     2086 2023-01-24 15:28:52.231194 sym-cli-0.4.9/sym/cli/helpers/ec2/cache.py
--rw-r--r--   0        0        0     7538 2023-01-24 15:28:52.231470 sym-cli-0.4.9/sym/cli/helpers/ec2/client.py
--rw-r--r--   0        0        0      214 2023-01-24 15:28:52.231750 sym-cli-0.4.9/sym/cli/helpers/ec2/factory.py
--rw-r--r--   0        0        0     2867 2023-01-24 15:28:52.232042 sym-cli-0.4.9/sym/cli/helpers/ec2/multiregion.py
--rw-r--r--   0        0        0      912 2023-01-24 15:28:52.232326 sym-cli-0.4.9/sym/cli/helpers/global_options.py
--rw-r--r--   0        0        0     4865 2023-01-24 15:28:52.232623 sym-cli-0.4.9/sym/cli/helpers/options.py
--rw-r--r--   0        0        0      287 2023-01-24 15:28:52.232886 sym-cli-0.4.9/sym/cli/helpers/org.py
--rw-r--r--   0        0        0     9485 2023-01-24 15:28:52.233224 sym-cli-0.4.9/sym/cli/helpers/params.py
--rw-r--r--   0        0        0      946 2023-01-24 15:28:52.233486 sym-cli-0.4.9/sym/cli/helpers/pty.py
--rw-r--r--   0        0        0    10719 2023-01-24 15:28:52.233817 sym-cli-0.4.9/sym/cli/helpers/ssh.py
--rw-r--r--   0        0        0     1543 2023-01-24 15:28:52.234105 sym-cli-0.4.9/sym/cli/helpers/sym_group.py
--rw-r--r--   0        0        0      812 2023-01-24 15:28:52.234399 sym-cli-0.4.9/sym/cli/helpers/threading.py
--rw-r--r--   0        0        0      262 2023-01-24 15:28:52.234648 sym-cli-0.4.9/sym/cli/helpers/validations.py
--rw-r--r--   0        0        0     1722 2023-01-24 15:28:52.234926 sym-cli-0.4.9/sym/cli/helpers/version.py
--rw-r--r--   0        0        0       90 2023-01-24 15:28:52.235358 sym-cli-0.4.9/sym/cli/saml_clients/__init__.py
--rw-r--r--   0        0        0     5733 2023-01-24 15:28:52.235646 sym-cli-0.4.9/sym/cli/saml_clients/aws_okta.py
--rw-r--r--   0        0        0     2681 2023-01-24 15:28:52.235887 sym-cli-0.4.9/sym/cli/saml_clients/aws_profile.py
--rw-r--r--   0        0        0     1140 2023-01-24 15:28:52.236119 sym-cli-0.4.9/sym/cli/saml_clients/chooser.py
--rw-r--r--   0        0        0     6699 2023-01-24 15:28:52.236374 sym-cli-0.4.9/sym/cli/saml_clients/saml2aws.py
--rw-r--r--   0        0        0     8989 2023-01-24 15:28:52.236647 sym-cli-0.4.9/sym/cli/saml_clients/saml_client.py
--rw-r--r--   0        0        0     1247 2023-01-24 15:28:52.236889 sym-cli-0.4.9/sym/cli/saml_clients/saml_client_factory.py
--rw-r--r--   0        0        0      277 2023-01-24 15:28:52.237157 sym-cli-0.4.9/sym/cli/sym.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.237452 sym-cli-0.4.9/sym/cli/tests/__init__.py
--rw-r--r--   0        0        0     3834 2023-01-24 15:28:52.237803 sym-cli-0.4.9/sym/cli/tests/commands/conftest.py
--rw-r--r--   0        0        0    10471 2023-01-24 15:28:52.238117 sym-cli-0.4.9/sym/cli/tests/commands/test_ansible.py
--rw-r--r--   0        0        0      677 2023-01-24 15:28:52.238400 sym-cli-0.4.9/sym/cli/tests/commands/test_host_to_instance.py
--rw-r--r--   0        0        0     6642 2023-01-24 15:28:52.238773 sym-cli-0.4.9/sym/cli/tests/commands/test_ssh.py
--rw-r--r--   0        0        0     1685 2023-01-24 15:28:52.239043 sym-cli-0.4.9/sym/cli/tests/commands/test_ssh_session.py
--rw-r--r--   0        0        0    11563 2023-01-24 15:28:52.239375 sym-cli-0.4.9/sym/cli/tests/commands/test_write_creds.py
--rw-r--r--   0        0        0     4423 2023-01-24 15:28:52.239658 sym-cli-0.4.9/sym/cli/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.239975 sym-cli-0.4.9/sym/cli/tests/decorators/__init__.py
--rw-r--r--   0        0        0      635 2023-01-24 15:28:52.240244 sym-cli-0.4.9/sym/cli/tests/decorators/test_intercept_error.py
--rw-r--r--   0        0        0      425 2023-01-24 15:28:52.240490 sym-cli-0.4.9/sym/cli/tests/decorators/test_retry.py
--rw-r--r--   0        0        0     1108 2023-01-24 15:28:52.240754 sym-cli-0.4.9/sym/cli/tests/decorators/test_setup_sentry.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.241002 sym-cli-0.4.9/sym/cli/tests/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.241207 sym-cli-0.4.9/sym/cli/tests/helpers/ec2/__init__.py
--rw-r--r--   0        0        0      957 2023-01-24 15:28:52.241432 sym-cli-0.4.9/sym/cli/tests/helpers/ec2/conftest.py
--rw-r--r--   0        0        0     3642 2023-01-24 15:28:52.241777 sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_caching.py
--rw-r--r--   0        0        0     6985 2023-01-24 15:28:52.242071 sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_client.py
--rw-r--r--   0        0        0     2084 2023-01-24 15:28:52.242355 sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_multiregion.py
--rw-r--r--   0        0        0      846 2023-01-24 15:28:52.242628 sym-cli-0.4.9/sym/cli/tests/helpers/sandbox.py
--rw-r--r--   0        0        0     1702 2023-01-24 15:28:52.242945 sym-cli-0.4.9/sym/cli/tests/helpers/test_ansible.py
--rw-r--r--   0        0        0     2383 2023-01-24 15:28:52.243242 sym-cli-0.4.9/sym/cli/tests/helpers/test_boto.py
--rw-r--r--   0        0        0     3087 2023-01-24 15:28:52.243502 sym-cli-0.4.9/sym/cli/tests/helpers/test_config.py
--rw-r--r--   0        0        0      581 2023-01-24 15:28:52.243762 sym-cli-0.4.9/sym/cli/tests/helpers/test_has_command.py
--rw-r--r--   0        0        0      563 2023-01-24 15:28:52.244047 sym-cli-0.4.9/sym/cli/tests/helpers/test_params.py
--rw-r--r--   0        0        0     2786 2023-01-24 15:28:52.244360 sym-cli-0.4.9/sym/cli/tests/helpers/test_ssh.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.244622 sym-cli-0.4.9/sym/cli/tests/helpers/updater/__init__.py
--rw-r--r--   0        0        0     2934 2023-01-24 15:28:52.244849 sym-cli-0.4.9/sym/cli/tests/helpers/updater/conftest.py
--rw-r--r--   0        0        0   267688 2023-01-24 15:28:52.246986 sym-cli-0.4.9/sym/cli/tests/helpers/updater/responses/sym-cli-0.2.7.json
--rw-r--r--   0        0        0   267688 2023-01-24 15:28:52.248075 sym-cli-0.4.9/sym/cli/tests/helpers/updater/responses/sym-cli.json
--rw-r--r--   0        0        0     5329 2023-01-24 15:28:52.248402 sym-cli-0.4.9/sym/cli/tests/helpers/updater/test_updater.py
--rw-r--r--   0        0        0     1497 2023-01-24 15:28:52.248808 sym-cli-0.4.9/sym/cli/tests/integration/conftest.py
--rw-r--r--   0        0        0     2832 2023-01-24 15:28:52.249062 sym-cli-0.4.9/sym/cli/tests/integration/test_ld.py
--rw-r--r--   0        0        0      944 2023-01-24 15:28:52.249295 sym-cli-0.4.9/sym/cli/tests/matchers.py
--rw-r--r--   0        0        0        0 2023-01-24 15:28:52.249550 sym-cli-0.4.9/sym/cli/tests/saml_clients/__init__.py
--rw-r--r--   0        0        0     3886 2023-01-24 15:28:52.249771 sym-cli-0.4.9/sym/cli/tests/saml_clients/conftest.py
--rw-r--r--   0        0        0     2187 2023-01-24 15:28:52.250093 sym-cli-0.4.9/sym/cli/tests/saml_clients/test_aws_okta.py
--rw-r--r--   0        0        0     1224 2023-01-24 15:28:52.250405 sym-cli-0.4.9/sym/cli/tests/saml_clients/test_aws_profile.py
--rw-r--r--   0        0        0     1365 2023-01-24 15:28:52.250754 sym-cli-0.4.9/sym/cli/tests/saml_clients/test_chooser.py
--rw-r--r--   0        0        0     3722 2023-01-24 15:28:52.251050 sym-cli-0.4.9/sym/cli/tests/saml_clients/test_saml2aws.py
--rw-r--r--   0        0        0     1333 2023-01-24 15:28:52.251351 sym-cli-0.4.9/sym/cli/tests/saml_clients/test_saml_client.py
--rw-r--r--   0        0        0     3730 2023-01-24 15:28:52.251671 sym-cli-0.4.9/sym/cli/tests/test_sym.py
--rw-r--r--   0        0        0       22 2023-01-24 15:35:56.604803 sym-cli-0.4.9/sym/cli/version.py
--rw-r--r--   0        0        0     1803 2023-01-24 15:35:58.205270 sym-cli-0.4.9/setup.py
--rw-r--r--   0        0        0     1509 2023-01-24 15:35:58.205743 sym-cli-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-05-31 14:20:47.903977 sym_cli-0.5.0/DESCRIPTION.md
+-rw-r--r--   0        0        0     2054 2023-05-31 14:20:49.647979 sym_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/__init__.py
+-rw-r--r--   0        0        0     2175 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/action_registry.py
+-rw-r--r--   0        0        0     1463 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ansible_action.py
+-rw-r--r--   0        0        0     1614 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ansible_playbook_action.py
+-rw-r--r--   0        0        0     1438 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/ssh_session_action.py
+-rw-r--r--   0        0        0     1299 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/sym_action.py
+-rw-r--r--   0        0        0     1675 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/actions/write_creds_action.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/__init__.py
+-rw-r--r--   0        0        0    18609 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/connection/__init__.py
+-rw-r--r--   0        0        0    13933 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/ansible/connection/sym_aws_ssm.py
+-rw-r--r--   0        0        0       90 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1897 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ansible.py
+-rw-r--r--   0        0        0     2179 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ansible_playbook.py
+-rw-r--r--   0        0        0      664 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/check.py
+-rw-r--r--   0        0        0     2073 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/config.py
+-rw-r--r--   0        0        0     1016 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/defaults.py
+-rw-r--r--   0        0        0     3503 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/doctor.py
+-rw-r--r--   0        0        0      798 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/exec.py
+-rw-r--r--   0        0        0     1098 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/host_to_instance.py
+-rw-r--r--   0        0        0      683 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/login.py
+-rw-r--r--   0        0        0     1040 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/resources.py
+-rw-r--r--   0        0        0     7895 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh.py
+-rw-r--r--   0        0        0     1224 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh_session.py
+-rw-r--r--   0        0        0     1767 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssh_tunnel.py
+-rw-r--r--   0        0        0      894 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/ssm.py
+-rw-r--r--   0        0        0     2750 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/sym.py
+-rw-r--r--   0        0        0      204 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/version.py
+-rw-r--r--   0        0        0     1894 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/commands/write_creds.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/constants/__init__.py
+-rw-r--r--   0        0        0      746 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/constants/env.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/ansible_options.py
+-rw-r--r--   0        0        0     1376 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/request_data.py
+-rw-r--r--   0        0        0      142 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/data/target_options.py
+-rw-r--r--   0        0        0     5000 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/decorators.py
+-rw-r--r--   0        0        0     5573 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/errors.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     6376 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ansible.py
+-rw-r--r--   0        0        0     5142 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/boto.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/__init__.py
+-rw-r--r--   0        0        0     1614 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/core.py
+-rw-r--r--   0        0        0     1827 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/ec2.py
+-rw-r--r--   0        0        0     1088 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/model.py
+-rw-r--r--   0        0        0     1694 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/runner.py
+-rw-r--r--   0        0        0     2202 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/check/ssh.py
+-rw-r--r--   0        0        0     3938 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/config.py
+-rw-r--r--   0        0        0      626 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/constants.py
+-rw-r--r--   0        0        0     8538 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/doctor.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0     2086 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/cache.py
+-rw-r--r--   0        0        0     7538 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/client.py
+-rw-r--r--   0        0        0      214 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/factory.py
+-rw-r--r--   0        0        0     2867 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/ec2/multiregion.py
+-rw-r--r--   0        0        0      912 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/global_options.py
+-rw-r--r--   0        0        0     4865 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/options.py
+-rw-r--r--   0        0        0      287 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/org.py
+-rw-r--r--   0        0        0     8756 2023-05-31 14:20:47.911977 sym_cli-0.5.0/sym/cli/helpers/params.py
+-rw-r--r--   0        0        0      946 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/pty.py
+-rw-r--r--   0        0        0    10719 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/ssh.py
+-rw-r--r--   0        0        0     1543 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/sym_group.py
+-rw-r--r--   0        0        0      812 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/threading.py
+-rw-r--r--   0        0        0      262 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/validations.py
+-rw-r--r--   0        0        0     1722 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/helpers/version.py
+-rw-r--r--   0        0        0       90 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3256 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_config.py
+-rw-r--r--   0        0        0     5733 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_okta.py
+-rw-r--r--   0        0        0     2887 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/aws_profile.py
+-rw-r--r--   0        0        0     1168 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/chooser.py
+-rw-r--r--   0        0        0     6699 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml2aws.py
+-rw-r--r--   0        0        0     8989 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml_client.py
+-rw-r--r--   0        0        0     1247 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/saml_clients/saml_client_factory.py
+-rw-r--r--   0        0        0      277 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/sym.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/__init__.py
+-rw-r--r--   0        0        0     3834 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/conftest.py
+-rw-r--r--   0        0        0    10471 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ansible.py
+-rw-r--r--   0        0        0      677 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_host_to_instance.py
+-rw-r--r--   0        0        0     6642 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ssh.py
+-rw-r--r--   0        0        0     1685 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_ssh_session.py
+-rw-r--r--   0        0        0    11563 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/commands/test_write_creds.py
+-rw-r--r--   0        0        0     4423 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/__init__.py
+-rw-r--r--   0        0        0      635 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_intercept_error.py
+-rw-r--r--   0        0        0      425 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_retry.py
+-rw-r--r--   0        0        0     1108 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/decorators/test_setup_sentry.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/conftest.py
+-rw-r--r--   0        0        0     3642 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_caching.py
+-rw-r--r--   0        0        0     6985 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_client.py
+-rw-r--r--   0        0        0     2084 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_multiregion.py
+-rw-r--r--   0        0        0      846 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/sandbox.py
+-rw-r--r--   0        0        0     1702 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_ansible.py
+-rw-r--r--   0        0        0     2383 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_boto.py
+-rw-r--r--   0        0        0     3087 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_config.py
+-rw-r--r--   0        0        0      581 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_has_command.py
+-rw-r--r--   0        0        0      563 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_params.py
+-rw-r--r--   0        0        0     2786 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/test_ssh.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/conftest.py
+-rw-r--r--   0        0        0   267688 2023-05-31 14:20:47.915977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli-0.2.7.json
+-rw-r--r--   0        0        0   267688 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli.json
+-rw-r--r--   0        0        0     5329 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/helpers/updater/test_updater.py
+-rw-r--r--   0        0        0     1497 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2832 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/integration/test_ld.py
+-rw-r--r--   0        0        0      944 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/matchers.py
+-rw-r--r--   0        0        0        0 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/conftest.py
+-rw-r--r--   0        0        0     2187 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_okta.py
+-rw-r--r--   0        0        0     1224 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_profile.py
+-rw-r--r--   0        0        0     1365 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_chooser.py
+-rw-r--r--   0        0        0     3722 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml2aws.py
+-rw-r--r--   0        0        0     1333 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml_client.py
+-rw-r--r--   0        0        0     3730 2023-05-31 14:20:47.919977 sym_cli-0.5.0/sym/cli/tests/test_sym.py
+-rw-r--r--   0        0        0       22 2023-05-31 14:20:49.695979 sym_cli-0.5.0/sym/cli/version.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 sym_cli-0.5.0/PKG-INFO
```

### Comparing `sym-cli-0.4.9/pyproject.toml` & `sym_cli-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-cli"
-version = "0.4.9"
+version = "0.5.0"
 description = "Sym's Official CLI for Users"
 authors = ["SymOps, Inc. <pypi@symops.io>"]
 packages = [{ include = "sym/*" }]
 readme = "DESCRIPTION.md"
 homepage = "https://symops.com/"
 documentation = "https://docs.symops.com/docs/install-sym-cli"
 classifiers = [
```

### Comparing `sym-cli-0.4.9/sym/cli/actions/action_registry.py` & `sym_cli-0.5.0/sym/cli/actions/action_registry.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/actions/ansible_action.py` & `sym_cli-0.5.0/sym/cli/actions/ansible_action.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/actions/ansible_playbook_action.py` & `sym_cli-0.5.0/sym/cli/actions/ansible_playbook_action.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/actions/ssh_session_action.py` & `sym_cli-0.5.0/sym/cli/actions/ssh_session_action.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/actions/sym_action.py` & `sym_cli-0.5.0/sym/cli/actions/sym_action.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/actions/write_creds_action.py` & `sym_cli-0.5.0/sym/cli/actions/write_creds_action.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/ansible/connection/__init__.py` & `sym_cli-0.5.0/sym/cli/ansible/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/ansible/connection/sym_aws_ssm.py` & `sym_cli-0.5.0/sym/cli/ansible/connection/sym_aws_ssm.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 import boto3
 from ansible.errors import AnsibleConnectionFailure, AnsibleError, AnsibleFileNotFound
 from ansible.module_utils._text import to_bytes, to_native, to_text
 from ansible.module_utils.six.moves import xrange
 from ansible.plugins.connection import ConnectionBase
 from ansible.utils.display import Display
+from botocore.client import Config
 
 URL_TTL = 3600
 CHUNK_SIZE = 1024
 MAX_DELAY = 30
 START_COMMAND = "SYM_COMMAND_START"
 END_COMMAND = "SYM_COMMAND_END"
 
@@ -230,15 +231,18 @@
         # Disable command echo and prompt
         self._process.stdin.write(to_bytes("stty -echo\n" + "PS1=''\n"))
 
     def start_ssm_session(self):
         instance_meta = self._get_instance_meta()
         self.instance_id = instance_meta["instance"]
 
-        self._s3_client = self._get_boto_client("s3")
+        self._s3_client = self._get_boto_client("s3",
+                                                region=instance_meta["region"],
+                                                config=Config(signature_version='s3v4')
+                                                )
         self._ssm_client = self._get_boto_client("ssm", region=instance_meta["region"])
 
         display.vvv(
             u"ESTABLISH SSM CONNECTION TO: {0}".format(self.instance_id),
             host=self.host,
         )
 
@@ -334,19 +338,19 @@
                 display.vvvv(u"EXEC end: {0}".format(line), host=self.host)
                 return (returncode, stdout, self._flush_stderr())
 
             stdout = stdout + line
 
         return (self._process.returncode, stdout, self._flush_stderr())
 
-    def _get_boto_client(self, service, region=None):
+    def _get_boto_client(self, service, region=None, config=None):
         return boto3.Session(
             profile_name=self.get_option("profile"),
             region_name=region or self.get_option("region"),
-        ).client(service)
+        ).client(service, config=config)
 
     def _get_url(self, action, key, http_method):
         return self._s3_client.generate_presigned_url(
             action,
             Params={"Bucket": self.get_option("bucket"), "Key": key},
             ExpiresIn=URL_TTL,
             HttpMethod=http_method,
```

### Comparing `sym-cli-0.4.9/sym/cli/commands/ansible.py` & `sym_cli-0.5.0/sym/cli/commands/ansible.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/ansible_playbook.py` & `sym_cli-0.5.0/sym/cli/commands/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/check.py` & `sym_cli-0.5.0/sym/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/config.py` & `sym_cli-0.5.0/sym/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/defaults.py` & `sym_cli-0.5.0/sym/cli/commands/defaults.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/doctor.py` & `sym_cli-0.5.0/sym/cli/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/exec.py` & `sym_cli-0.5.0/sym/cli/commands/exec.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/host_to_instance.py` & `sym_cli-0.5.0/sym/cli/commands/host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/login.py` & `sym_cli-0.5.0/sym/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/resources.py` & `sym_cli-0.5.0/sym/cli/commands/resources.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/ssh.py` & `sym_cli-0.5.0/sym/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/ssh_session.py` & `sym_cli-0.5.0/sym/cli/commands/ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/ssh_tunnel.py` & `sym_cli-0.5.0/sym/cli/commands/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/ssm.py` & `sym_cli-0.5.0/sym/cli/commands/ssm.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/sym.py` & `sym_cli-0.5.0/sym/cli/commands/sym.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/commands/write_creds.py` & `sym_cli-0.5.0/sym/cli/commands/write_creds.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/constants/env.py` & `sym_cli-0.5.0/sym/cli/constants/env.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/data/request_data.py` & `sym_cli-0.5.0/sym/cli/data/request_data.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/decorators.py` & `sym_cli-0.5.0/sym/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/errors.py` & `sym_cli-0.5.0/sym/cli/errors.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/ansible.py` & `sym_cli-0.5.0/sym/cli/helpers/ansible.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/boto.py` & `sym_cli-0.5.0/sym/cli/helpers/boto.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,24 @@
         RequestExpired: ExpiredCredentials,
     }
 )
 
 
 def boto_client(saml_client, service):
     creds = saml_client.get_creds()
-    return boto3.client(
-        service,
-        config=BotoConfig(region_name=get_region(saml_client, creds)),
-        aws_access_key_id=creds["AWS_ACCESS_KEY_ID"],
-        aws_secret_access_key=creds["AWS_SECRET_ACCESS_KEY"],
-        aws_session_token=creds.get("AWS_SESSION_TOKEN"),
-    )
+    if access_key_id := creds.get("AWS_ACCESS_KEY_ID"):
+        return boto3.client(
+            service,
+            config=BotoConfig(region_name=get_region(saml_client, creds)),
+            aws_access_key_id=access_key_id,
+            aws_secret_access_key=creds["AWS_SECRET_ACCESS_KEY"],
+            aws_session_token=creds.get("AWS_SESSION_TOKEN"),
+        )
+    # If there is no access key id, then assume that the boto3 default session is set up
+    return boto3.client(service)
 
 
 def get_region(saml_client, creds=None) -> str:
     override = saml_client.options.aws_region
     return override or (creds or saml_client.get_creds()).get("AWS_REGION")
```

### Comparing `sym-cli-0.4.9/sym/cli/helpers/check/core.py` & `sym_cli-0.5.0/sym/cli/helpers/check/core.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/check/ec2.py` & `sym_cli-0.5.0/sym/cli/helpers/check/ec2.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/check/model.py` & `sym_cli-0.5.0/sym/cli/helpers/check/model.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/check/runner.py` & `sym_cli-0.5.0/sym/cli/helpers/check/runner.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/check/ssh.py` & `sym_cli-0.5.0/sym/cli/helpers/check/ssh.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/config.py` & `sym_cli-0.5.0/sym/cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/constants.py` & `sym_cli-0.5.0/sym/cli/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/doctor.py` & `sym_cli-0.5.0/sym/cli/helpers/doctor.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/ec2/cache.py` & `sym_cli-0.5.0/sym/cli/helpers/ec2/cache.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/ec2/client.py` & `sym_cli-0.5.0/sym/cli/helpers/ec2/client.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/ec2/multiregion.py` & `sym_cli-0.5.0/sym/cli/helpers/ec2/multiregion.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/global_options.py` & `sym_cli-0.5.0/sym/cli/helpers/global_options.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/options.py` & `sym_cli-0.5.0/sym/cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/params.py` & `sym_cli-0.5.0/sym/cli/helpers/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,35 +177,14 @@
                 region="us-east-1",
                 arn="arn:aws:iam::838419636750:role/SSMTestRoleCustomBucket",
                 ansible_bucket="sym-ansible-dev",
                 aliases=["test_custom", "test_custom2"],
             ),
         },
     },
-    "healthy-health": {
-        "resource_env_var": "ENVIRONMENT",
-        "users": {"ssh": "ubuntu"},
-        "domain": "healthy-health.co",
-        "aws_saml_url": (
-            "https://healthy-health.okta.com/home/amazon_aws/0oagrj7yFaVtJoI2N5d5/272"
-        ),
-        "aws_okta_params": {
-            "mfa_provider": "OKTA",
-            "assume_role_ttl": "1h",
-            "session_ttl": "30m",
-        },
-        "saml2aws_params": {"mfa": "Auto", "aws_session_duration": "1800"},
-        "profiles": {
-            "prod": Profile(
-                display_name="Prod",
-                region="us-east-1",
-                arn="arn:aws:iam::223440862848:role/ssm-healthy-health-user-prod",
-            ),
-        },
-    },
 }
 
 
 def get_org_params() -> OrgParams:
     return PARAMS[Config.get_org()]
```

### Comparing `sym-cli-0.4.9/sym/cli/helpers/pty.py` & `sym_cli-0.5.0/sym/cli/helpers/pty.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/ssh.py` & `sym_cli-0.5.0/sym/cli/helpers/ssh.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/sym_group.py` & `sym_cli-0.5.0/sym/cli/helpers/sym_group.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/threading.py` & `sym_cli-0.5.0/sym/cli/helpers/threading.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/helpers/version.py` & `sym_cli-0.5.0/sym/cli/helpers/version.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/aws_okta.py` & `sym_cli-0.5.0/sym/cli/saml_clients/aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/aws_profile.py` & `sym_cli-0.5.0/sym/cli/saml_clients/aws_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from ..helpers.params import Profile
 from .saml_client import SAMLClient
 
 AwsCredentialsPath = Path(
     os.getenv("AWS_CREDENTIAL_FILE", Path.home() / ".aws" / "credentials")
 )
 
-
+# This client assumes that access key and secret are defined in the credentials file.
+# If you want to use a named profile that works with SSO or some other supported AWS credential
+# process, use AwsConfig
 class AwsProfile(SAMLClient):
     binary = "aws"
     option_value = "aws-profile"
     priority = 0
     setup_help = f"Set up your profile in `{str(AwsCredentialsPath)}`."
 
     resource: str
```

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/chooser.py` & `sym_cli-0.5.0/sym/cli/saml_clients/chooser.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from sym.shared.cli.helpers.os import has_command
 from sym.shared.cli.helpers.util import requires_all_imports
 
 from ..errors import SAMLClientNotFound
 from . import import_all
 from .saml_client import SAMLClient
 
-SAMLClientName = Literal["auto", "aws-okta", "saml2aws", "aws-profile"]
-AUTO_EXCLUDED_SAML_CLIENT_NAMES = ["aws-profile"]
+SAMLClientName = Literal["auto", "aws-okta", "saml2aws", "aws-profile", "aws-config"]
+AUTO_EXCLUDED_SAML_CLIENT_NAMES = ["aws-profile", "aws-config"]
 
 
 @requires_all_imports(import_all)
 def option_values():
     return ["auto"] + [x.option_value for x in SAMLClient.sorted_subclasses()]
```

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/saml2aws.py` & `sym_cli-0.5.0/sym/cli/saml_clients/saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/saml_client.py` & `sym_cli-0.5.0/sym/cli/saml_clients/saml_client.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/saml_clients/saml_client_factory.py` & `sym_cli-0.5.0/sym/cli/saml_clients/saml_client_factory.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/test_ansible.py` & `sym_cli-0.5.0/sym/cli/tests/commands/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/test_host_to_instance.py` & `sym_cli-0.5.0/sym/cli/tests/commands/test_host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/test_ssh.py` & `sym_cli-0.5.0/sym/cli/tests/commands/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/test_ssh_session.py` & `sym_cli-0.5.0/sym/cli/tests/commands/test_ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/commands/test_write_creds.py` & `sym_cli-0.5.0/sym/cli/tests/commands/test_write_creds.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/decorators/test_intercept_error.py` & `sym_cli-0.5.0/sym/cli/tests/decorators/test_intercept_error.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/decorators/test_setup_sentry.py` & `sym_cli-0.5.0/sym/cli/tests/decorators/test_setup_sentry.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/ec2/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_caching.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_caching.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_client.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def test_get_regions_boto_error_fallback(ec2_stub, ec2_client: Ec2Client):
     ec2_stub.add_client_error(
         "describe_regions",
         service_message="Error describing regions",
         http_status_code=400,
     )
     regions = ec2_client.get_regions()
-    assert len(regions) == 26
+    assert len(regions) == 27
     assert "us-east-1" in regions
 
 
 def test_load_instance_by_id(ec2_stub, ec2_client: Ec2Client):
     ec2_stub.add_response(
         "describe_instances",
         BOTO_INSTANCE_RESPONSE,
```

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/ec2/test_multiregion.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/ec2/test_multiregion.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/sandbox.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/sandbox.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_ansible.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_boto.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_boto.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_config.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_config.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_has_command.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_has_command.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_params.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_params.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/test_ssh.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/updater/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/updater/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/updater/responses/sym-cli-0.2.7.json` & `sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli-0.2.7.json`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/updater/responses/sym-cli.json` & `sym_cli-0.5.0/sym/cli/tests/helpers/updater/responses/sym-cli.json`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/helpers/updater/test_updater.py` & `sym_cli-0.5.0/sym/cli/tests/helpers/updater/test_updater.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/integration/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/integration/test_ld.py` & `sym_cli-0.5.0/sym/cli/tests/integration/test_ld.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/matchers.py` & `sym_cli-0.5.0/sym/cli/tests/matchers.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/conftest.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/conftest.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/test_aws_okta.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/test_aws_profile.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_aws_profile.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/test_chooser.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_chooser.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/test_saml2aws.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/saml_clients/test_saml_client.py` & `sym_cli-0.5.0/sym/cli/tests/saml_clients/test_saml_client.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/sym/cli/tests/test_sym.py` & `sym_cli-0.5.0/sym/cli/tests/test_sym.py`

 * *Files identical despite different names*

### Comparing `sym-cli-0.4.9/PKG-INFO` & `sym_cli-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: sym-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: Sym's Official CLI for Users
 Home-page: https://symops.com/
 Author: SymOps, Inc.
 Author-email: pypi@symops.io
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: PyYAML (>=5.3.1,<6.0.0)
 Requires-Dist: SecretStorage (>=3.2.0,<4.0.0)
 Requires-Dist: analytics-python (>=1.3.1,<2.0.0)
 Requires-Dist: boto3 (>=1.16.20,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.1,<0.6.0)
 Requires-Dist: colorama (<0.4.4)
```


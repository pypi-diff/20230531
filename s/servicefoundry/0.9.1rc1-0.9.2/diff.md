# Comparing `tmp/servicefoundry-0.9.1rc1.tar.gz` & `tmp/servicefoundry-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.1rc1.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.2.tar", max compression
```

## Comparing `servicefoundry-0.9.1rc1.tar` & `servicefoundry-0.9.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      672 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/README.md
--rw-r--r--   0        0        0     2119 2023-05-26 13:01:30.985095 servicefoundry-0.9.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1315 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/__init__.py
--rw-r--r--   0        0        0    37574 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6480 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2795 2023-05-26 13:01:16.237064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3587 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3863 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2492 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23939 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5624 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9147 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-05-26 13:01:16.241064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-05-26 13:01:16.245064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5318 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-05-26 13:01:16.249064 servicefoundry-0.9.1rc1/servicefoundry/version.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-05-31 15:59:48.797209 servicefoundry-0.9.2/README.md
+-rw-r--r--   0        0        0     2116 2023-05-31 16:00:01.813432 servicefoundry-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1315 2023-05-31 15:59:48.797209 servicefoundry-0.9.2/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    38045 2023-05-31 15:59:48.797209 servicefoundry-0.9.2/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6496 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6480 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2795 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3587 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3863 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2492 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23939 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5624 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9147 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-05-31 15:59:48.801209 servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5318 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-05-31 15:59:48.805209 servicefoundry-0.9.2/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.2/PKG-INFO
```

### Comparing `servicefoundry-0.9.1rc1/README.md` & `servicefoundry-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/pyproject.toml` & `servicefoundry-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.1rc1"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.2"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/__init__.py` & `servicefoundry-0.9.2/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.2/servicefoundry/auto_gen/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-05-18T08:13:41+00:00
+#   timestamp: 2023-05-31T15:52:02+00:00
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, confloat, conint, constr
 from typing_extensions import Literal
 
 
 class BasicAuthCreds(BaseModel):
     """
@@ -25,15 +25,15 @@
         ...,
         description="+label=Password for service auth\n+message=Password should not be more than 64 characters\n+sort=2",
     )
 
 
 class BlueGreen(BaseModel):
     """
-        +docs=This strategy brings up the new release completely before switching the complete load to the new release.
+    +docs=This strategy brings up the new release completely before switching the complete load to the new release.
     This minimizes the time that two versions are serving traffic at the same time.
     +label=Blue Green strategy
     """
 
     type: Literal["blue_green"] = Field(..., description="+value=blue_green")
     enable_auto_promotion: bool = Field(
         False,
@@ -62,15 +62,15 @@
         30,
         description="+docs=Duration for which to pause the release. The release process will wait for these seconds before proceeding to the next step.\nIf this is not set, the step will pause indefinitely on this step\n+label=Pause duration\n+unit=seconds\n+placeholder=Duration",
     )
 
 
 class DockerFileBuild(BaseModel):
     """
-        +docs=Describes that we are using a dockerfile to build our image
+    +docs=Describes that we are using a dockerfile to build our image
     +label=Docker File (I already have Docker File)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^dockerfile$") = Field(..., description="+value=dockerfile")
     dockerfile_path: str = Field(
         "./Dockerfile",
@@ -84,15 +84,15 @@
         None,
         description="+label=Entrypoint Override\n+usage=Override the command to run when the container starts\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
 
 
 class GitSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a git repository to build our image
+    +docs=Describes that we are using code stored in a git repository to build our image
     +label=Git Source
     +icon=fa-solid fa-code-branch:black
     +sort=300
     """
 
     type: constr(regex=r"^git$") = Field(..., description="+value=git")
     repo_url: constr(
@@ -108,15 +108,15 @@
         None,
         description="+label=Branch Name\n+usage=Selecting branch will select latest commit SHA of the branch.\n+sort=3\n+ignore",
     )
 
 
 class HttpProbe(BaseModel):
     """
-        +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
+    +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +label=Instructions for assessing container health by executing an HTTP GET request.
     """
 
     type: constr(regex=r"^http$") = Field(..., description="+sort=1\n+value=http")
     path: str = Field(
         ...,
@@ -133,15 +133,15 @@
     scheme: str = Field(
         "HTTP", description="+sort=5\n+usage=Scheme to use for connecting to the host"
     )
 
 
 class HuggingfaceModelHub(BaseModel):
     """
-        +docs=Huggingface model hub (deploy a model from HF model hub)
+    +docs=Huggingface model hub (deploy a model from HF model hub)
     +label=Huggingface model hub
     +usage=Deploy a model from HF model hub
     """
 
     type: constr(regex=r"^hf-model-hub$") = Field(
         ..., description="+value=hf-model-hub"
     )
@@ -153,60 +153,71 @@
         None,
         description="+label=Pipeline\n+usage=Pipeline to use for inference. If not set, we will try to infer the `task` name for the given model.\nExamples:- `summarization`, `text-generation`, `text-classification`, etc.\nYou can read more about HF pipelines here:- https://huggingface.co/docs/transformers/pipeline_tutorial\nYou can find a list of tasks here:- https://huggingface.co/docs/transformers/v4.24.0/en/main_classes/pipelines#transformers.pipeline.task\n+placeholder=summarization",
     )
 
 
 class Image(BaseModel):
     """
-        +docs=Describes that we are using a pre-built image stored in a Docker Image registry
+    +docs=Describes that we are using a pre-built image stored in a Docker Image registry
     +label=Docker Image (Deploy an existing image)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^image$") = Field(..., description="+value=image")
-    image_uri: str = Field(
+    image_uri: constr(regex=r"^\S*$") = Field(
         ...,
         description="+label=Image URI\n+usage=The image URI. Specify the name of the image and the tag.\nIf the image is in Dockerhub, you can skip registry-url (for e.g. `tensorflow/tensorflow`).\nYou can use an image from a private registry using Advanced fields\n+placeholder=registry-url/account/image:version (e.g. docker.io/tensorflow/tensorflow)",
     )
     docker_registry: Optional[str] = Field(
         None,
         description="+docs=FQN of the container registry. You can the FQN of your desired container registry (or add one)\nin the  Integrations page[Integrations](https://app.truefoundry.tech/integrations?tab=docker-registry) page\n+label=Docker Registry\n+usage=FQN of the container registry. If you can't find your registry here,\nadd it through the [Integrations](/integrations?tab=docker-registry) page",
     )
     command: Optional[Union[str, List[str]]] = Field(
         None,
         description="+label=Entrypoint Override\n+usage=Override the command to run when container starts.\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
 
 
+class Kustomize(BaseModel):
+    patch: Optional[Dict[str, Any]] = Field(
+        None,
+        description="+label=Patch\n+usage=Content of kustomization.yaml to perform kustomize operation. Please do not include the `resources` section. It is filled in automatically",
+    )
+    additions: Optional[List[Dict[str, Any]]] = Field(
+        None,
+        description="+label=Additional Manifests\n+usage=Additional kubernetes manifests to be included in the application",
+    )
+
+
 class LocalSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a local developement environment to build our image
+    +docs=Describes that we are using code stored in a local developement environment to build our image
     +label=Local
     +icon=fa-folder:black
     +sort=100
     """
 
     type: constr(regex=r"^local$") = Field(..., description="+value=local")
     project_root_path: str = Field("./", description="+usage=Local project root path.")
     local_build: bool = Field(True, description="run docker build locally")
 
 
 class Manual(BaseModel):
     """
-        +docs=Describes that we are going to manually trigger our job.
+    +docs=Describes that we are going to manually trigger our job.
     +label=Manual
     +usage=Trigger the job manually. [Docs](https://docs.truefoundry.com/docs/more-configurations)
     """
 
     type: constr(regex=r"^manual$") = Field(..., description="+value=manual")
 
 
 class CapacityType(str, Enum):
     """
-        +label=Capacity Type
+    +label=Capacity Type
     +usage=Configure what type of nodes to run the app. By default no placement logic is applied.
     "spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.
     "spot" will strictly place the application on spot nodes.
     "on_demand" will strictly place the application on on-demand nodes.
     """
 
     spot_fallback_on_demand = "spot_fallback_on_demand"
@@ -238,16 +249,16 @@
     """
     +label=Node pool selector
     """
 
     type: Literal["nodepool_selector"] = Field(
         ..., description="+value=nodepool_selector"
     )
-    nodepools: List[str] = Field(
-        ...,
+    nodepools: Optional[List[str]] = Field(
+        None,
         description="+label=Nodepools\n+usage=Nodepools where you want to run your workload. Multiple nodepools can be selected.\n The workload is guaranteed to be scheduled on one of the nodepool",
     )
 
 
 class ParamType(str, Enum):
     string = "string"
     ml_repo = "ml_repo"
@@ -276,15 +287,15 @@
 
     TCP = "TCP"
     UDP = "UDP"
 
 
 class AppProtocol(str, Enum):
     """
-        +label=Application Protocol
+    +label=Application Protocol
     +usage=Application Protocol for the port.
     Select the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).
     If you are running a gRPC server, select the `grpc` option.
     This is only applicable if `expose=true`.
     """
 
     http = "http"
@@ -327,15 +338,15 @@
         description="+label=Application Protocol\n+usage=Application Protocol for the port.\nSelect the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).\nIf you are running a gRPC server, select the `grpc` option.\nThis is only applicable if `expose=true`.",
     )
     auth: Optional[BasicAuthCreds] = None
 
 
 class PythonBuild(BaseModel):
     """
-        +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
+    +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
     +label=Python Code (I don't have Dockerfile)
     +icon=fa-brands fa-python:#306998
     """
 
     type: constr(regex=r"^tfy-python-buildpack$") = Field(
         ..., description="+value=tfy-python-buildpack"
     )
@@ -379,29 +390,29 @@
         ...,
         description="+label=Requests per second\n+usage=Average request per second averaged over all replicas that autoscaler should try to maintain",
     )
 
 
 class RemoteSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a remote respository to build our image
+    +docs=Describes that we are using code stored in a remote respository to build our image
     +label=S3
     +icon=fa-brands fa-aws:black
     +sort=200
     """
 
     type: constr(regex=r"^remote$") = Field(..., description="+value=remote")
     remote_uri: str = Field(
         ..., description="+docs=Remote repository URI\n+label=Remote URI"
     )
 
 
 class Resources(BaseModel):
     """
-        +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
+    +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
     To learn more you can go [here](https://docs.truefoundry.com/docs/resources)
     +icon=fa-microchip
     +label=Resources
     +usage=Set resource constraints for the application. [Docs](https://docs.truefoundry.com/docs/resources)
     """
 
     cpu_request: confloat(ge=0.001, le=128.0) = Field(
@@ -440,15 +451,15 @@
         None,
         description="+label=Node\n+usage=This field determines how the underlying node resource is to be utilized",
     )
 
 
 class Rolling(BaseModel):
     """
-        +docs=This strategy updates the pods in a rolling fashion such that a subset of the
+    +docs=This strategy updates the pods in a rolling fashion such that a subset of the
     total pods are replaced with new version at one time.
     A commonly used strategy can be to have maxUnavailablePercentage close to 0 so that there
     is no downtime and keep the maxSurgePercentage to around 25%. If you are anyways running
     a large number of pods, the service can often tolerate a few pods going down - so you
     max maxUnavailablePercentage = 10 and maxSurgePercentage=0. You can read about it more
     [here](https://spot.io/resources/kubernetes-autoscaling/5-kubernetes-deployment-strategies-roll-out-like-the-pros/)
     +label=Rolling update strategy
@@ -465,27 +476,27 @@
         0,
         description="+label=Max Surge(%)\n+usage=Percentage of total replicas of updated image that can be brought up over the total replicas count.\nFor a value of 25 when replicas are set to 12 this would mean (12+(25% of 12) = 15) pods might be running at one time.\nSetting this to a higher value can help in speeding up the deployment process.",
     )
 
 
 class ConcurrencyPolicy(str, Enum):
     """
-        +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
+    +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
     will enable multiple instances of this job to run. Forbid will keep the current instance of the job running and stop a new instance from being run.
     Replace will terminate any currently running instance of the job and start a new one.
     """
 
     Forbid = "Forbid"
     Allow = "Allow"
     Replace = "Replace"
 
 
 class Schedule(BaseModel):
     """
-        +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
+    +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
     +label=Schedule
     +usage=Run the job on a schedule. [Docs](https://docs.truefoundry.com/docs/deploy-a-cron-job)
     """
 
     type: constr(regex=r"^scheduled$") = Field(..., description="+value=scheduled")
     schedule: str = Field(
         ...,
@@ -520,15 +531,15 @@
         description="+label=File Path\n+usage=Absolute file path where the file will be created.\n+message=Please enter a valid file path",
     )
     data: str = Field(..., description="+label=Data\n+usage=The file content.")
 
 
 class TruefoundryModelRegistry(BaseModel):
     """
-        +docs=Truefoundry model registry (deploy a model from TFY model registry)
+    +docs=Truefoundry model registry (deploy a model from TFY model registry)
     +label=Truefoundry model registry
     +usage=Deploy a model from TFY model registry
     """
 
     type: constr(regex=r"^tfy-model-registry$") = Field(
         ..., description="+value=tfy-model-registry"
     )
@@ -547,15 +558,15 @@
     volume_fqn: constr(regex=r"^tfy-volume:\/\/.+:.+:.+$") = Field(
         ...,
         description="+label=Volume\n+usage=The Truefoundry volume that needs to be mounted.",
     )
 
 
 class Autoscaling(BaseModel):
-    min_replicas: conint(ge=1) = Field(
+    min_replicas: conint(ge=0) = Field(
         1,
         description="+label=Minimum replicas\n+usage=Minimum number of replicas to keep available",
     )
     max_replicas: conint(ge=1, le=20) = Field(
         ...,
         description="+label=Maximum replicas\n+usage=Maximum number of replicas allowed for the component.",
     )
@@ -563,15 +574,15 @@
         ...,
         description="+label=Autoscaling metrics\n+usage=Metrics to use for the autoscaler",
     )
 
 
 class Build(BaseModel):
     """
-        +docs=Describes how we build our code into a Docker image.
+    +docs=Describes how we build our code into a Docker image.
     +label=Source Code (Build and deploy source code)
     +icon=fa-code
     """
 
     type: constr(regex=r"^build$") = Field(..., description="+value=build")
     docker_registry: Optional[str] = Field(
         None,
@@ -585,29 +596,29 @@
         ...,
         description="+docs=Instructions to build a container image out of the build source\n+label=Build using DockerFile or using Buildpack\n+icon=fa-wrench\n+sort=2",
     )
 
 
 class Canary(BaseModel):
     """
-        +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
+    +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
     This can help with verifying the health of the new release without shifting complete traffic.
     +label=Canary strategy
     """
 
     type: Literal["canary"] = Field(..., description="+value=canary")
     steps: List[CanaryStep] = Field(
         ...,
         description="+docs=These steps would be executed in order to enable shifting of traffic slowly from stable to canary version\n+label=Steps",
     )
 
 
 class HealthProbe(BaseModel):
     """
-        +docs=Describes the configuration for the Health Probe's
+    +docs=Describes the configuration for the Health Probe's
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +icon=fa-heart
     """
 
     config: HttpProbe
     initial_delay_seconds: conint(ge=0, le=36000) = Field(
         0,
@@ -673,15 +684,15 @@
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
 class ModelDeployment(BaseModel):
     """
-        +docs=Describes the configuration for the model deployment
+    +docs=Describes the configuration for the model deployment
     +usage=To learn more you can go [here](https://dash.readme.com/project/truefoundry/v0.1.1/docs/model-deployment-2)
     """
 
     type: constr(regex=r"^model-deployment$") = Field(
         ..., description="+value=model-deployment"
     )
     name: constr(regex=r"^[a-z][a-z0-9\-]{1,17}[a-z0-9]$") = Field(
@@ -710,15 +721,15 @@
         description="+usage=Name of the service. This uniquely identifies this service in the workspace.\n> Name can only contain alphanumeric characters and '-' and can be atmost 25 characters long\n+sort=1\n+message=3 to 25 lower case characters long alphanumeric word, may contain - in between, cannot start with a number",
     )
     image: Union[Build, Image] = Field(
         ...,
         description="+docs=Specify whether you want to deploy a Docker image or build and deploy from source code\n+label=Deploy a Docker image or build and deploy from source code\n+icon=fa-solid fa-cloud-arrow-up:#21B6A8\n+sort=2",
     )
     resources: Optional[Resources] = None
-    replicas: Union[confloat(ge=1.0, le=20.0), Autoscaling] = Field(
+    replicas: Union[confloat(ge=0.0, le=20.0), Autoscaling] = Field(
         1,
         description="+label=Replicas\n+usage=Replicas of service you want to run\n+icon=fa-clone\n+sort=3",
     )
     env: Optional[Dict[str, str]] = Field(
         None,
         description="+label=Environment Variables\n+usage=Configure environment variables to be injected in the service. [Docs](https://docs.truefoundry.com/docs/env-variables)\n+icon=fa-globe\n+sort=6",
     )
@@ -742,11 +753,12 @@
         None,
         description="+label=Rollout strategy\n+usage=Strategy to dictate how a rollout should happen when a new release for this service is made",
     )
     allow_interception: bool = Field(
         False,
         description="+label=Allow intercepts\n+usage=Whether to allow intercepts to be applied for this service.\nThis would inject an additional sidecar in each pod of the service. Not recommended on production",
     )
+    kustomize: Optional[Kustomize] = None
 
 
 class Application(BaseModel):
     __root__: Union[Service, Job, ModelDeployment]
```

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.2/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         [apt_update_command, apt_install_command, clear_apt_lists_command]
     )
 
 
 def generate_pip_install_command(
     requirements_path: Optional[str], pip_packages: Optional[List[str]]
 ) -> Optional[str]:
-    upgrade_pip_command = "python -m pip install -U pip"
+    upgrade_pip_command = "python -m pip install -U pip setuptools wheel"
     final_pip_install_command = None
     pip_install_base_command = "python -m pip install --use-pep517 --no-cache-dir"
     if requirements_path:
         final_pip_install_command = f"{pip_install_base_command} -r {requirements_path}"
 
     if pip_packages:
         final_pip_install_command = (
```

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.2/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.2/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.2/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/display_util.py` & `servicefoundry-0.9.2/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/cli/util.py` & `servicefoundry-0.9.2/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.2/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/app.py` & `servicefoundry-0.9.2/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/build.py` & `servicefoundry-0.9.2/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.2/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.2/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/route.py` & `servicefoundry-0.9.2/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/service.py` & `servicefoundry-0.9.2/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.2/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.2/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.2/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.2/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.2/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.2/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.2/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.2/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.2/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.2/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.2/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.2/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.2/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.2/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.2/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.2/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.2/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.2/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/const.py` & `servicefoundry-0.9.2/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.2/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.2/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.2/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.2/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.2/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.2/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.2/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.2/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.2/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.2/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/messages.py` & `servicefoundry-0.9.2/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.2/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/session.py` & `servicefoundry-0.9.2/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/util.py` & `servicefoundry-0.9.2/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/lib/win32.py` & `servicefoundry-0.9.2/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/logger.py` & `servicefoundry-0.9.2/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.2/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.2/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.2/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.2/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.2/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.2/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.1rc1/PKG-INFO` & `servicefoundry-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.1rc1
+Version: 0.9.2
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```


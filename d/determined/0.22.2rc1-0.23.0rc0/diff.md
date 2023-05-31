# Comparing `tmp/determined-0.22.2rc1-py3-none-any.whl.zip` & `tmp/determined-0.23.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,251 +1,259 @@
-Zip file size: 569192 bytes, number of entries: 249
--rw-r--r--  2.0 unx     1131 b- defN 23-May-22 23:17 determined/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-May-22 23:17 determined/__version__.py
--rw-r--r--  2.0 unx     1664 b- defN 23-May-22 23:17 determined/_env_context.py
--rw-r--r--  2.0 unx     8804 b- defN 23-May-22 23:17 determined/_execution.py
--rw-r--r--  2.0 unx     2779 b- defN 23-May-22 23:17 determined/_experiment_config.py
--rw-r--r--  2.0 unx     4781 b- defN 23-May-22 23:17 determined/_import.py
--rw-r--r--  2.0 unx    14901 b- defN 23-May-22 23:17 determined/_info.py
--rw-r--r--  2.0 unx     1272 b- defN 23-May-22 23:17 determined/_tf_rng.py
--rw-r--r--  2.0 unx     1214 b- defN 23-May-22 23:17 determined/_trial.py
--rw-r--r--  2.0 unx     4726 b- defN 23-May-22 23:17 determined/_trial_context.py
--rw-r--r--  2.0 unx     3356 b- defN 23-May-22 23:17 determined/_trial_controller.py
--rw-r--r--  2.0 unx     2417 b- defN 23-May-22 23:17 determined/constants.py
--rw-r--r--  2.0 unx     2734 b- defN 23-May-22 23:17 determined/errors.py
--rw-r--r--  2.0 unx     5431 b- defN 23-May-22 23:17 determined/gpu.py
--rw-r--r--  2.0 unx     6182 b- defN 23-May-22 23:17 determined/horovod.py
--rw-r--r--  2.0 unx    19382 b- defN 23-May-22 23:17 determined/ipc.py
--rw-r--r--  2.0 unx     3065 b- defN 23-May-22 23:17 determined/load.py
--rw-r--r--  2.0 unx      737 b- defN 23-May-22 23:17 determined/monkey_patch.py
--rw-r--r--  2.0 unx    39670 b- defN 23-May-22 23:17 determined/profiler.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/py.typed
--rw-r--r--  2.0 unx    15909 b- defN 23-May-22 23:17 determined/util.py
--rw-r--r--  2.0 unx     6578 b- defN 23-May-22 23:17 determined/workload.py
--rw-r--r--  2.0 unx      476 b- defN 23-May-22 23:17 determined/cli/__init__.py
--rw-r--r--  2.0 unx       75 b- defN 23-May-22 23:17 determined/cli/__main__.py
--rw-r--r--  2.0 unx     3423 b- defN 23-May-22 23:17 determined/cli/_util.py
--rw-r--r--  2.0 unx     9810 b- defN 23-May-22 23:17 determined/cli/agent.py
--rw-r--r--  2.0 unx     6409 b- defN 23-May-22 23:17 determined/cli/checkpoint.py
--rw-r--r--  2.0 unx    12530 b- defN 23-May-22 23:17 determined/cli/cli.py
--rw-r--r--  2.0 unx    14081 b- defN 23-May-22 23:17 determined/cli/command.py
--rw-r--r--  2.0 unx     2138 b- defN 23-May-22 23:17 determined/cli/dev.py
--rw-r--r--  2.0 unx      739 b- defN 23-May-22 23:17 determined/cli/errors.py
--rw-r--r--  2.0 unx    50931 b- defN 23-May-22 23:17 determined/cli/experiment.py
--rw-r--r--  2.0 unx     8291 b- defN 23-May-22 23:17 determined/cli/job.py
--rw-r--r--  2.0 unx     2137 b- defN 23-May-22 23:17 determined/cli/master.py
--rw-r--r--  2.0 unx     8747 b- defN 23-May-22 23:17 determined/cli/model.py
--rw-r--r--  2.0 unx     5641 b- defN 23-May-22 23:17 determined/cli/notebook.py
--rw-r--r--  2.0 unx     1761 b- defN 23-May-22 23:17 determined/cli/oauth.py
--rw-r--r--  2.0 unx    12190 b- defN 23-May-22 23:17 determined/cli/project.py
--rw-r--r--  2.0 unx    10219 b- defN 23-May-22 23:17 determined/cli/proxy.py
--rw-r--r--  2.0 unx    18787 b- defN 23-May-22 23:17 determined/cli/rbac.py
--rw-r--r--  2.0 unx     3783 b- defN 23-May-22 23:17 determined/cli/remote.py
--rw-r--r--  2.0 unx     4847 b- defN 23-May-22 23:17 determined/cli/render.py
--rw-r--r--  2.0 unx     2372 b- defN 23-May-22 23:17 determined/cli/resources.py
--rw-r--r--  2.0 unx     9718 b- defN 23-May-22 23:17 determined/cli/shell.py
--rw-r--r--  2.0 unx     5240 b- defN 23-May-22 23:17 determined/cli/sso.py
--rw-r--r--  2.0 unx     6400 b- defN 23-May-22 23:17 determined/cli/task.py
--rw-r--r--  2.0 unx     5354 b- defN 23-May-22 23:17 determined/cli/template.py
--rw-r--r--  2.0 unx     8240 b- defN 23-May-22 23:17 determined/cli/tensorboard.py
--rw-r--r--  2.0 unx      135 b- defN 23-May-22 23:17 determined/cli/top_arg_descriptions.py
--rw-r--r--  2.0 unx    15112 b- defN 23-May-22 23:17 determined/cli/trial.py
--rw-r--r--  2.0 unx     1448 b- defN 23-May-22 23:17 determined/cli/tunnel.py
--rw-r--r--  2.0 unx     6875 b- defN 23-May-22 23:17 determined/cli/user.py
--rw-r--r--  2.0 unx     9754 b- defN 23-May-22 23:17 determined/cli/user_groups.py
--rw-r--r--  2.0 unx     2557 b- defN 23-May-22 23:17 determined/cli/version.py
--rw-r--r--  2.0 unx    15179 b- defN 23-May-22 23:17 determined/cli/workspace.py
--rw-r--r--  2.0 unx      352 b- defN 23-May-22 23:17 determined/common/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 23-May-22 23:17 determined/common/_logging.py
--rw-r--r--  2.0 unx     8593 b- defN 23-May-22 23:17 determined/common/check.py
--rw-r--r--  2.0 unx     2255 b- defN 23-May-22 23:17 determined/common/constants.py
--rw-r--r--  2.0 unx     8222 b- defN 23-May-22 23:17 determined/common/context.py
--rw-r--r--  2.0 unx     8612 b- defN 23-May-22 23:17 determined/common/declarative_argparse.py
--rw-r--r--  2.0 unx     1662 b- defN 23-May-22 23:17 determined/common/requests.py
--rw-r--r--  2.0 unx     6349 b- defN 23-May-22 23:17 determined/common/util.py
--rw-r--r--  2.0 unx      778 b- defN 23-May-22 23:17 determined/common/api/__init__.py
--rw-r--r--  2.0 unx     3383 b- defN 23-May-22 23:17 determined/common/api/_session.py
--rw-r--r--  2.0 unx     2840 b- defN 23-May-22 23:17 determined/common/api/_util.py
--rw-r--r--  2.0 unx     1450 b- defN 23-May-22 23:17 determined/common/api/analytics.py
--rw-r--r--  2.0 unx    16070 b- defN 23-May-22 23:17 determined/common/api/authentication.py
--rw-r--r--  2.0 unx   619513 b- defN 23-May-22 23:17 determined/common/api/bindings.py
--rw-r--r--  2.0 unx     7415 b- defN 23-May-22 23:17 determined/common/api/certs.py
--rw-r--r--  2.0 unx     2555 b- defN 23-May-22 23:17 determined/common/api/errors.py
--rw-r--r--  2.0 unx     3235 b- defN 23-May-22 23:17 determined/common/api/logs.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-22 23:17 determined/common/api/metric.py
--rw-r--r--  2.0 unx     3147 b- defN 23-May-22 23:17 determined/common/api/profiler.py
--rw-r--r--  2.0 unx    10416 b- defN 23-May-22 23:17 determined/common/api/request.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/common/api/checkpoint/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/common/api/checkpoint/torch_load.py
--rw-r--r--  2.0 unx      502 b- defN 23-May-22 23:17 determined/common/experimental/__init__.py
--rw-r--r--  2.0 unx    15864 b- defN 23-May-22 23:17 determined/common/experimental/determined.py
--rw-r--r--  2.0 unx    11398 b- defN 23-May-22 23:17 determined/common/experimental/experiment.py
--rw-r--r--  2.0 unx    12639 b- defN 23-May-22 23:17 determined/common/experimental/model.py
--rw-r--r--  2.0 unx      306 b- defN 23-May-22 23:17 determined/common/experimental/oauth2_scim_client.py
--rw-r--r--  2.0 unx      466 b- defN 23-May-22 23:17 determined/common/experimental/session.py
--rw-r--r--  2.0 unx    15743 b- defN 23-May-22 23:17 determined/common/experimental/trial.py
--rw-r--r--  2.0 unx     3503 b- defN 23-May-22 23:17 determined/common/experimental/user.py
--rw-r--r--  2.0 unx      125 b- defN 23-May-22 23:17 determined/common/experimental/checkpoint/__init__.py
--rw-r--r--  2.0 unx    13827 b- defN 23-May-22 23:17 determined/common/experimental/checkpoint/_checkpoint.py
--rw-r--r--  2.0 unx     3868 b- defN 23-May-22 23:17 determined/common/storage/__init__.py
--rw-r--r--  2.0 unx     3822 b- defN 23-May-22 23:17 determined/common/storage/azure.py
--rw-r--r--  2.0 unx     3514 b- defN 23-May-22 23:17 determined/common/storage/azure_client.py
--rw-r--r--  2.0 unx     7152 b- defN 23-May-22 23:17 determined/common/storage/base.py
--rw-r--r--  2.0 unx     4447 b- defN 23-May-22 23:17 determined/common/storage/boto3_credential_manager.py
--rw-r--r--  2.0 unx     1014 b- defN 23-May-22 23:17 determined/common/storage/cloud.py
--rw-r--r--  2.0 unx     5789 b- defN 23-May-22 23:17 determined/common/storage/gcs.py
--rw-r--r--  2.0 unx     2070 b- defN 23-May-22 23:17 determined/common/storage/hdfs.py
--rw-r--r--  2.0 unx     6195 b- defN 23-May-22 23:17 determined/common/storage/s3.py
--rw-r--r--  2.0 unx     7816 b- defN 23-May-22 23:17 determined/common/storage/shared.py
--rw-r--r--  2.0 unx      747 b- defN 23-May-22 23:17 determined/core/__init__.py
--rw-r--r--  2.0 unx    29691 b- defN 23-May-22 23:17 determined/core/_checkpoint.py
--rw-r--r--  2.0 unx    10984 b- defN 23-May-22 23:17 determined/core/_context.py
--rw-r--r--  2.0 unx    16194 b- defN 23-May-22 23:17 determined/core/_distributed.py
--rw-r--r--  2.0 unx    12738 b- defN 23-May-22 23:17 determined/core/_preempt.py
--rw-r--r--  2.0 unx    15041 b- defN 23-May-22 23:17 determined/core/_searcher.py
--rw-r--r--  2.0 unx      932 b- defN 23-May-22 23:17 determined/core/_tensorboard_mode.py
--rw-r--r--  2.0 unx    10462 b- defN 23-May-22 23:17 determined/core/_train.py
--rw-r--r--  2.0 unx       40 b- defN 23-May-22 23:17 determined/deploy/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 23-May-22 23:17 determined/deploy/cli.py
--rw-r--r--  2.0 unx       94 b- defN 23-May-22 23:17 determined/deploy/errors.py
--rw-r--r--  2.0 unx     1472 b- defN 23-May-22 23:17 determined/deploy/healthcheck.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/aws/__init__.py
--rw-r--r--  2.0 unx    19597 b- defN 23-May-22 23:17 determined/deploy/aws/aws.py
--rw-r--r--  2.0 unx    24035 b- defN 23-May-22 23:17 determined/deploy/aws/cli.py
--rw-r--r--  2.0 unx     2998 b- defN 23-May-22 23:17 determined/deploy/aws/constants.py
--rw-r--r--  2.0 unx     1420 b- defN 23-May-22 23:17 determined/deploy/aws/gen_vcpu_mapping.py
--rw-r--r--  2.0 unx     2201 b- defN 23-May-22 23:17 determined/deploy/aws/master_config_inject.py
--rw-r--r--  2.0 unx     4911 b- defN 23-May-22 23:17 determined/deploy/aws/preflight.py
--rw-r--r--  2.0 unx    17324 b- defN 23-May-22 23:17 determined/deploy/aws/vcpu_mapping.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/__init__.py
--rw-r--r--  2.0 unx     5624 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/base.py
--rw-r--r--  2.0 unx     1593 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/govcloud.py
--rw-r--r--  2.0 unx     3094 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/secure.py
--rw-r--r--  2.0 unx     1349 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/simple.py
--rw-r--r--  2.0 unx     1400 b- defN 23-May-22 23:17 determined/deploy/aws/deployment_types/vpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/aws/templates/__init__.py
--rw-r--r--  2.0 unx    29259 b- defN 23-May-22 23:17 determined/deploy/aws/templates/efs.yaml
--rw-r--r--  2.0 unx    29969 b- defN 23-May-22 23:17 determined/deploy/aws/templates/fsx.yaml
--rw-r--r--  2.0 unx    23518 b- defN 23-May-22 23:17 determined/deploy/aws/templates/govcloud.yaml
--rw-r--r--  2.0 unx    29153 b- defN 23-May-22 23:17 determined/deploy/aws/templates/secure.yaml
--rw-r--r--  2.0 unx    24926 b- defN 23-May-22 23:17 determined/deploy/aws/templates/simple.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/gcp/__init__.py
--rw-r--r--  2.0 unx    19015 b- defN 23-May-22 23:17 determined/deploy/gcp/cli.py
--rw-r--r--  2.0 unx      772 b- defN 23-May-22 23:17 determined/deploy/gcp/constants.py
--rw-r--r--  2.0 unx    12420 b- defN 23-May-22 23:17 determined/deploy/gcp/gcp.py
--rw-r--r--  2.0 unx     2380 b- defN 23-May-22 23:17 determined/deploy/gcp/preflight.py
--rw-r--r--  2.0 unx     5376 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/main.tf
--rw-r--r--  2.0 unx     1569 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/master.yaml.tmpl
--rw-r--r--  2.0 unx     1487 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/outputs.tf
--rw-r--r--  2.0 unx     3767 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/variables.tf
--rw-r--r--  2.0 unx     6122 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/compute/main.tf
--rw-r--r--  2.0 unx      424 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/compute/outputs.tf
--rw-r--r--  2.0 unx     1574 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/compute/variables.tf
--rw-r--r--  2.0 unx     1222 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/database/main.tf
--rw-r--r--  2.0 unx      283 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/database/outputs.tf
--rw-r--r--  2.0 unx      320 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/database/variables.tf
--rw-r--r--  2.0 unx      522 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/filestore/main.tf
--rw-r--r--  2.0 unx      184 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
--rw-r--r--  2.0 unx      125 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/filestore/variables.tf
--rw-r--r--  2.0 unx     1026 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/firewall/main.tf
--rw-r--r--  2.0 unx      195 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
--rw-r--r--  2.0 unx       75 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/firewall/variables.tf
--rw-r--r--  2.0 unx      637 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/gcs/main.tf
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
--rw-r--r--  2.0 unx      161 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/gcs/variables.tf
--rw-r--r--  2.0 unx      161 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/ip/main.tf
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/ip/outputs.tf
--rw-r--r--  2.0 unx       88 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/ip/variables.tf
--rw-r--r--  2.0 unx     1112 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/network/main.tf
--rw-r--r--  2.0 unx      275 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/network/outputs.tf
--rw-r--r--  2.0 unx      207 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/network/variables.tf
--rw-r--r--  2.0 unx      962 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/service_account/main.tf
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
--rw-r--r--  2.0 unx      138 b- defN 23-May-22 23:17 determined/deploy/gcp/terraform/modules/service_account/variables.tf
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/gke/__init__.py
--rw-r--r--  2.0 unx    19568 b- defN 23-May-22 23:17 determined/deploy/gke/cli.py
--rw-r--r--  2.0 unx      408 b- defN 23-May-22 23:17 determined/deploy/gke/constants.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/deploy/local/__init__.py
--rw-r--r--  2.0 unx    12829 b- defN 23-May-22 23:17 determined/deploy/local/cli.py
--rw-r--r--  2.0 unx    16913 b- defN 23-May-22 23:17 determined/deploy/local/cluster_utils.py
--rw-r--r--  2.0 unx     1134 b- defN 23-May-22 23:17 determined/deploy/local/preflight.py
--rw-r--r--  2.0 unx      697 b- defN 23-May-22 23:17 determined/estimator/__init__.py
--rw-r--r--  2.0 unx     1288 b- defN 23-May-22 23:17 determined/estimator/_callback.py
--rw-r--r--  2.0 unx     7375 b- defN 23-May-22 23:17 determined/estimator/_estimator_context.py
--rw-r--r--  2.0 unx    40175 b- defN 23-May-22 23:17 determined/estimator/_estimator_trial.py
--rw-r--r--  2.0 unx     3086 b- defN 23-May-22 23:17 determined/estimator/_load.py
--rw-r--r--  2.0 unx    13742 b- defN 23-May-22 23:17 determined/estimator/_reducer.py
--rw-r--r--  2.0 unx     9600 b- defN 23-May-22 23:17 determined/estimator/_util.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/exec/__init__.py
--rw-r--r--  2.0 unx     3836 b- defN 23-May-22 23:17 determined/exec/gc_checkpoints.py
--rw-r--r--  2.0 unx     8857 b- defN 23-May-22 23:17 determined/exec/harness.py
--rw-r--r--  2.0 unx     4233 b- defN 23-May-22 23:17 determined/exec/launch.py
--rw-r--r--  2.0 unx      389 b- defN 23-May-22 23:17 determined/exec/pid_client.py
--rw-r--r--  2.0 unx     1476 b- defN 23-May-22 23:17 determined/exec/pid_server.py
--rw-r--r--  2.0 unx    13479 b- defN 23-May-22 23:17 determined/exec/prep_container.py
--rw-r--r--  2.0 unx    10994 b- defN 23-May-22 23:17 determined/exec/tensorboard.py
--rw-r--r--  2.0 unx      264 b- defN 23-May-22 23:17 determined/experimental/__init__.py
--rw-r--r--  2.0 unx     3473 b- defN 23-May-22 23:17 determined/experimental/_native.py
--rw-r--r--  2.0 unx    15160 b- defN 23-May-22 23:17 determined/experimental/client.py
--rw-r--r--  2.0 unx      744 b- defN 23-May-22 23:17 determined/keras/__init__.py
--rw-r--r--  2.0 unx     7579 b- defN 23-May-22 23:17 determined/keras/_data.py
--rw-r--r--  2.0 unx    11491 b- defN 23-May-22 23:17 determined/keras/_enqueuer.py
--rw-r--r--  2.0 unx     4020 b- defN 23-May-22 23:17 determined/keras/_load.py
--rw-r--r--  2.0 unx      486 b- defN 23-May-22 23:17 determined/keras/_tensorboard_callback.py
--rw-r--r--  2.0 unx    19042 b- defN 23-May-22 23:17 determined/keras/_tf_keras_context.py
--rw-r--r--  2.0 unx     1204 b- defN 23-May-22 23:17 determined/keras/_tf_keras_multi_gpu.py
--rw-r--r--  2.0 unx    48040 b- defN 23-May-22 23:17 determined/keras/_tf_keras_trial.py
--rw-r--r--  2.0 unx    28556 b- defN 23-May-22 23:17 determined/keras/callbacks.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 23:17 determined/launch/__init__.py
--rw-r--r--  2.0 unx    13720 b- defN 23-May-22 23:17 determined/launch/deepspeed.py
--rw-r--r--  2.0 unx    10813 b- defN 23-May-22 23:17 determined/launch/horovod.py
--rw-r--r--  2.0 unx     4574 b- defN 23-May-22 23:17 determined/launch/torch_distributed.py
--rw-r--r--  2.0 unx     4502 b- defN 23-May-22 23:17 determined/launch/wrap_rank.py
--rw-r--r--  2.0 unx       98 b- defN 23-May-22 23:17 determined/layers/__init__.py
--rw-r--r--  2.0 unx    19401 b- defN 23-May-22 23:17 determined/layers/_workload_sequencer.py
--rw-r--r--  2.0 unx     1151 b- defN 23-May-22 23:17 determined/pytorch/__init__.py
--rw-r--r--  2.0 unx     5459 b- defN 23-May-22 23:17 determined/pytorch/_callback.py
--rw-r--r--  2.0 unx    16294 b- defN 23-May-22 23:17 determined/pytorch/_data.py
--rw-r--r--  2.0 unx     3670 b- defN 23-May-22 23:17 determined/pytorch/_experimental.py
--rw-r--r--  2.0 unx    12510 b- defN 23-May-22 23:17 determined/pytorch/_load.py
--rw-r--r--  2.0 unx     3286 b- defN 23-May-22 23:17 determined/pytorch/_lr_scheduler.py
--rw-r--r--  2.0 unx     8275 b- defN 23-May-22 23:17 determined/pytorch/_metric_utils.py
--rw-r--r--  2.0 unx    45136 b- defN 23-May-22 23:17 determined/pytorch/_pytorch_context.py
--rw-r--r--  2.0 unx    68474 b- defN 23-May-22 23:17 determined/pytorch/_pytorch_trial.py
--rw-r--r--  2.0 unx    21406 b- defN 23-May-22 23:17 determined/pytorch/_reducer.py
--rw-r--r--  2.0 unx    13510 b- defN 23-May-22 23:17 determined/pytorch/_trainer.py
--rw-r--r--  2.0 unx     9561 b- defN 23-May-22 23:17 determined/pytorch/samplers.py
--rw-r--r--  2.0 unx      347 b- defN 23-May-22 23:17 determined/pytorch/deepspeed/__init__.py
--rw-r--r--  2.0 unx    17524 b- defN 23-May-22 23:17 determined/pytorch/deepspeed/_deepspeed_context.py
--rw-r--r--  2.0 unx    42777 b- defN 23-May-22 23:17 determined/pytorch/deepspeed/_deepspeed_trial.py
--rw-r--r--  2.0 unx     1987 b- defN 23-May-22 23:17 determined/pytorch/deepspeed/_mpu.py
--rw-r--r--  2.0 unx       67 b- defN 23-May-22 23:17 determined/pytorch/lightning/__init__.py
--rw-r--r--  2.0 unx    18157 b- defN 23-May-22 23:17 determined/pytorch/lightning/_adapter.py
--rw-r--r--  2.0 unx      343 b- defN 23-May-22 23:17 determined/searcher/__init__.py
--rw-r--r--  2.0 unx     3563 b- defN 23-May-22 23:17 determined/searcher/_remote_search_runner.py
--rw-r--r--  2.0 unx    10081 b- defN 23-May-22 23:17 determined/searcher/_search_method.py
--rw-r--r--  2.0 unx    14053 b- defN 23-May-22 23:17 determined/searcher/_search_runner.py
--rw-r--r--  2.0 unx      512 b- defN 23-May-22 23:17 determined/tensorboard/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-May-22 23:17 determined/tensorboard/azure.py
--rw-r--r--  2.0 unx     5884 b- defN 23-May-22 23:17 determined/tensorboard/base.py
--rw-r--r--  2.0 unx     4534 b- defN 23-May-22 23:17 determined/tensorboard/build.py
--rw-r--r--  2.0 unx     2305 b- defN 23-May-22 23:17 determined/tensorboard/gcs.py
--rw-r--r--  2.0 unx     1333 b- defN 23-May-22 23:17 determined/tensorboard/hdfs.py
--rw-r--r--  2.0 unx     1892 b- defN 23-May-22 23:17 determined/tensorboard/s3.py
--rw-r--r--  2.0 unx     1747 b- defN 23-May-22 23:17 determined/tensorboard/shared.py
--rw-r--r--  2.0 unx     3734 b- defN 23-May-22 23:17 determined/tensorboard/util.py
--rw-r--r--  2.0 unx      780 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/azure.py
--rw-r--r--  2.0 unx     1670 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/base.py
--rw-r--r--  2.0 unx     1733 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/gcs.py
--rw-r--r--  2.0 unx     2476 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/s3.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-22 23:17 determined/tensorboard/fetchers/shared.py
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 23:17 determined/tensorboard/metric_writers/__init__.py
--rw-r--r--  2.0 unx     2113 b- defN 23-May-22 23:17 determined/tensorboard/metric_writers/callback.py
--rw-r--r--  2.0 unx     2936 b- defN 23-May-22 23:17 determined/tensorboard/metric_writers/pytorch.py
--rw-r--r--  2.0 unx     4385 b- defN 23-May-22 23:17 determined/tensorboard/metric_writers/tensorflow.py
--rw-r--r--  2.0 unx     1262 b- defN 23-May-22 23:17 determined-0.22.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 23:17 determined-0.22.2rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-May-22 23:17 determined-0.22.2rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 23:17 determined-0.22.2rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    22843 b- defN 23-May-22 23:17 determined-0.22.2rc1.dist-info/RECORD
-249 files, 2373457 bytes uncompressed, 532762 bytes compressed:  77.6%
+Zip file size: 607479 bytes, number of entries: 257
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-31 17:03 determined/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-May-31 17:03 determined/__version__.py
+-rw-r--r--  2.0 unx     1664 b- defN 23-May-31 17:03 determined/_env_context.py
+-rw-r--r--  2.0 unx     8804 b- defN 23-May-31 17:03 determined/_execution.py
+-rw-r--r--  2.0 unx     2779 b- defN 23-May-31 17:03 determined/_experiment_config.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-May-31 17:03 determined/_import.py
+-rw-r--r--  2.0 unx    14901 b- defN 23-May-31 17:03 determined/_info.py
+-rw-r--r--  2.0 unx     1272 b- defN 23-May-31 17:03 determined/_tf_rng.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-May-31 17:03 determined/_trial.py
+-rw-r--r--  2.0 unx     4726 b- defN 23-May-31 17:03 determined/_trial_context.py
+-rw-r--r--  2.0 unx     3356 b- defN 23-May-31 17:03 determined/_trial_controller.py
+-rw-r--r--  2.0 unx     2417 b- defN 23-May-31 17:03 determined/constants.py
+-rw-r--r--  2.0 unx     2734 b- defN 23-May-31 17:03 determined/errors.py
+-rw-r--r--  2.0 unx     5431 b- defN 23-May-31 17:03 determined/gpu.py
+-rw-r--r--  2.0 unx     6182 b- defN 23-May-31 17:03 determined/horovod.py
+-rw-r--r--  2.0 unx    19382 b- defN 23-May-31 17:03 determined/ipc.py
+-rw-r--r--  2.0 unx     3065 b- defN 23-May-31 17:03 determined/load.py
+-rw-r--r--  2.0 unx      737 b- defN 23-May-31 17:03 determined/monkey_patch.py
+-rw-r--r--  2.0 unx    39670 b- defN 23-May-31 17:03 determined/profiler.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/py.typed
+-rw-r--r--  2.0 unx    16449 b- defN 23-May-31 17:03 determined/util.py
+-rw-r--r--  2.0 unx     6578 b- defN 23-May-31 17:03 determined/workload.py
+-rw-r--r--  2.0 unx      497 b- defN 23-May-31 17:03 determined/cli/__init__.py
+-rw-r--r--  2.0 unx       75 b- defN 23-May-31 17:03 determined/cli/__main__.py
+-rw-r--r--  2.0 unx     4002 b- defN 23-May-31 17:03 determined/cli/_util.py
+-rw-r--r--  2.0 unx     9810 b- defN 23-May-31 17:03 determined/cli/agent.py
+-rw-r--r--  2.0 unx     8025 b- defN 23-May-31 17:03 determined/cli/checkpoint.py
+-rw-r--r--  2.0 unx    12532 b- defN 23-May-31 17:03 determined/cli/cli.py
+-rw-r--r--  2.0 unx    12930 b- defN 23-May-31 17:03 determined/cli/command.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-May-31 17:03 determined/cli/dev.py
+-rw-r--r--  2.0 unx      739 b- defN 23-May-31 17:03 determined/cli/errors.py
+-rw-r--r--  2.0 unx    50903 b- defN 23-May-31 17:03 determined/cli/experiment.py
+-rw-r--r--  2.0 unx     8291 b- defN 23-May-31 17:03 determined/cli/job.py
+-rw-r--r--  2.0 unx     2105 b- defN 23-May-31 17:03 determined/cli/master.py
+-rw-r--r--  2.0 unx     8747 b- defN 23-May-31 17:03 determined/cli/model.py
+-rw-r--r--  2.0 unx     5531 b- defN 23-May-31 17:03 determined/cli/notebook.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-May-31 17:03 determined/cli/oauth.py
+-rw-r--r--  2.0 unx    12162 b- defN 23-May-31 17:03 determined/cli/project.py
+-rw-r--r--  2.0 unx    10219 b- defN 23-May-31 17:03 determined/cli/proxy.py
+-rw-r--r--  2.0 unx    18787 b- defN 23-May-31 17:03 determined/cli/rbac.py
+-rw-r--r--  2.0 unx     3846 b- defN 23-May-31 17:03 determined/cli/remote.py
+-rw-r--r--  2.0 unx     5948 b- defN 23-May-31 17:03 determined/cli/render.py
+-rw-r--r--  2.0 unx     2372 b- defN 23-May-31 17:03 determined/cli/resources.py
+-rw-r--r--  2.0 unx     9442 b- defN 23-May-31 17:03 determined/cli/shell.py
+-rw-r--r--  2.0 unx     5240 b- defN 23-May-31 17:03 determined/cli/sso.py
+-rw-r--r--  2.0 unx     6406 b- defN 23-May-31 17:03 determined/cli/task.py
+-rw-r--r--  2.0 unx     5354 b- defN 23-May-31 17:03 determined/cli/template.py
+-rw-r--r--  2.0 unx     7525 b- defN 23-May-31 17:03 determined/cli/tensorboard.py
+-rw-r--r--  2.0 unx      135 b- defN 23-May-31 17:03 determined/cli/top_arg_descriptions.py
+-rw-r--r--  2.0 unx    15033 b- defN 23-May-31 17:03 determined/cli/trial.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-May-31 17:03 determined/cli/tunnel.py
+-rw-r--r--  2.0 unx     7309 b- defN 23-May-31 17:03 determined/cli/user.py
+-rw-r--r--  2.0 unx     9754 b- defN 23-May-31 17:03 determined/cli/user_groups.py
+-rw-r--r--  2.0 unx     2557 b- defN 23-May-31 17:03 determined/cli/version.py
+-rw-r--r--  2.0 unx    15179 b- defN 23-May-31 17:03 determined/cli/workspace.py
+-rw-r--r--  2.0 unx      352 b- defN 23-May-31 17:03 determined/common/__init__.py
+-rw-r--r--  2.0 unx      498 b- defN 23-May-31 17:03 determined/common/_logging.py
+-rw-r--r--  2.0 unx     8593 b- defN 23-May-31 17:03 determined/common/check.py
+-rw-r--r--  2.0 unx     2154 b- defN 23-May-31 17:03 determined/common/constants.py
+-rw-r--r--  2.0 unx     8222 b- defN 23-May-31 17:03 determined/common/context.py
+-rw-r--r--  2.0 unx     8612 b- defN 23-May-31 17:03 determined/common/declarative_argparse.py
+-rw-r--r--  2.0 unx     1662 b- defN 23-May-31 17:03 determined/common/requests.py
+-rw-r--r--  2.0 unx     6867 b- defN 23-May-31 17:03 determined/common/util.py
+-rw-r--r--  2.0 unx      821 b- defN 23-May-31 17:03 determined/common/api/__init__.py
+-rw-r--r--  2.0 unx     3383 b- defN 23-May-31 17:03 determined/common/api/_session.py
+-rw-r--r--  2.0 unx     3644 b- defN 23-May-31 17:03 determined/common/api/_util.py
+-rw-r--r--  2.0 unx     1450 b- defN 23-May-31 17:03 determined/common/api/analytics.py
+-rw-r--r--  2.0 unx    16070 b- defN 23-May-31 17:03 determined/common/api/authentication.py
+-rw-r--r--  2.0 unx   627696 b- defN 23-May-31 17:03 determined/common/api/bindings.py
+-rw-r--r--  2.0 unx     7415 b- defN 23-May-31 17:03 determined/common/api/certs.py
+-rw-r--r--  2.0 unx     2555 b- defN 23-May-31 17:03 determined/common/api/errors.py
+-rw-r--r--  2.0 unx     3235 b- defN 23-May-31 17:03 determined/common/api/logs.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-31 17:03 determined/common/api/metric.py
+-rw-r--r--  2.0 unx     3147 b- defN 23-May-31 17:03 determined/common/api/profiler.py
+-rw-r--r--  2.0 unx    10416 b- defN 23-May-31 17:03 determined/common/api/request.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/common/api/checkpoint/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/common/api/checkpoint/torch_load.py
+-rw-r--r--  2.0 unx      502 b- defN 23-May-31 17:03 determined/common/experimental/__init__.py
+-rw-r--r--  2.0 unx    15864 b- defN 23-May-31 17:03 determined/common/experimental/determined.py
+-rw-r--r--  2.0 unx    11398 b- defN 23-May-31 17:03 determined/common/experimental/experiment.py
+-rw-r--r--  2.0 unx    12639 b- defN 23-May-31 17:03 determined/common/experimental/model.py
+-rw-r--r--  2.0 unx      306 b- defN 23-May-31 17:03 determined/common/experimental/oauth2_scim_client.py
+-rw-r--r--  2.0 unx      466 b- defN 23-May-31 17:03 determined/common/experimental/session.py
+-rw-r--r--  2.0 unx    15743 b- defN 23-May-31 17:03 determined/common/experimental/trial.py
+-rw-r--r--  2.0 unx     3503 b- defN 23-May-31 17:03 determined/common/experimental/user.py
+-rw-r--r--  2.0 unx      125 b- defN 23-May-31 17:03 determined/common/experimental/checkpoint/__init__.py
+-rw-r--r--  2.0 unx    14995 b- defN 23-May-31 17:03 determined/common/experimental/checkpoint/_checkpoint.py
+-rw-r--r--  2.0 unx     3809 b- defN 23-May-31 17:03 determined/common/storage/__init__.py
+-rw-r--r--  2.0 unx     4280 b- defN 23-May-31 17:03 determined/common/storage/azure.py
+-rw-r--r--  2.0 unx     3573 b- defN 23-May-31 17:03 determined/common/storage/azure_client.py
+-rw-r--r--  2.0 unx     9368 b- defN 23-May-31 17:03 determined/common/storage/base.py
+-rw-r--r--  2.0 unx     4447 b- defN 23-May-31 17:03 determined/common/storage/boto3_credential_manager.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-May-31 17:03 determined/common/storage/cloud.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-May-31 17:03 determined/common/storage/gcs.py
+-rw-r--r--  2.0 unx     6649 b- defN 23-May-31 17:03 determined/common/storage/s3.py
+-rw-r--r--  2.0 unx     8972 b- defN 23-May-31 17:03 determined/common/storage/shared.py
+-rw-r--r--  2.0 unx      747 b- defN 23-May-31 17:03 determined/core/__init__.py
+-rw-r--r--  2.0 unx    29425 b- defN 23-May-31 17:03 determined/core/_checkpoint.py
+-rw-r--r--  2.0 unx    11141 b- defN 23-May-31 17:03 determined/core/_context.py
+-rw-r--r--  2.0 unx    16194 b- defN 23-May-31 17:03 determined/core/_distributed.py
+-rw-r--r--  2.0 unx    12738 b- defN 23-May-31 17:03 determined/core/_preempt.py
+-rw-r--r--  2.0 unx    15041 b- defN 23-May-31 17:03 determined/core/_searcher.py
+-rw-r--r--  2.0 unx      932 b- defN 23-May-31 17:03 determined/core/_tensorboard_mode.py
+-rw-r--r--  2.0 unx    10462 b- defN 23-May-31 17:03 determined/core/_train.py
+-rw-r--r--  2.0 unx       40 b- defN 23-May-31 17:03 determined/deploy/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 23-May-31 17:03 determined/deploy/cli.py
+-rw-r--r--  2.0 unx       94 b- defN 23-May-31 17:03 determined/deploy/errors.py
+-rw-r--r--  2.0 unx     1472 b- defN 23-May-31 17:03 determined/deploy/healthcheck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/aws/__init__.py
+-rw-r--r--  2.0 unx    19597 b- defN 23-May-31 17:03 determined/deploy/aws/aws.py
+-rw-r--r--  2.0 unx    24189 b- defN 23-May-31 17:03 determined/deploy/aws/cli.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-May-31 17:03 determined/deploy/aws/constants.py
+-rw-r--r--  2.0 unx     1420 b- defN 23-May-31 17:03 determined/deploy/aws/gen_vcpu_mapping.py
+-rw-r--r--  2.0 unx     2201 b- defN 23-May-31 17:03 determined/deploy/aws/master_config_inject.py
+-rw-r--r--  2.0 unx     4911 b- defN 23-May-31 17:03 determined/deploy/aws/preflight.py
+-rw-r--r--  2.0 unx    17324 b- defN 23-May-31 17:03 determined/deploy/aws/vcpu_mapping.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/__init__.py
+-rw-r--r--  2.0 unx     5624 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/base.py
+-rw-r--r--  2.0 unx     1593 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/govcloud.py
+-rw-r--r--  2.0 unx     3094 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/secure.py
+-rw-r--r--  2.0 unx     1469 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/simple.py
+-rw-r--r--  2.0 unx     1400 b- defN 23-May-31 17:03 determined/deploy/aws/deployment_types/vpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/aws/templates/__init__.py
+-rw-r--r--  2.0 unx    29341 b- defN 23-May-31 17:03 determined/deploy/aws/templates/efs.yaml
+-rw-r--r--  2.0 unx    30051 b- defN 23-May-31 17:03 determined/deploy/aws/templates/fsx.yaml
+-rw-r--r--  2.0 unx    23665 b- defN 23-May-31 17:03 determined/deploy/aws/templates/govcloud.yaml
+-rw-r--r--  2.0 unx    29201 b- defN 23-May-31 17:03 determined/deploy/aws/templates/secure.yaml
+-rw-r--r--  2.0 unx    24822 b- defN 23-May-31 17:03 determined/deploy/aws/templates/simple-rds.yaml
+-rw-r--r--  2.0 unx    24974 b- defN 23-May-31 17:03 determined/deploy/aws/templates/simple.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/gcp/__init__.py
+-rw-r--r--  2.0 unx    19015 b- defN 23-May-31 17:03 determined/deploy/gcp/cli.py
+-rw-r--r--  2.0 unx      772 b- defN 23-May-31 17:03 determined/deploy/gcp/constants.py
+-rw-r--r--  2.0 unx    12420 b- defN 23-May-31 17:03 determined/deploy/gcp/gcp.py
+-rw-r--r--  2.0 unx     2380 b- defN 23-May-31 17:03 determined/deploy/gcp/preflight.py
+-rw-r--r--  2.0 unx     5376 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/main.tf
+-rw-r--r--  2.0 unx     1569 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/master.yaml.tmpl
+-rw-r--r--  2.0 unx     1487 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/outputs.tf
+-rw-r--r--  2.0 unx     3767 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/variables.tf
+-rw-r--r--  2.0 unx     6122 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/compute/main.tf
+-rw-r--r--  2.0 unx      424 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/compute/outputs.tf
+-rw-r--r--  2.0 unx     1574 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/compute/variables.tf
+-rw-r--r--  2.0 unx     1222 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/database/main.tf
+-rw-r--r--  2.0 unx      283 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/database/outputs.tf
+-rw-r--r--  2.0 unx      320 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/database/variables.tf
+-rw-r--r--  2.0 unx      522 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/filestore/main.tf
+-rw-r--r--  2.0 unx      184 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/filestore/outputs.tf
+-rw-r--r--  2.0 unx      125 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/filestore/variables.tf
+-rw-r--r--  2.0 unx     1026 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/firewall/main.tf
+-rw-r--r--  2.0 unx      195 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/firewall/outputs.tf
+-rw-r--r--  2.0 unx       75 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/firewall/variables.tf
+-rw-r--r--  2.0 unx      637 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/gcs/main.tf
+-rw-r--r--  2.0 unx       51 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/gcs/outputs.tf
+-rw-r--r--  2.0 unx      161 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/gcs/variables.tf
+-rw-r--r--  2.0 unx      161 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/ip/main.tf
+-rw-r--r--  2.0 unx      122 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/ip/outputs.tf
+-rw-r--r--  2.0 unx       88 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/ip/variables.tf
+-rw-r--r--  2.0 unx     1112 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/network/main.tf
+-rw-r--r--  2.0 unx      275 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/network/outputs.tf
+-rw-r--r--  2.0 unx      207 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/network/variables.tf
+-rw-r--r--  2.0 unx      962 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/service_account/main.tf
+-rw-r--r--  2.0 unx       73 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/service_account/outputs.tf
+-rw-r--r--  2.0 unx      138 b- defN 23-May-31 17:03 determined/deploy/gcp/terraform/modules/service_account/variables.tf
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/gke/__init__.py
+-rw-r--r--  2.0 unx    19568 b- defN 23-May-31 17:03 determined/deploy/gke/cli.py
+-rw-r--r--  2.0 unx      408 b- defN 23-May-31 17:03 determined/deploy/gke/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/deploy/local/__init__.py
+-rw-r--r--  2.0 unx    12829 b- defN 23-May-31 17:03 determined/deploy/local/cli.py
+-rw-r--r--  2.0 unx    16913 b- defN 23-May-31 17:03 determined/deploy/local/cluster_utils.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-31 17:03 determined/deploy/local/preflight.py
+-rw-r--r--  2.0 unx      697 b- defN 23-May-31 17:03 determined/estimator/__init__.py
+-rw-r--r--  2.0 unx     1288 b- defN 23-May-31 17:03 determined/estimator/_callback.py
+-rw-r--r--  2.0 unx     7375 b- defN 23-May-31 17:03 determined/estimator/_estimator_context.py
+-rw-r--r--  2.0 unx    40175 b- defN 23-May-31 17:03 determined/estimator/_estimator_trial.py
+-rw-r--r--  2.0 unx     3086 b- defN 23-May-31 17:03 determined/estimator/_load.py
+-rw-r--r--  2.0 unx    13742 b- defN 23-May-31 17:03 determined/estimator/_reducer.py
+-rw-r--r--  2.0 unx     9600 b- defN 23-May-31 17:03 determined/estimator/_util.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/exec/__init__.py
+-rw-r--r--  2.0 unx     5434 b- defN 23-May-31 17:03 determined/exec/gc_checkpoints.py
+-rw-r--r--  2.0 unx     8857 b- defN 23-May-31 17:03 determined/exec/harness.py
+-rw-r--r--  2.0 unx     4233 b- defN 23-May-31 17:03 determined/exec/launch.py
+-rw-r--r--  2.0 unx      389 b- defN 23-May-31 17:03 determined/exec/pid_client.py
+-rw-r--r--  2.0 unx     1476 b- defN 23-May-31 17:03 determined/exec/pid_server.py
+-rw-r--r--  2.0 unx    13479 b- defN 23-May-31 17:03 determined/exec/prep_container.py
+-rw-r--r--  2.0 unx    10994 b- defN 23-May-31 17:03 determined/exec/tensorboard.py
+-rw-r--r--  2.0 unx      308 b- defN 23-May-31 17:03 determined/experimental/__init__.py
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-31 17:03 determined/experimental/_native.py
+-rw-r--r--  2.0 unx    15330 b- defN 23-May-31 17:03 determined/experimental/client.py
+-rw-r--r--  2.0 unx     7673 b- defN 23-May-31 17:03 determined/experimental/unmanaged.py
+-rw-r--r--  2.0 unx      744 b- defN 23-May-31 17:03 determined/keras/__init__.py
+-rw-r--r--  2.0 unx     7579 b- defN 23-May-31 17:03 determined/keras/_data.py
+-rw-r--r--  2.0 unx    11491 b- defN 23-May-31 17:03 determined/keras/_enqueuer.py
+-rw-r--r--  2.0 unx     4020 b- defN 23-May-31 17:03 determined/keras/_load.py
+-rw-r--r--  2.0 unx      486 b- defN 23-May-31 17:03 determined/keras/_tensorboard_callback.py
+-rw-r--r--  2.0 unx    19042 b- defN 23-May-31 17:03 determined/keras/_tf_keras_context.py
+-rw-r--r--  2.0 unx     1204 b- defN 23-May-31 17:03 determined/keras/_tf_keras_multi_gpu.py
+-rw-r--r--  2.0 unx    48040 b- defN 23-May-31 17:03 determined/keras/_tf_keras_trial.py
+-rw-r--r--  2.0 unx    28556 b- defN 23-May-31 17:03 determined/keras/callbacks.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 17:03 determined/launch/__init__.py
+-rw-r--r--  2.0 unx    13720 b- defN 23-May-31 17:03 determined/launch/deepspeed.py
+-rw-r--r--  2.0 unx    10813 b- defN 23-May-31 17:03 determined/launch/horovod.py
+-rw-r--r--  2.0 unx     4574 b- defN 23-May-31 17:03 determined/launch/torch_distributed.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-May-31 17:03 determined/launch/wrap_rank.py
+-rw-r--r--  2.0 unx       98 b- defN 23-May-31 17:03 determined/layers/__init__.py
+-rw-r--r--  2.0 unx    19401 b- defN 23-May-31 17:03 determined/layers/_workload_sequencer.py
+-rw-r--r--  2.0 unx     1151 b- defN 23-May-31 17:03 determined/pytorch/__init__.py
+-rw-r--r--  2.0 unx     5459 b- defN 23-May-31 17:03 determined/pytorch/_callback.py
+-rw-r--r--  2.0 unx    16294 b- defN 23-May-31 17:03 determined/pytorch/_data.py
+-rw-r--r--  2.0 unx     3670 b- defN 23-May-31 17:03 determined/pytorch/_experimental.py
+-rw-r--r--  2.0 unx    12510 b- defN 23-May-31 17:03 determined/pytorch/_load.py
+-rw-r--r--  2.0 unx     3286 b- defN 23-May-31 17:03 determined/pytorch/_lr_scheduler.py
+-rw-r--r--  2.0 unx     8275 b- defN 23-May-31 17:03 determined/pytorch/_metric_utils.py
+-rw-r--r--  2.0 unx    45136 b- defN 23-May-31 17:03 determined/pytorch/_pytorch_context.py
+-rw-r--r--  2.0 unx    68474 b- defN 23-May-31 17:03 determined/pytorch/_pytorch_trial.py
+-rw-r--r--  2.0 unx    21406 b- defN 23-May-31 17:03 determined/pytorch/_reducer.py
+-rw-r--r--  2.0 unx    13510 b- defN 23-May-31 17:03 determined/pytorch/_trainer.py
+-rw-r--r--  2.0 unx     9561 b- defN 23-May-31 17:03 determined/pytorch/samplers.py
+-rw-r--r--  2.0 unx      347 b- defN 23-May-31 17:03 determined/pytorch/deepspeed/__init__.py
+-rw-r--r--  2.0 unx    17164 b- defN 23-May-31 17:03 determined/pytorch/deepspeed/_deepspeed_context.py
+-rw-r--r--  2.0 unx    43712 b- defN 23-May-31 17:03 determined/pytorch/deepspeed/_deepspeed_trial.py
+-rw-r--r--  2.0 unx     1987 b- defN 23-May-31 17:03 determined/pytorch/deepspeed/_mpu.py
+-rw-r--r--  2.0 unx      409 b- defN 23-May-31 17:03 determined/pytorch/dsat/__init__.py
+-rw-r--r--  2.0 unx     1738 b- defN 23-May-31 17:03 determined/pytorch/dsat/__main__.py
+-rw-r--r--  2.0 unx     2541 b- defN 23-May-31 17:03 determined/pytorch/dsat/_defaults.py
+-rw-r--r--  2.0 unx    60199 b- defN 23-May-31 17:03 determined/pytorch/dsat/_dsat_search_method.py
+-rw-r--r--  2.0 unx     3736 b- defN 23-May-31 17:03 determined/pytorch/dsat/_run_dsat.py
+-rw-r--r--  2.0 unx    20100 b- defN 23-May-31 17:03 determined/pytorch/dsat/_utils.py
+-rw-r--r--  2.0 unx       67 b- defN 23-May-31 17:03 determined/pytorch/lightning/__init__.py
+-rw-r--r--  2.0 unx    18157 b- defN 23-May-31 17:03 determined/pytorch/lightning/_adapter.py
+-rw-r--r--  2.0 unx      343 b- defN 23-May-31 17:03 determined/searcher/__init__.py
+-rw-r--r--  2.0 unx     4051 b- defN 23-May-31 17:03 determined/searcher/_remote_search_runner.py
+-rw-r--r--  2.0 unx    16443 b- defN 23-May-31 17:03 determined/searcher/_search_method.py
+-rw-r--r--  2.0 unx    15851 b- defN 23-May-31 17:03 determined/searcher/_search_runner.py
+-rw-r--r--  2.0 unx      512 b- defN 23-May-31 17:03 determined/tensorboard/__init__.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-May-31 17:03 determined/tensorboard/azure.py
+-rw-r--r--  2.0 unx     5884 b- defN 23-May-31 17:03 determined/tensorboard/base.py
+-rw-r--r--  2.0 unx     4008 b- defN 23-May-31 17:03 determined/tensorboard/build.py
+-rw-r--r--  2.0 unx     2305 b- defN 23-May-31 17:03 determined/tensorboard/gcs.py
+-rw-r--r--  2.0 unx     1892 b- defN 23-May-31 17:03 determined/tensorboard/s3.py
+-rw-r--r--  2.0 unx     1747 b- defN 23-May-31 17:03 determined/tensorboard/shared.py
+-rw-r--r--  2.0 unx     3734 b- defN 23-May-31 17:03 determined/tensorboard/util.py
+-rw-r--r--  2.0 unx      780 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/azure.py
+-rw-r--r--  2.0 unx     1670 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/base.py
+-rw-r--r--  2.0 unx     1733 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/gcs.py
+-rw-r--r--  2.0 unx     2476 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/s3.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-31 17:03 determined/tensorboard/fetchers/shared.py
+-rw-r--r--  2.0 unx       91 b- defN 23-May-31 17:03 determined/tensorboard/metric_writers/__init__.py
+-rw-r--r--  2.0 unx     2113 b- defN 23-May-31 17:03 determined/tensorboard/metric_writers/callback.py
+-rw-r--r--  2.0 unx     2936 b- defN 23-May-31 17:03 determined/tensorboard/metric_writers/pytorch.py
+-rw-r--r--  2.0 unx     4385 b- defN 23-May-31 17:03 determined/tensorboard/metric_writers/tensorflow.py
+-rw-r--r--  2.0 unx       70 b- defN 23-May-31 17:03 determined/transformers/__init__.py
+-rw-r--r--  2.0 unx    12727 b- defN 23-May-31 17:03 determined/transformers/_hf_callback.py
+-rw-r--r--  2.0 unx     1232 b- defN 23-May-31 17:03 determined-0.23.0rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 17:03 determined-0.23.0rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-May-31 17:03 determined-0.23.0rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-31 17:03 determined-0.23.0rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    23615 b- defN 23-May-31 17:03 determined-0.23.0rc0.dist-info/RECORD
+257 files, 2533413 bytes uncompressed, 569811 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -276,17 +276,14 @@
 
 Filename: determined/common/storage/cloud.py
 Comment: 
 
 Filename: determined/common/storage/gcs.py
 Comment: 
 
-Filename: determined/common/storage/hdfs.py
-Comment: 
-
 Filename: determined/common/storage/s3.py
 Comment: 
 
 Filename: determined/common/storage/shared.py
 Comment: 
 
 Filename: determined/core/__init__.py
@@ -378,14 +375,17 @@
 
 Filename: determined/deploy/aws/templates/govcloud.yaml
 Comment: 
 
 Filename: determined/deploy/aws/templates/secure.yaml
 Comment: 
 
+Filename: determined/deploy/aws/templates/simple-rds.yaml
+Comment: 
+
 Filename: determined/deploy/aws/templates/simple.yaml
 Comment: 
 
 Filename: determined/deploy/gcp/__init__.py
 Comment: 
 
 Filename: determined/deploy/gcp/cli.py
@@ -555,14 +555,17 @@
 
 Filename: determined/experimental/_native.py
 Comment: 
 
 Filename: determined/experimental/client.py
 Comment: 
 
+Filename: determined/experimental/unmanaged.py
+Comment: 
+
 Filename: determined/keras/__init__.py
 Comment: 
 
 Filename: determined/keras/_data.py
 Comment: 
 
 Filename: determined/keras/_enqueuer.py
@@ -651,14 +654,32 @@
 
 Filename: determined/pytorch/deepspeed/_deepspeed_trial.py
 Comment: 
 
 Filename: determined/pytorch/deepspeed/_mpu.py
 Comment: 
 
+Filename: determined/pytorch/dsat/__init__.py
+Comment: 
+
+Filename: determined/pytorch/dsat/__main__.py
+Comment: 
+
+Filename: determined/pytorch/dsat/_defaults.py
+Comment: 
+
+Filename: determined/pytorch/dsat/_dsat_search_method.py
+Comment: 
+
+Filename: determined/pytorch/dsat/_run_dsat.py
+Comment: 
+
+Filename: determined/pytorch/dsat/_utils.py
+Comment: 
+
 Filename: determined/pytorch/lightning/__init__.py
 Comment: 
 
 Filename: determined/pytorch/lightning/_adapter.py
 Comment: 
 
 Filename: determined/searcher/__init__.py
@@ -684,17 +705,14 @@
 
 Filename: determined/tensorboard/build.py
 Comment: 
 
 Filename: determined/tensorboard/gcs.py
 Comment: 
 
-Filename: determined/tensorboard/hdfs.py
-Comment: 
-
 Filename: determined/tensorboard/s3.py
 Comment: 
 
 Filename: determined/tensorboard/shared.py
 Comment: 
 
 Filename: determined/tensorboard/util.py
@@ -726,23 +744,29 @@
 
 Filename: determined/tensorboard/metric_writers/pytorch.py
 Comment: 
 
 Filename: determined/tensorboard/metric_writers/tensorflow.py
 Comment: 
 
-Filename: determined-0.22.2rc1.dist-info/METADATA
+Filename: determined/transformers/__init__.py
+Comment: 
+
+Filename: determined/transformers/_hf_callback.py
+Comment: 
+
+Filename: determined-0.23.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: determined-0.22.2rc1.dist-info/WHEEL
+Filename: determined-0.23.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: determined-0.22.2rc1.dist-info/entry_points.txt
+Filename: determined-0.23.0rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: determined-0.22.2rc1.dist-info/top_level.txt
+Filename: determined-0.23.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: determined-0.22.2rc1.dist-info/RECORD
+Filename: determined-0.23.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.22.2-rc1"
+__version__ = "0.23.0-rc0"
```

## determined/util.py

```diff
@@ -1,9 +1,10 @@
 import collections
 import contextlib
+import copy
 import datetime
 import enum
 import errno
 import inspect
 import json
 import logging
 import math
@@ -132,14 +133,28 @@
     for i in range(list_len):
         for k in dict_of_lists.keys():
             output_list[i][k] = dict_of_lists[k][i]
 
     return output_list
 
 
+def merge_dicts(base_dict: Dict[Any, Any], source_dict: Dict[Any, Any]) -> Dict[Any, Any]:
+    """
+    Recursively replace and merge values from source_dict into base_dict. Returns a new
+    dictionary, leaving both inputs unmodified.
+    """
+    merged_dict = copy.deepcopy(base_dict)
+    for key, value in source_dict.items():
+        if key in base_dict and isinstance(value, dict):
+            merged_dict[key] = merge_dicts(base_dict[key], value)
+        else:
+            merged_dict[key] = value
+    return merged_dict
+
+
 def validate_batch_metrics(batch_metrics: List[Dict[str, Any]]) -> None:
     metric_dict = _list_to_dict(batch_metrics)
 
     # We expect that all batches have the same set of metrics.
     metric_dict_keys = metric_dict.keys()
     for idx, metric_dict in zip(range(len(batch_metrics)), batch_metrics):
         keys = metric_dict.keys()
```

## determined/cli/__init__.py

```diff
@@ -2,14 +2,15 @@
     output_format_args,
     make_pagination_args,
     default_pagination_args,
     setup_session,
     require_feature_flag,
     login_sdk_client,
     print_warnings,
+    wait_ntsc_ready,
 )
 from determined.cli import (
     agent,
     checkpoint,
     cli,
     command,
     experiment,
```

## determined/cli/_util.py

```diff
@@ -1,14 +1,15 @@
 import argparse
 import functools
 import sys
 from typing import Any, Callable, Dict, List, Sequence
 
 import termcolor
 
+from determined.cli import errors, render
 from determined.common import api, declarative_argparse, util
 from determined.common.api import authentication, bindings, certs
 from determined.experimental import client
 
 from .errors import FeatureFlagDisabled
 
 output_format_args: Dict[str, declarative_argparse.Arg] = {
@@ -114,7 +115,20 @@
 
     return decorator
 
 
 def print_warnings(warnings: Sequence[bindings.v1LaunchWarning]) -> None:
     for warning in warnings:
         print(termcolor.colored(api.WARNING_MESSAGE_MAP[warning], "yellow"), file=sys.stderr)
+
+
+def wait_ntsc_ready(session: api.Session, ntsc_type: api.NTSC_Kind, eid: str) -> None:
+    """
+    Use to wait for a notebook, tensorboard, or shell command to become ready.
+    """
+    name = ntsc_type.value
+    loading_animator = render.Animator(f"Waiting for {name} to become ready")
+    err_msg = api.task_is_ready(session, eid, loading_animator.next)
+    msg = f"{name} (id: {eid}) is ready." if not err_msg else f"Waiting stopped: {err_msg}"
+    loading_animator.clear(msg)
+    if err_msg:
+        raise errors.CliError(err_msg)
```

## determined/cli/checkpoint.py

```diff
@@ -77,15 +77,15 @@
         "Resources",
         "Size",
     ]
     values = [
         [
             c.training.trialId,
             c.metadata.get("steps_completed", None),
-            c.state.value.replace("STATE_", "") if c.state is not None else "UNSPECIFIED",
+            c.state,
             get_validation_metric(c, searcher_metric),
             c.uuid,
             render.format_resources(c.resources),
             render.format_resource_sizes(c.resources),
         ]
         for c in checkpoints
     ]
@@ -119,15 +119,36 @@
         "with each checkpoint in the checkpoint storage. Do you still want to proceed?"
     ):
         c_uuids = args.checkpoints_uuids.split(",")
         delete_body = bindings.v1DeleteCheckpointsRequest(checkpointUuids=c_uuids)
         bindings.delete_DeleteCheckpoints(cli.setup_session(args), body=delete_body)
         print("Deletion of checkpoints {} is in progress".format(args.checkpoints_uuids))
     else:
-        print("Aborting deletion of checkpoints.")
+        print("Stopping deletion of checkpoints.")
+
+
+@authentication.required
+def checkpoints_file_rm(args: Namespace) -> None:
+    if (
+        args.yes
+        or len(args.glob) == 0
+        or render.yes_or_no(
+            "All files matching specified globs will be deleted in all checkpoints provided\n"
+            "in checkpoint storage. Do you still want to proceed?"
+        )
+    ):
+        c_uuids = args.checkpoints_uuids.split(",")
+        remove_body = bindings.v1CheckpointsRemoveFilesRequest(
+            checkpointGlobs=args.glob,
+            checkpointUuids=c_uuids,
+        )
+        bindings.post_CheckpointsRemoveFiles(cli.setup_session(args), body=remove_body)
+        print(f"Removal of files from checkpoints {args.checkpoints_uuids} is in progress")
+    else:
+        print("Stopping removal of files from checkpoints.")
 
 
 main_cmd = Cmd(
     "c|heckpoint",
     None,
     "manage checkpoints",
     [
@@ -179,11 +200,36 @@
                 Arg(
                     "--yes",
                     action="store_true",
                     default=False,
                     help="automatically answer yes to prompts",
                 ),
             ],
+        ),
+        Cmd(
+            "rm",
+            checkpoints_file_rm,
+            "remove files from checkpoints",
+            [
+                Arg(
+                    "checkpoints_uuids",
+                    help="comma-separated list of checkpoints to remove files from",
+                ),
+                Arg(
+                    "--glob",
+                    action="append",
+                    default=[],
+                    help="glob to specify which files will be deleted, if unspecified no files "
+                    + "will be deleted and checkpoint resources will "
+                    + "be read from storage and refreshed",
+                ),
+                Arg(
+                    "--yes",
+                    action="store_true",
+                    default=False,
+                    help="automatically answer yes to prompts",
+                ),
+            ],
         ),
     ],
 )
 args_description = [main_cmd]  # type: List[Any]
```

## determined/cli/cli.py

```diff
@@ -308,9 +308,9 @@
     except KeyboardInterrupt:
         # die() may not be defined yet.
         if debug_mode():
             import traceback
 
             traceback.print_exc(file=sys.stderr)
 
-        print(colored("Interrupting...\n", "red"), file=sys.stderr)
+        print(colored("\nInterrupting...\n", "red"), file=sys.stderr)
         exit(3)
```

## determined/cli/command.py

```diff
@@ -394,32 +394,7 @@
         body["workspaceId"] = workspace_id
 
     return api.post(
         master,
         endpoint,
         body,
     ).json()
-
-
-def render_event_stream(event: Any) -> None:
-    description = event["description"]
-    if event["scheduled_event"] is not None:
-        print(
-            colored("Scheduling {} (id: {})...".format(description, event["parent_id"]), "yellow")
-        )
-    elif event["assigned_event"] is not None:
-        print(colored("{} was assigned to an agent...".format(description), "green"))
-    elif event["resources_started_event"] is not None:
-        print(colored("Resources for {} has started...".format(description), "green"))
-    elif event["service_ready_event"] is not None:
-        pass  # Ignore this message.
-    elif event["terminate_request_event"] is not None:
-        print(colored("{} was requested to terminate...".format(description), "red"))
-    elif event["exited_event"] is not None:
-        # TODO: Non-success exit statuses should be red
-        stat = event["exited_event"]
-        print(colored("{} was terminated: {}".format(description, stat), "green"))
-        pass
-    elif event["log_event"] is not None:
-        print(event["log_event"], flush=True)
-    else:
-        raise ValueError("unexpected event: {}".format(event))
```

## determined/cli/experiment.py

```diff
@@ -373,15 +373,15 @@
         "Archived",
         "Resource Pool",
         "Labels",
     ]
     values: List[List] = [
         [
             exp.id,
-            exp.state.value.replace("STATE_", ""),
+            exp.state,
             render.format_percent(exp.progress),
             render.format_time(exp.startTime),
             render.format_time(exp.endTime),
             exp.name,
             exp.description,
             exp.archived,
             exp.resourcePool,
```

## determined/cli/master.py

```diff
@@ -23,15 +23,15 @@
         determined.cli.render.print_json(resp.to_json())
     else:
         print(yaml.safe_dump(resp.to_json(), default_flow_style=False))
 
 
 def format_log_entry(log: bindings.v1LogEntry) -> str:
     """Format v1LogEntry for printing."""
-    log_level = str(log.level.value)[len("LOG_LEVEL_") :] if log.level else ""
+    log_level = log.level if log.level else ""
     return f"{log.timestamp} [{log_level}]: {log.message}"
 
 
 @authentication.required
 def logs(args: Namespace) -> None:
     offset: Optional[int] = None
     if args.tail:
```

## determined/cli/notebook.py

```diff
@@ -36,36 +36,37 @@
 
     nb = resp.notebook
 
     if args.detach:
         print(nb.id)
         return
 
+    render.report_job_launched("notebook", resp.notebook.id)
+
     if resp.warnings:
         cli.print_warnings(resp.warnings)
     currentSlotsExceeded = (resp.warnings is not None) and (
         bindings.v1LaunchWarning.CURRENT_SLOTS_EXCEEDED in resp.warnings
     )
 
-    with api.ws(args.master, "notebooks/{}/events".format(nb.id)) as ws:
-        for msg in ws:
-            if msg["service_ready_event"] and nb.serviceAddress and not args.no_browser:
-                url = api.browser_open(
-                    args.master,
-                    request.make_interactive_task_url(
-                        task_id=nb.id,
-                        service_address=nb.serviceAddress,
-                        description=nb.description,
-                        resource_pool=nb.resourcePool,
-                        task_type="jupyter-lab",
-                        currentSlotsExceeded=currentSlotsExceeded,
-                    ),
-                )
-                print(colored("Jupyter Notebook is running at: {}".format(url), "green"))
-            command.render_event_stream(msg)
+    cli.wait_ntsc_ready(cli.setup_session(args), api.NTSC_Kind.notebook, nb.id)
+
+    assert nb.serviceAddress is not None, "missing tensorboard serviceAddress"
+    nb_path = request.make_interactive_task_url(
+        task_id=nb.id,
+        service_address=nb.serviceAddress,
+        description=nb.description,
+        resource_pool=nb.resourcePool,
+        task_type="jupyter-lab",
+        currentSlotsExceeded=currentSlotsExceeded,
+    )
+    url = api.make_url(args.master, nb_path)
+    if not args.no_browser:
+        api.browser_open(args.master, nb_path)
+    print(colored("Jupyter Notebook is running at: {}".format(url), "green"))
 
 
 @authentication.required
 def open_notebook(args: Namespace) -> None:
     notebook_id = command.expand_uuid_prefixes(args)
     resp = api.get(args.master, "api/v1/notebooks/{}".format(notebook_id)).json()["notebook"]
     check_eq(resp["state"], "STATE_RUNNING", "Notebook must be in a running state")
```

## determined/cli/project.py

```diff
@@ -15,15 +15,15 @@
 def render_experiments(args: Namespace, experiments: Sequence[bindings.v1Experiment]) -> None:
     def format_experiment(e: bindings.v1Experiment) -> List[Any]:
         result = [
             e.id,
             e.username,
             e.name,
             e.forkedFrom,
-            e.state.value.replace("STATE_", ""),
+            e.state,
             render.format_percent(e.progress),
             render.format_time(e.startTime),
             render.format_time(e.endTime),
             e.resourcePool,
         ]
         if args.all:
             result.append(e.archived)
```

## determined/cli/remote.py

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 from pathlib import Path
 from typing import Any, List
 
 from termcolor import colored
 
 from determined import cli
-from determined.cli import command, task
+from determined.cli import command, render, task
 from determined.common import api
 from determined.common.api import authentication
 from determined.common.declarative_argparse import Arg, Cmd, Group
 
 
 @authentication.required
 def run_command(args: Namespace) -> None:
@@ -26,14 +26,16 @@
         workspace_id=workspace_id,
     )["command"]
 
     if args.detach:
         print(resp["id"])
         return
 
+    render.report_job_launched("command", resp["id"])
+
     try:
         logs = api.task_logs(cli.setup_session(args), resp["id"], follow=True)
         api.pprint_logs(logs)
     finally:
         print(
             colored(
                 "Task log stream ended. To reopen log stream, run: "
```

## determined/cli/render.py

```diff
@@ -5,14 +5,15 @@
 import pathlib
 import sys
 from datetime import timezone
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
 import dateutil.parser
 import tabulate
+import termcolor
 
 from determined.common import util, yaml
 
 # Avoid reporting BrokenPipeError when piping `tabulate` output through
 # a filter like `head`.
 _FORMAT = "presto"
 _DEFAULT_VALUE = "N/A"
@@ -40,14 +41,47 @@
     init_args = {}
     for arg in spec.args[1:]:
         transform = transforms.get(arg, lambda x: x)
         init_args[arg] = transform(data[arg])
     return class_(**init_args)
 
 
+class Animator:
+    """
+    Animator is a simple class for rendering a loading animation in the terminal.
+    Use to communicate progress to the user when a call may take a while.
+    """
+
+    MAX_LINE_LENGTH = 80
+
+    def __init__(self, message: str = "Loading") -> None:
+        self.message = message
+        self.step = 0
+
+    def next(self) -> None:
+        self.render_frame(self.step, self.message)
+        self.step += 1
+
+    @staticmethod
+    def render_frame(step: int, message: str) -> None:
+        animation = "|/-\\"
+        sys.stdout.write("\r" + message + " " + animation[step % len(animation)] + " ")
+        sys.stdout.flush()
+
+    def reset(self) -> None:
+        self.clear()
+        self.step = 0
+
+    @staticmethod
+    def clear(message: str = "Loading done.") -> None:
+        sys.stdout.write("\r" + " " * Animator.MAX_LINE_LENGTH + "\r")
+        sys.stdout.write("\r" + message + "\n")
+        sys.stdout.flush()
+
+
 def render_objects(
     generic: Any, values: Iterable[Any], default_value: str = "N/A", table_fmt: str = _FORMAT
 ) -> None:
     keys = inspect.getfullargspec(generic).args[1:]
     headers = [key.replace("_", " ").title() for key in keys]
     if len(headers) == 0:
         raise ValueError("must have at least one header to display")
@@ -158,7 +192,12 @@
     try:
         if isinstance(data, str):
             data = json.loads(data)
         formatted_json = json.dumps(data, sort_keys=True, indent=2)
         print(formatted_json)
     except json.decoder.JSONDecodeError:
         print(data)
+
+
+def report_job_launched(_type: str, _id: str) -> None:
+    msg = f"Launched {_type} (id: {_id})."
+    print(termcolor.colored(msg, "green"))
```

## determined/cli/shell.py

```diff
@@ -11,17 +11,17 @@
 from pathlib import Path
 from typing import IO, Any, ContextManager, Dict, Iterator, List, Tuple, Union
 
 import appdirs
 from termcolor import colored
 
 from determined import cli
-from determined.cli import command, task
+from determined.cli import command, render, task
 from determined.common import api
-from determined.common.api import authentication, certs
+from determined.common.api import authentication, bindings, certs
 from determined.common.check import check_eq
 from determined.common.declarative_argparse import Arg, Cmd, Group
 
 
 @authentication.required
 def start_shell(args: Namespace) -> None:
     data = {}
@@ -37,56 +37,52 @@
         args.template,
         context_path=args.context,
         includes=args.include,
         data=data,
         workspace_id=workspace_id,
     )["shell"]
 
+    sid = resp["id"]
+
     if args.detach:
-        print(resp["id"])
+        print(sid)
         return
 
-    ready = False
-    with api.ws(args.master, f"shells/{resp['id']}/events") as ws:
-        for msg in ws:
-            if msg["service_ready_event"]:
-                ready = True
-                break
-            command.render_event_stream(msg)
-    if ready:
-        shell = api.get(args.master, f"api/v1/shells/{resp['id']}").json()["shell"]
-        check_eq(shell["state"], "STATE_RUNNING", "Shell must be in a running state")
-        _open_shell(
-            args.master,
-            shell,
-            args.ssh_opts,
-            retain_keys_and_print=args.show_ssh_command,
-            print_only=False,
-        )
+    render.report_job_launched("shell", sid)
+
+    session = cli.setup_session(args)
+    cli.wait_ntsc_ready(cli.setup_session(args), api.NTSC_Kind.shell, sid)
+
+    shell = bindings.get_GetShell(session, shellId=sid).shell
+    _open_shell(
+        args.master,
+        shell.to_json(),
+        args.ssh_opts,
+        retain_keys_and_print=args.show_ssh_command,
+        print_only=False,
+    )
 
 
 @authentication.required
 def open_shell(args: Namespace) -> None:
     shell_id = command.expand_uuid_prefixes(args)
     shell = api.get(args.master, f"api/v1/shells/{shell_id}").json()["shell"]
-    check_eq(shell["state"], "STATE_RUNNING", "Shell must be in a running state")
     _open_shell(
         args.master,
         shell,
         args.ssh_opts,
         retain_keys_and_print=args.show_ssh_command,
         print_only=False,
     )
 
 
 @authentication.required
 def show_ssh_command(args: Namespace) -> None:
     shell_id = command.expand_uuid_prefixes(args)
     shell = api.get(args.master, f"api/v1/shells/{shell_id}").json()["shell"]
-    check_eq(shell["state"], "STATE_RUNNING", "Shell must be in a running state")
     _open_shell(args.master, shell, args.ssh_opts, retain_keys_and_print=True, print_only=True)
 
 
 def _prepare_key(retention_dir: Union[Path, None]) -> Tuple[ContextManager[IO], str]:
     if retention_dir:
         key_path = retention_dir / "key"
         keyfile = key_path.open("w")
@@ -128,14 +124,15 @@
     master: str,
     shell: Dict[str, Any],
     additional_opts: List[str],
     retain_keys_and_print: bool,
     print_only: bool,
 ) -> None:
     cache_dir = None
+    check_eq(shell["state"], "STATE_RUNNING", "Shell must be in a running state")
     if retain_keys_and_print:
         cache_dir = Path(appdirs.user_cache_dir("determined")) / "shell" / shell["id"]
         if not cache_dir.exists():
             cache_dir.mkdir(parents=True)
 
     f, keypath = _prepare_key(cache_dir)
     with f as keyfile:
```

## determined/cli/task.py

```diff
@@ -114,14 +114,17 @@
     Arg(
         "-f",
         "--follow",
         action="store_true",
         help="follow the logs of a running task, similar to tail -f",
     ),
     Group(
+        cli.output_format_args["json"],
+    ),
+    Group(
         Arg(
             "--head",
             type=int,
             help="number of lines to show, counting from the beginning of the log",
         ),
         Arg(
             "--tail",
@@ -207,14 +210,13 @@
                 # Since declarative argparse tries to attach the help_str to the func itself:
                 # ./harness/determined/common/declarative_argparse.py#L57
                 # Each func must be unique.
                 partial(logs),
                 "fetch task logs",
                 [
                     Arg("task_id", help="task ID"),
-                    cli.output_format_args["json"],
                     *common_log_options,
                 ],
             ),
         ],
     ),
 ]
```

## determined/cli/tensorboard.py

```diff
@@ -1,15 +1,15 @@
 from argparse import ONE_OR_MORE, ArgumentError, FileType, Namespace
 from functools import partial
 from pathlib import Path
 
 from termcolor import colored
 
 from determined import cli
-from determined.cli import command, task
+from determined.cli import command, render, task
 from determined.common import api, context
 from determined.common.api import authentication, bindings, request
 from determined.common.check import check_eq
 from determined.common.declarative_argparse import Arg, ArgsDescription, Cmd, Group
 
 
 @authentication.required
@@ -26,53 +26,42 @@
         trialIds=args.trial_ids,
         experimentIds=args.experiment_ids,
         files=context.read_v1_context(args.context, args.include),
         workspaceId=workspace_id,
     )
 
     resp = bindings.post_LaunchTensorboard(cli.setup_session(args), body=body)
+    tsb = resp.tensorboard
 
     if args.detach:
         print(resp.tensorboard.id)
         return
 
+    render.report_job_launched("tensorboard", tsb.id)
+
     if resp.warnings:
         cli.print_warnings(resp.warnings)
     currentSlotsExceeded = (resp.warnings is not None) and (
         bindings.v1LaunchWarning.CURRENT_SLOTS_EXCEEDED in resp.warnings
     )
-    url = "tensorboard/{}/events".format(resp.tensorboard.id)
-    with api.ws(args.master, url) as ws:
-        for msg in ws:
-            if msg["log_event"] is not None:
-                # TensorBoard will print a url by default. The URL is incorrect since
-                # TensorBoard is not aware of the master proxy address it is assigned.
-                if "http" in msg["log_event"]:
-                    continue
-
-            if msg["service_ready_event"] and resp.tensorboard.serviceAddress is not None:
-                if args.no_browser:
-                    url = api.make_url(args.master, resp.tensorboard.serviceAddress)
-                else:
-                    url = api.browser_open(
-                        args.master,
-                        request.make_interactive_task_url(
-                            task_id=resp.tensorboard.id,
-                            service_address=resp.tensorboard.serviceAddress,
-                            resource_pool=resp.tensorboard.resourcePool,
-                            description=resp.tensorboard.description,
-                            task_type="tensorboard",
-                            currentSlotsExceeded=currentSlotsExceeded,
-                        ),
-                    )
-
-                print(colored("TensorBoard is running at: {}".format(url), "green"))
-                command.render_event_stream(msg)
-                break
-            command.render_event_stream(msg)
+    cli.wait_ntsc_ready(cli.setup_session(args), api.NTSC_Kind.tensorboard, tsb.id)
+
+    assert tsb.serviceAddress is not None, "missing tensorboard serviceAddress"
+    nb_path = request.make_interactive_task_url(
+        task_id=tsb.id,
+        service_address=tsb.serviceAddress,
+        description=tsb.description,
+        resource_pool=tsb.resourcePool,
+        task_type="tensorboard",
+        currentSlotsExceeded=currentSlotsExceeded,
+    )
+    url = api.make_url(args.master, nb_path)
+    if not args.no_browser:
+        api.browser_open(args.master, nb_path)
+    print(colored("Tensorboard is running at: {}".format(url), "green"))
 
 
 @authentication.required
 def open_tensorboard(args: Namespace) -> None:
     tensorboard_id = command.expand_uuid_prefixes(args)
     resp = api.get(args.master, "api/v1/tensorboards/{}".format(tensorboard_id)).json()[
         "tensorboard"
```

## determined/cli/trial.py

```diff
@@ -8,15 +8,15 @@
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from termcolor import colored
 
 from determined import cli
 from determined.cli import render
 from determined.cli.master import format_log_entry
-from determined.common import api, constants
+from determined.common import api
 from determined.common.api import authentication, bindings
 from determined.common.declarative_argparse import Arg, ArgsDescription, Cmd, Group
 from determined.common.experimental import Determined
 
 from .checkpoint import render_checkpoint
 
 
@@ -24,37 +24,35 @@
     container: bindings.v1WorkloadContainer,
 ) -> Union[bindings.v1MetricsWorkload, bindings.v1CheckpointWorkload]:
     result = container.training or container.validation or container.checkpoint
     assert result is not None
     return result
 
 
-def _format_state(state: Union[bindings.checkpointv1State, bindings.experimentv1State]) -> str:
-    return str(state.value).replace("STATE_", "")
-
-
 def _format_validation(validation: Optional[bindings.v1MetricsWorkload]) -> Optional[str]:
     if not validation:
         return None
 
     return json.dumps(validation.metrics.to_json(), indent=4)
 
 
 def _format_checkpoint(checkpoint: Optional[bindings.v1CheckpointWorkload]) -> List[Any]:
     if not checkpoint:
         return [None, None, None]
 
-    state = _format_state(checkpoint.state)
-    if state in (constants.COMPLETED, constants.DELETED):
+    if checkpoint.state in (
+        bindings.checkpointv1State.COMPLETED,
+        bindings.checkpointv1State.DELETED,
+    ):
         return [
-            state,
+            checkpoint.state,
             checkpoint.uuid,
             json.dumps(checkpoint.metadata, indent=4),
         ]
-    elif state in (constants.ACTIVE, constants.ERROR):
+    elif checkpoint.state in (bindings.checkpointv1State.ACTIVE, bindings.checkpointv1State.ERROR):
         return [checkpoint.state, None, json.dumps(checkpoint.metadata, indent=4)]
     else:
         raise AssertionError("Invalid checkpoint state: {}".format(checkpoint.state))
 
 
 def _workloads_tabulate(
     workloads: Sequence[bindings.v1WorkloadContainer], metrics: bool
```

## determined/cli/user.py

```diff
@@ -1,17 +1,17 @@
 import getpass
 from argparse import Namespace
 from collections import namedtuple
 from typing import Any, List
 
 from termcolor import colored
 
-from determined.cli import login_sdk_client
+from determined.cli import login_sdk_client, setup_session
 from determined.common import api
-from determined.common.api import authentication, certs
+from determined.common.api import authentication, bindings, certs
 from determined.common.declarative_argparse import Arg, Cmd
 from determined.experimental import client
 
 from . import render
 
 FullUser = namedtuple(
     "FullUser",
@@ -23,19 +23,36 @@
         "remote",
         "agent_uid",
         "agent_gid",
         "agent_user",
         "agent_group",
     ],
 )
+FullUserNoAdmin = namedtuple(
+    "FullUserNoAdmin",
+    [
+        "user_id",
+        "username",
+        "active",
+        "remote",
+        "agent_uid",
+        "agent_gid",
+        "agent_user",
+        "agent_group",
+    ],
+)
 
 
 @login_sdk_client
 def list_users(args: Namespace) -> None:
-    render.render_objects(FullUser, client.list_users())
+    resp = bindings.get_GetMaster(setup_session(args))
+    if resp.to_json().get("rbacEnabled"):
+        render.render_objects(FullUserNoAdmin, client.list_users())
+    else:
+        render.render_objects(FullUser, client.list_users())
 
 
 @login_sdk_client
 def activate_user(parsed_args: Namespace) -> None:
     user_obj = client.get_user_by_name(parsed_args.username)
     user_obj.activate()
```

## determined/common/constants.py

```diff
@@ -23,20 +23,14 @@
 MAX_METRICS_SIZE = 100 * (1 << 20)
 
 # The username and password for the default user.
 DEFAULT_DETERMINED_USER = "determined"
 DEFAULT_DETERMINED_PASSWORD = ""
 DEFAULT_CHECKPOINT_PATH = "checkpoints"
 
-ACTIVE = "ACTIVE"
-CANCELED = "CANCELED"
-COMPLETED = "COMPLETED"
-DELETED = "DELETED"
-ERROR = "ERROR"
-
 SHARED_FS_CONTAINER_PATH = "/determined_shared_fs"
 
 # By default, we ignore:
 #  - all byte-compiled Python files to ignore a potential stale compilation
 #  - terraform files generated by `det deploy gcp`, e.g. when user creates
 #    a cluster from the (tutorial) model def directory.
 #  - .git and IDE-related content
```

## determined/common/util.py

```diff
@@ -3,21 +3,23 @@
 import io
 import json
 import os
 import pathlib
 import platform
 import random
 import sys
+import time
 from typing import (
     IO,
     Any,
     Callable,
     Iterator,
     Optional,
     Sequence,
+    Tuple,
     TypeVar,
     Union,
     no_type_check,
     overload,
 )
 
 import urllib3
@@ -196,7 +198,25 @@
     # notably does not handle the trailing Z to signify the UTC timezone [2].
     #
     # [1] https://tc39.es/ecma262/#sec-date-time-string-format
     # [2] https://bugs.python.org/issue35829
     if ts.endswith("Z"):
         ts = ts[:-1] + "+00:00"
     return datetime.datetime.fromisoformat(ts)
+
+
+def wait_for(
+    predicate: Callable[[], Tuple[bool, T]], timeout: int = 60, interval: float = 0.1
+) -> T:
+    """
+    Wait for the predicate to return (Done, ReturnValue) while
+    checking for a timeout. without preempting the predicate.
+    """
+
+    start = time.time()
+    done = False
+    while not done:
+        if time.time() - start > timeout:
+            raise TimeoutError("timed out waiting for predicate")
+        done, rv = predicate()
+        time.sleep(interval)
+    return rv
```

## determined/common/api/__init__.py

```diff
@@ -1,11 +1,17 @@
-from determined.common.api import authentication, errors, metric, request
+from determined.common.api import authentication, errors, metric, request, bindings
 from determined.common.api._session import Session
-from determined.common.api import bindings
-from determined.common.api._util import PageOpts, read_paginated, WARNING_MESSAGE_MAP
+from determined.common.api._util import (
+    PageOpts,
+    read_paginated,
+    WARNING_MESSAGE_MAP,
+    wait_for_ntsc_state,
+    task_is_ready,
+    NTSC_Kind,
+)
 from determined.common.api.authentication import Authentication, salt_and_hash
 from determined.common.api.logs import (
     pprint_logs,
     trial_logs,
     task_logs,
 )
 from determined.common.api.request import (
```

## determined/common/api/_util.py

```diff
@@ -1,13 +1,15 @@
 import enum
-import time
-from typing import Callable, Iterator, Optional, TypeVar, Union
+from typing import Callable, Iterator, Optional, Tuple, TypeVar, Union
 
+from determined.common import api, util
 from determined.common.api import Session, bindings
 
+# from determined.cli.render import Animator
+
 
 class PageOpts(str, enum.Enum):
     single = "1"
     all = "all"
 
 
 # Not that read_paginated requires the output of get_with_offset to be a Paginated type to work.
@@ -67,18 +69,44 @@
 
 def wait_for_ntsc_state(
     session: Session,
     typ: NTSC_Kind,
     ntsc_id: str,
     predicate: Callable[[bindings.taskv1State], bool],
     timeout: int = 10,  # seconds
-) -> Optional[bindings.taskv1State]:
+) -> bindings.taskv1State:
     """wait for ntsc to reach a state that satisfies the predicate"""
-    start = time.time()
-    last_state = None
-    while True:
-        if time.time() - start > timeout:
-            raise Exception(f"timed out waiting for state predicate to pass. reached {last_state}")
+
+    def get_state() -> Tuple[bool, bindings.taskv1State]:
         last_state = get_ntsc_details(session, typ, ntsc_id).state
-        if predicate(last_state):
-            return last_state
-        time.sleep(0.5)
+        return predicate(last_state), last_state
+
+    return util.wait_for(get_state, timeout)
+
+
+def task_is_ready(
+    session: api.Session, task_id: str, progress_report: Optional[Callable] = None
+) -> Optional[str]:
+    """
+    wait until a task is ready
+    return: None if task is ready, otherwise return an error message
+    """
+
+    def _task_is_done_loading() -> Tuple[bool, Optional[str]]:
+        task = bindings.get_GetTask(session, taskId=task_id).task
+        if progress_report:
+            progress_report()
+        assert task is not None, "task must not be present."
+        if len(task.allocations) == 0:
+            return False, None
+
+        is_ready = task.allocations[0].isReady
+        if is_ready:
+            return True, None
+
+        if task.endTime is not None:
+            return True, "task has been terminated."
+
+        return False, ""
+
+    err_msg = util.wait_for(_task_is_done_loading, timeout=300, interval=1)
+    return err_msg
```

## determined/common/api/bindings.py

```diff
@@ -1,11 +1,12 @@
 # Code generated by generate_bindings.py. DO NOT EDIT.
 import enum
 import json
 import math
+import os
 import typing
 
 import requests
 
 if typing.TYPE_CHECKING:
     from determined.common import api
 
@@ -51,24 +52,61 @@
             f"Stream Error during {operation_name}: {error.message}"
         )
 
     def __str__(self) -> str:
         return self.message
 
 
-class GetMasterResponseProduct(enum.Enum):
+class DetEnum(enum.Enum):
+    def __str__(self) -> str:
+        skip = len(self.prefix())
+        return f"{self.value[skip:]}"
+    @classmethod
+    def prefix(cls) -> str:
+        prefix: str = os.path.commonprefix([e.value for e in cls])
+        return prefix if prefix.endswith("_") else ""
+
+
+
+class GetMasterResponseProduct(DetEnum):
     UNSPECIFIED = "PRODUCT_UNSPECIFIED"
     COMMUNITY = "PRODUCT_COMMUNITY"
 
-class GetTrialWorkloadsRequestFilterOption(enum.Enum):
+class GetTrialWorkloadsRequestFilterOption(DetEnum):
     UNSPECIFIED = "FILTER_OPTION_UNSPECIFIED"
     CHECKPOINT = "FILTER_OPTION_CHECKPOINT"
     VALIDATION = "FILTER_OPTION_VALIDATION"
     CHECKPOINT_OR_VALIDATION = "FILTER_OPTION_CHECKPOINT_OR_VALIDATION"
 
+class PatchCheckpointOptionalResources:
+    resources: "typing.Optional[typing.Dict[str, str]]" = None
+
+    def __init__(
+        self,
+        *,
+        resources: "typing.Union[typing.Dict[str, str], None, Unset]" = _unset,
+    ):
+        if not isinstance(resources, Unset):
+            self.resources = resources
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "PatchCheckpointOptionalResources":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+        }
+        if "resources" in obj:
+            kwargs["resources"] = obj["resources"]
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+        }
+        if not omit_unset or "resources" in vars(self):
+            out["resources"] = self.resources
+        return out
+
 class PatchExperimentPatchCheckpointStorage:
     saveExperimentBest: "typing.Optional[int]" = None
     saveTrialBest: "typing.Optional[int]" = None
     saveTrialLatest: "typing.Optional[int]" = None
 
     def __init__(
         self,
@@ -205,21 +243,21 @@
         }
         if not omit_unset or "rank" in vars(self):
             out["rank"] = self.rank
         if not omit_unset or "sorter" in vars(self):
             out["sorter"] = None if self.sorter is None else self.sorter.to_json(omit_unset)
         return out
 
-class TrialProfilerMetricLabelsProfilerMetricType(enum.Enum):
+class TrialProfilerMetricLabelsProfilerMetricType(DetEnum):
     UNSPECIFIED = "PROFILER_METRIC_TYPE_UNSPECIFIED"
     SYSTEM = "PROFILER_METRIC_TYPE_SYSTEM"
     TIMING = "PROFILER_METRIC_TYPE_TIMING"
     MISC = "PROFILER_METRIC_TYPE_MISC"
 
-class TrialSorterNamespace(enum.Enum):
+class TrialSorterNamespace(DetEnum):
     UNSPECIFIED = "NAMESPACE_UNSPECIFIED"
     HPARAMS = "NAMESPACE_HPARAMS"
     TRAINING_METRICS = "NAMESPACE_TRAINING_METRICS"
     VALIDATION_METRICS = "NAMESPACE_VALIDATION_METRICS"
 
 class UpdateTrialTagsRequestIds:
     ids: "typing.Optional[typing.Sequence[int]]" = None
@@ -243,36 +281,37 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
         }
         if not omit_unset or "ids" in vars(self):
             out["ids"] = self.ids
         return out
 
-class checkpointv1State(enum.Enum):
+class checkpointv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     ACTIVE = "STATE_ACTIVE"
     COMPLETED = "STATE_COMPLETED"
     ERROR = "STATE_ERROR"
     DELETED = "STATE_DELETED"
+    PARTIALLY_DELETED = "STATE_PARTIALLY_DELETED"
 
-class containerv1State(enum.Enum):
+class containerv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     ASSIGNED = "STATE_ASSIGNED"
     PULLING = "STATE_PULLING"
     STARTING = "STATE_STARTING"
     RUNNING = "STATE_RUNNING"
     TERMINATED = "STATE_TERMINATED"
 
-class devicev1Type(enum.Enum):
+class devicev1Type(DetEnum):
     UNSPECIFIED = "TYPE_UNSPECIFIED"
     CPU = "TYPE_CPU"
     CUDA = "TYPE_CUDA"
     ROCM = "TYPE_ROCM"
 
-class experimentv1State(enum.Enum):
+class experimentv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     ACTIVE = "STATE_ACTIVE"
     PAUSED = "STATE_PAUSED"
     STOPPING_COMPLETED = "STATE_STOPPING_COMPLETED"
     STOPPING_CANCELED = "STATE_STOPPING_CANCELED"
     STOPPING_ERROR = "STATE_STOPPING_ERROR"
     COMPLETED = "STATE_COMPLETED"
@@ -283,21 +322,21 @@
     DELETE_FAILED = "STATE_DELETE_FAILED"
     STOPPING_KILLED = "STATE_STOPPING_KILLED"
     QUEUED = "STATE_QUEUED"
     PULLING = "STATE_PULLING"
     STARTING = "STATE_STARTING"
     RUNNING = "STATE_RUNNING"
 
-class jobv1State(enum.Enum):
+class jobv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     QUEUED = "STATE_QUEUED"
     SCHEDULED = "STATE_SCHEDULED"
     SCHEDULED_BACKFILLED = "STATE_SCHEDULED_BACKFILLED"
 
-class jobv1Type(enum.Enum):
+class jobv1Type(DetEnum):
     UNSPECIFIED = "TYPE_UNSPECIFIED"
     EXPERIMENT = "TYPE_EXPERIMENT"
     NOTEBOOK = "TYPE_NOTEBOOK"
     TENSORBOARD = "TYPE_TENSORBOARD"
     SHELL = "TYPE_SHELL"
     COMMAND = "TYPE_COMMAND"
     CHECKPOINT_GC = "TYPE_CHECKPOINT_GC"
@@ -332,15 +371,15 @@
         }
         if not omit_unset or "typeUrl" in vars(self):
             out["typeUrl"] = self.typeUrl
         if not omit_unset or "value" in vars(self):
             out["value"] = self.value
         return out
 
-class protobufNullValue(enum.Enum):
+class protobufNullValue(DetEnum):
     NULL_VALUE = "NULL_VALUE"
 
 class runtimeError:
     code: "typing.Optional[int]" = None
     details: "typing.Optional[typing.Sequence[protobufAny]]" = None
     error: "typing.Optional[str]" = None
     message: "typing.Optional[str]" = None
@@ -443,25 +482,25 @@
             out["httpCode"] = self.httpCode
         if not omit_unset or "httpStatus" in vars(self):
             out["httpStatus"] = self.httpStatus
         if not omit_unset or "message" in vars(self):
             out["message"] = self.message
         return out
 
-class taskv1State(enum.Enum):
+class taskv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     PULLING = "STATE_PULLING"
     STARTING = "STATE_STARTING"
     RUNNING = "STATE_RUNNING"
     TERMINATED = "STATE_TERMINATED"
     TERMINATING = "STATE_TERMINATING"
     WAITING = "STATE_WAITING"
     QUEUED = "STATE_QUEUED"
 
-class trialv1State(enum.Enum):
+class trialv1State(DetEnum):
     UNSPECIFIED = "STATE_UNSPECIFIED"
     ACTIVE = "STATE_ACTIVE"
     PAUSED = "STATE_PAUSED"
     STOPPING_CANCELED = "STATE_STOPPING_CANCELED"
     STOPPING_KILLED = "STATE_STOPPING_KILLED"
     STOPPING_COMPLETED = "STATE_STOPPING_COMPLETED"
     STOPPING_ERROR = "STATE_STOPPING_ERROR"
@@ -673,15 +712,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "results": [x.to_json(omit_unset) for x in self.results],
         }
         return out
 
-class v1ActivityType(enum.Enum):
+class v1ActivityType(DetEnum):
     UNSPECIFIED = "ACTIVITY_TYPE_UNSPECIFIED"
     GET = "ACTIVITY_TYPE_GET"
 
 class v1AddProjectNoteResponse:
 
     def __init__(
         self,
@@ -920,77 +959,61 @@
         out: "typing.Dict[str, typing.Any]" = {
             "periodStart": self.periodStart,
             "seconds": dump_float(self.seconds),
         }
         return out
 
 class v1Allocation:
-    allocationId: "typing.Optional[str]" = None
     endTime: "typing.Optional[str]" = None
-    isReady: "typing.Optional[bool]" = None
     startTime: "typing.Optional[str]" = None
-    state: "typing.Optional[taskv1State]" = None
-    taskId: "typing.Optional[str]" = None
 
     def __init__(
         self,
         *,
-        allocationId: "typing.Union[str, None, Unset]" = _unset,
+        allocationId: str,
+        isReady: bool,
+        state: "taskv1State",
+        taskId: str,
         endTime: "typing.Union[str, None, Unset]" = _unset,
-        isReady: "typing.Union[bool, None, Unset]" = _unset,
         startTime: "typing.Union[str, None, Unset]" = _unset,
-        state: "typing.Union[taskv1State, None, Unset]" = _unset,
-        taskId: "typing.Union[str, None, Unset]" = _unset,
     ):
-        if not isinstance(allocationId, Unset):
-            self.allocationId = allocationId
+        self.allocationId = allocationId
+        self.isReady = isReady
+        self.state = state
+        self.taskId = taskId
         if not isinstance(endTime, Unset):
             self.endTime = endTime
-        if not isinstance(isReady, Unset):
-            self.isReady = isReady
         if not isinstance(startTime, Unset):
             self.startTime = startTime
-        if not isinstance(state, Unset):
-            self.state = state
-        if not isinstance(taskId, Unset):
-            self.taskId = taskId
 
     @classmethod
     def from_json(cls, obj: Json) -> "v1Allocation":
         kwargs: "typing.Dict[str, typing.Any]" = {
+            "allocationId": obj["allocationId"],
+            "isReady": obj["isReady"],
+            "state": taskv1State(obj["state"]),
+            "taskId": obj["taskId"],
         }
-        if "allocationId" in obj:
-            kwargs["allocationId"] = obj["allocationId"]
         if "endTime" in obj:
             kwargs["endTime"] = obj["endTime"]
-        if "isReady" in obj:
-            kwargs["isReady"] = obj["isReady"]
         if "startTime" in obj:
             kwargs["startTime"] = obj["startTime"]
-        if "state" in obj:
-            kwargs["state"] = taskv1State(obj["state"]) if obj["state"] is not None else None
-        if "taskId" in obj:
-            kwargs["taskId"] = obj["taskId"]
         return cls(**kwargs)
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
+            "allocationId": self.allocationId,
+            "isReady": self.isReady,
+            "state": self.state.value,
+            "taskId": self.taskId,
         }
-        if not omit_unset or "allocationId" in vars(self):
-            out["allocationId"] = self.allocationId
         if not omit_unset or "endTime" in vars(self):
             out["endTime"] = self.endTime
-        if not omit_unset or "isReady" in vars(self):
-            out["isReady"] = self.isReady
         if not omit_unset or "startTime" in vars(self):
             out["startTime"] = self.startTime
-        if not omit_unset or "state" in vars(self):
-            out["state"] = None if self.state is None else self.state.value
-        if not omit_unset or "taskId" in vars(self):
-            out["taskId"] = self.taskId
         return out
 
 class v1AllocationAllGatherRequest:
     numPeers: "typing.Optional[int]" = None
     requestUuid: "typing.Optional[str]" = None
 
     def __init__(
@@ -1827,14 +1850,40 @@
             out["metadata"] = self.metadata
         if not omit_unset or "resources" in vars(self):
             out["resources"] = self.resources
         if not omit_unset or "uuid" in vars(self):
             out["uuid"] = self.uuid
         return out
 
+class v1CheckpointsRemoveFilesRequest:
+
+    def __init__(
+        self,
+        *,
+        checkpointGlobs: "typing.Sequence[str]",
+        checkpointUuids: "typing.Sequence[str]",
+    ):
+        self.checkpointGlobs = checkpointGlobs
+        self.checkpointUuids = checkpointUuids
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1CheckpointsRemoveFilesRequest":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+            "checkpointGlobs": obj["checkpointGlobs"],
+            "checkpointUuids": obj["checkpointUuids"],
+        }
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+            "checkpointGlobs": self.checkpointGlobs,
+            "checkpointUuids": self.checkpointUuids,
+        }
+        return out
+
 class v1CloseTrialOperation:
     requestId: "typing.Optional[str]" = None
 
     def __init__(
         self,
         *,
         requestId: "typing.Union[str, None, Unset]" = _unset,
@@ -1887,15 +1936,15 @@
         }
         if not omit_unset or "filter" in vars(self):
             out["filter"] = None if self.filter is None else self.filter.to_json(omit_unset)
         if not omit_unset or "name" in vars(self):
             out["name"] = self.name
         return out
 
-class v1ColumnType(enum.Enum):
+class v1ColumnType(DetEnum):
     UNSPECIFIED = "COLUMN_TYPE_UNSPECIFIED"
     TEXT = "COLUMN_TYPE_TEXT"
     NUMBER = "COLUMN_TYPE_NUMBER"
     DATE = "COLUMN_TYPE_DATE"
 
 class v1Command:
     container: "typing.Optional[v1Container]" = None
@@ -2110,14 +2159,15 @@
     gitCommitDate: "typing.Optional[str]" = None
     gitCommitter: "typing.Optional[str]" = None
     gitRemote: "typing.Optional[str]" = None
     modelDefinition: "typing.Optional[typing.Sequence[v1File]]" = None
     parentId: "typing.Optional[int]" = None
     projectId: "typing.Optional[int]" = None
     template: "typing.Optional[str]" = None
+    unmanaged: "typing.Optional[bool]" = None
     validateOnly: "typing.Optional[bool]" = None
 
     def __init__(
         self,
         *,
         activate: "typing.Union[bool, None, Unset]" = _unset,
         config: "typing.Union[str, None, Unset]" = _unset,
@@ -2125,14 +2175,15 @@
         gitCommitDate: "typing.Union[str, None, Unset]" = _unset,
         gitCommitter: "typing.Union[str, None, Unset]" = _unset,
         gitRemote: "typing.Union[str, None, Unset]" = _unset,
         modelDefinition: "typing.Union[typing.Sequence[v1File], None, Unset]" = _unset,
         parentId: "typing.Union[int, None, Unset]" = _unset,
         projectId: "typing.Union[int, None, Unset]" = _unset,
         template: "typing.Union[str, None, Unset]" = _unset,
+        unmanaged: "typing.Union[bool, None, Unset]" = _unset,
         validateOnly: "typing.Union[bool, None, Unset]" = _unset,
     ):
         if not isinstance(activate, Unset):
             self.activate = activate
         if not isinstance(config, Unset):
             self.config = config
         if not isinstance(gitCommit, Unset):
@@ -2147,14 +2198,16 @@
             self.modelDefinition = modelDefinition
         if not isinstance(parentId, Unset):
             self.parentId = parentId
         if not isinstance(projectId, Unset):
             self.projectId = projectId
         if not isinstance(template, Unset):
             self.template = template
+        if not isinstance(unmanaged, Unset):
+            self.unmanaged = unmanaged
         if not isinstance(validateOnly, Unset):
             self.validateOnly = validateOnly
 
     @classmethod
     def from_json(cls, obj: Json) -> "v1CreateExperimentRequest":
         kwargs: "typing.Dict[str, typing.Any]" = {
         }
@@ -2174,14 +2227,16 @@
             kwargs["modelDefinition"] = [v1File.from_json(x) for x in obj["modelDefinition"]] if obj["modelDefinition"] is not None else None
         if "parentId" in obj:
             kwargs["parentId"] = obj["parentId"]
         if "projectId" in obj:
             kwargs["projectId"] = obj["projectId"]
         if "template" in obj:
             kwargs["template"] = obj["template"]
+        if "unmanaged" in obj:
+            kwargs["unmanaged"] = obj["unmanaged"]
         if "validateOnly" in obj:
             kwargs["validateOnly"] = obj["validateOnly"]
         return cls(**kwargs)
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
         }
@@ -2201,14 +2256,16 @@
             out["modelDefinition"] = None if self.modelDefinition is None else [x.to_json(omit_unset) for x in self.modelDefinition]
         if not omit_unset or "parentId" in vars(self):
             out["parentId"] = self.parentId
         if not omit_unset or "projectId" in vars(self):
             out["projectId"] = self.projectId
         if not omit_unset or "template" in vars(self):
             out["template"] = self.template
+        if not omit_unset or "unmanaged" in vars(self):
+            out["unmanaged"] = self.unmanaged
         if not omit_unset or "validateOnly" in vars(self):
             out["validateOnly"] = self.validateOnly
         return out
 
 class v1CreateExperimentResponse:
     warnings: "typing.Optional[typing.Sequence[v1LaunchWarning]]" = None
 
@@ -2325,14 +2382,78 @@
         }
         if not omit_unset or "hyperparams" in vars(self):
             out["hyperparams"] = self.hyperparams
         if not omit_unset or "requestId" in vars(self):
             out["requestId"] = self.requestId
         return out
 
+class v1CreateTrialRequest:
+    experimentId: "typing.Optional[int]" = None
+    hparams: "typing.Optional[typing.Dict[str, typing.Any]]" = None
+    unmanaged: "typing.Optional[bool]" = None
+
+    def __init__(
+        self,
+        *,
+        experimentId: "typing.Union[int, None, Unset]" = _unset,
+        hparams: "typing.Union[typing.Dict[str, typing.Any], None, Unset]" = _unset,
+        unmanaged: "typing.Union[bool, None, Unset]" = _unset,
+    ):
+        if not isinstance(experimentId, Unset):
+            self.experimentId = experimentId
+        if not isinstance(hparams, Unset):
+            self.hparams = hparams
+        if not isinstance(unmanaged, Unset):
+            self.unmanaged = unmanaged
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1CreateTrialRequest":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+        }
+        if "experimentId" in obj:
+            kwargs["experimentId"] = obj["experimentId"]
+        if "hparams" in obj:
+            kwargs["hparams"] = obj["hparams"]
+        if "unmanaged" in obj:
+            kwargs["unmanaged"] = obj["unmanaged"]
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+        }
+        if not omit_unset or "experimentId" in vars(self):
+            out["experimentId"] = self.experimentId
+        if not omit_unset or "hparams" in vars(self):
+            out["hparams"] = self.hparams
+        if not omit_unset or "unmanaged" in vars(self):
+            out["unmanaged"] = self.unmanaged
+        return out
+
+class v1CreateTrialResponse:
+
+    def __init__(
+        self,
+        *,
+        trial: "trialv1Trial",
+    ):
+        self.trial = trial
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1CreateTrialResponse":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+            "trial": trialv1Trial.from_json(obj["trial"]),
+        }
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+            "trial": self.trial.to_json(omit_unset),
+        }
+        return out
+
 class v1CreateTrialsCollectionRequest:
 
     def __init__(
         self,
         *,
         filters: "v1TrialFilters",
         name: str,
@@ -2873,15 +2994,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
         }
         if not omit_unset or "slot" in vars(self):
             out["slot"] = None if self.slot is None else self.slot.to_json(omit_unset)
         return out
 
-class v1EntityType(enum.Enum):
+class v1EntityType(DetEnum):
     UNSPECIFIED = "ENTITY_TYPE_UNSPECIFIED"
     PROJECT = "ENTITY_TYPE_PROJECT"
 
 class v1ExpMetricNamesResponse:
     searcherMetrics: "typing.Optional[typing.Sequence[str]]" = None
     trainingMetrics: "typing.Optional[typing.Sequence[str]]" = None
     validationMetrics: "typing.Optional[typing.Sequence[str]]" = None
@@ -2926,23 +3047,25 @@
 class v1Experiment:
     bestTrialId: "typing.Optional[int]" = None
     bestTrialSearcherMetric: "typing.Optional[float]" = None
     checkpointCount: "typing.Optional[int]" = None
     checkpointSize: "typing.Optional[str]" = None
     description: "typing.Optional[str]" = None
     displayName: "typing.Optional[str]" = None
+    duration: "typing.Optional[int]" = None
     endTime: "typing.Optional[str]" = None
     forkedFrom: "typing.Optional[int]" = None
     labels: "typing.Optional[typing.Sequence[str]]" = None
     notes: "typing.Optional[str]" = None
     parentArchived: "typing.Optional[bool]" = None
     progress: "typing.Optional[float]" = None
     projectName: "typing.Optional[str]" = None
     resourcePool: "typing.Optional[str]" = None
     trialIds: "typing.Optional[typing.Sequence[int]]" = None
+    unmanaged: "typing.Optional[bool]" = None
     userId: "typing.Optional[int]" = None
     workspaceId: "typing.Optional[int]" = None
     workspaceName: "typing.Optional[str]" = None
 
     def __init__(
         self,
         *,
@@ -2961,23 +3084,25 @@
         username: str,
         bestTrialId: "typing.Union[int, None, Unset]" = _unset,
         bestTrialSearcherMetric: "typing.Union[float, None, Unset]" = _unset,
         checkpointCount: "typing.Union[int, None, Unset]" = _unset,
         checkpointSize: "typing.Union[str, None, Unset]" = _unset,
         description: "typing.Union[str, None, Unset]" = _unset,
         displayName: "typing.Union[str, None, Unset]" = _unset,
+        duration: "typing.Union[int, None, Unset]" = _unset,
         endTime: "typing.Union[str, None, Unset]" = _unset,
         forkedFrom: "typing.Union[int, None, Unset]" = _unset,
         labels: "typing.Union[typing.Sequence[str], None, Unset]" = _unset,
         notes: "typing.Union[str, None, Unset]" = _unset,
         parentArchived: "typing.Union[bool, None, Unset]" = _unset,
         progress: "typing.Union[float, None, Unset]" = _unset,
         projectName: "typing.Union[str, None, Unset]" = _unset,
         resourcePool: "typing.Union[str, None, Unset]" = _unset,
         trialIds: "typing.Union[typing.Sequence[int], None, Unset]" = _unset,
+        unmanaged: "typing.Union[bool, None, Unset]" = _unset,
         userId: "typing.Union[int, None, Unset]" = _unset,
         workspaceId: "typing.Union[int, None, Unset]" = _unset,
         workspaceName: "typing.Union[str, None, Unset]" = _unset,
     ):
         self.archived = archived
         self.config = config
         self.id = id
@@ -2999,14 +3124,16 @@
             self.checkpointCount = checkpointCount
         if not isinstance(checkpointSize, Unset):
             self.checkpointSize = checkpointSize
         if not isinstance(description, Unset):
             self.description = description
         if not isinstance(displayName, Unset):
             self.displayName = displayName
+        if not isinstance(duration, Unset):
+            self.duration = duration
         if not isinstance(endTime, Unset):
             self.endTime = endTime
         if not isinstance(forkedFrom, Unset):
             self.forkedFrom = forkedFrom
         if not isinstance(labels, Unset):
             self.labels = labels
         if not isinstance(notes, Unset):
@@ -3017,14 +3144,16 @@
             self.progress = progress
         if not isinstance(projectName, Unset):
             self.projectName = projectName
         if not isinstance(resourcePool, Unset):
             self.resourcePool = resourcePool
         if not isinstance(trialIds, Unset):
             self.trialIds = trialIds
+        if not isinstance(unmanaged, Unset):
+            self.unmanaged = unmanaged
         if not isinstance(userId, Unset):
             self.userId = userId
         if not isinstance(workspaceId, Unset):
             self.workspaceId = workspaceId
         if not isinstance(workspaceName, Unset):
             self.workspaceName = workspaceName
 
@@ -3053,14 +3182,16 @@
             kwargs["checkpointCount"] = obj["checkpointCount"]
         if "checkpointSize" in obj:
             kwargs["checkpointSize"] = obj["checkpointSize"]
         if "description" in obj:
             kwargs["description"] = obj["description"]
         if "displayName" in obj:
             kwargs["displayName"] = obj["displayName"]
+        if "duration" in obj:
+            kwargs["duration"] = obj["duration"]
         if "endTime" in obj:
             kwargs["endTime"] = obj["endTime"]
         if "forkedFrom" in obj:
             kwargs["forkedFrom"] = obj["forkedFrom"]
         if "labels" in obj:
             kwargs["labels"] = obj["labels"]
         if "notes" in obj:
@@ -3071,14 +3202,16 @@
             kwargs["progress"] = float(obj["progress"]) if obj["progress"] is not None else None
         if "projectName" in obj:
             kwargs["projectName"] = obj["projectName"]
         if "resourcePool" in obj:
             kwargs["resourcePool"] = obj["resourcePool"]
         if "trialIds" in obj:
             kwargs["trialIds"] = obj["trialIds"]
+        if "unmanaged" in obj:
+            kwargs["unmanaged"] = obj["unmanaged"]
         if "userId" in obj:
             kwargs["userId"] = obj["userId"]
         if "workspaceId" in obj:
             kwargs["workspaceId"] = obj["workspaceId"]
         if "workspaceName" in obj:
             kwargs["workspaceName"] = obj["workspaceName"]
         return cls(**kwargs)
@@ -3107,14 +3240,16 @@
             out["checkpointCount"] = self.checkpointCount
         if not omit_unset or "checkpointSize" in vars(self):
             out["checkpointSize"] = self.checkpointSize
         if not omit_unset or "description" in vars(self):
             out["description"] = self.description
         if not omit_unset or "displayName" in vars(self):
             out["displayName"] = self.displayName
+        if not omit_unset or "duration" in vars(self):
+            out["duration"] = self.duration
         if not omit_unset or "endTime" in vars(self):
             out["endTime"] = self.endTime
         if not omit_unset or "forkedFrom" in vars(self):
             out["forkedFrom"] = self.forkedFrom
         if not omit_unset or "labels" in vars(self):
             out["labels"] = self.labels
         if not omit_unset or "notes" in vars(self):
@@ -3125,14 +3260,16 @@
             out["progress"] = None if self.progress is None else dump_float(self.progress)
         if not omit_unset or "projectName" in vars(self):
             out["projectName"] = self.projectName
         if not omit_unset or "resourcePool" in vars(self):
             out["resourcePool"] = self.resourcePool
         if not omit_unset or "trialIds" in vars(self):
             out["trialIds"] = self.trialIds
+        if not omit_unset or "unmanaged" in vars(self):
+            out["unmanaged"] = self.unmanaged
         if not omit_unset or "userId" in vars(self):
             out["userId"] = self.userId
         if not omit_unset or "workspaceId" in vars(self):
             out["workspaceId"] = self.workspaceId
         if not omit_unset or "workspaceName" in vars(self):
             out["workspaceName"] = self.workspaceName
         return out
@@ -3223,15 +3360,15 @@
             out["config"] = self.config
         if not omit_unset or "seed" in vars(self):
             out["seed"] = self.seed
         if not omit_unset or "trials" in vars(self):
             out["trials"] = None if self.trials is None else [x.to_json(omit_unset) for x in self.trials]
         return out
 
-class v1FailureType(enum.Enum):
+class v1FailureType(DetEnum):
     UNSPECIFIED = "FAILURE_TYPE_UNSPECIFIED"
     RESOURCES_FAILED = "FAILURE_TYPE_RESOURCES_FAILED"
     RESOURCES_ABORTED = "FAILURE_TYPE_RESOURCES_ABORTED"
     RESOURCES_MISSING = "FAILURE_TYPE_RESOURCES_MISSING"
     TASK_ABORTED = "FAILURE_TYPE_TASK_ABORTED"
     TASK_ERROR = "FAILURE_TYPE_TASK_ERROR"
     AGENT_FAILED = "FAILURE_TYPE_AGENT_FAILED"
@@ -3355,15 +3492,15 @@
             out["modifiedTime"] = self.modifiedTime
         if not omit_unset or "name" in vars(self):
             out["name"] = self.name
         if not omit_unset or "path" in vars(self):
             out["path"] = self.path
         return out
 
-class v1FittingPolicy(enum.Enum):
+class v1FittingPolicy(DetEnum):
     UNSPECIFIED = "FITTING_POLICY_UNSPECIFIED"
     BEST = "FITTING_POLICY_BEST"
     WORST = "FITTING_POLICY_WORST"
     KUBERNETES = "FITTING_POLICY_KUBERNETES"
     SLURM = "FITTING_POLICY_SLURM"
     PBS = "FITTING_POLICY_PBS"
 
@@ -3419,15 +3556,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "agent": self.agent.to_json(omit_unset),
         }
         return out
 
-class v1GetAgentsRequestSortBy(enum.Enum):
+class v1GetAgentsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     TIME = "SORT_BY_TIME"
 
 class v1GetAgentsResponse:
     pagination: "typing.Optional[v1Pagination]" = None
 
@@ -3528,15 +3665,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "command": self.command.to_json(omit_unset),
             "config": self.config,
         }
         return out
 
-class v1GetCommandsRequestSortBy(enum.Enum):
+class v1GetCommandsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     START_TIME = "SORT_BY_START_TIME"
     WORKSPACE_ID = "SORT_BY_WORKSPACE_ID"
 
 class v1GetCommandsResponse:
@@ -3599,15 +3736,15 @@
         }
         if not omit_unset or "completed" in vars(self):
             out["completed"] = self.completed
         if not omit_unset or "op" in vars(self):
             out["op"] = None if self.op is None else self.op.to_json(omit_unset)
         return out
 
-class v1GetExperimentCheckpointsRequestSortBy(enum.Enum):
+class v1GetExperimentCheckpointsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     UUID = "SORT_BY_UUID"
     TRIAL_ID = "SORT_BY_TRIAL_ID"
     BATCH_NUMBER = "SORT_BY_BATCH_NUMBER"
     END_TIME = "SORT_BY_END_TIME"
     STATE = "SORT_BY_STATE"
     SEARCHER_METRIC = "SORT_BY_SEARCHER_METRIC"
@@ -3690,15 +3827,15 @@
         out: "typing.Dict[str, typing.Any]" = {
             "experiment": self.experiment.to_json(omit_unset),
         }
         if not omit_unset or "jobSummary" in vars(self):
             out["jobSummary"] = None if self.jobSummary is None else self.jobSummary.to_json(omit_unset)
         return out
 
-class v1GetExperimentTrialsRequestSortBy(enum.Enum):
+class v1GetExperimentTrialsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     START_TIME = "SORT_BY_START_TIME"
     END_TIME = "SORT_BY_END_TIME"
     STATE = "SORT_BY_STATE"
     BEST_VALIDATION_METRIC = "SORT_BY_BEST_VALIDATION_METRIC"
     LATEST_VALIDATION_METRIC = "SORT_BY_LATEST_VALIDATION_METRIC"
@@ -3755,15 +3892,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
         }
         if not omit_unset or "validationHistory" in vars(self):
             out["validationHistory"] = None if self.validationHistory is None else [x.to_json(omit_unset) for x in self.validationHistory]
         return out
 
-class v1GetExperimentsRequestSortBy(enum.Enum):
+class v1GetExperimentsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     START_TIME = "SORT_BY_START_TIME"
     END_TIME = "SORT_BY_END_TIME"
     STATE = "SORT_BY_STATE"
     NUM_TRIALS = "SORT_BY_NUM_TRIALS"
@@ -4303,15 +4440,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "modelVersion": self.modelVersion.to_json(omit_unset),
         }
         return out
 
-class v1GetModelVersionsRequestSortBy(enum.Enum):
+class v1GetModelVersionsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     VERSION = "SORT_BY_VERSION"
     CREATION_TIME = "SORT_BY_CREATION_TIME"
 
 class v1GetModelVersionsResponse:
 
     def __init__(
@@ -4338,15 +4475,15 @@
         out: "typing.Dict[str, typing.Any]" = {
             "model": self.model.to_json(omit_unset),
             "modelVersions": [x.to_json(omit_unset) for x in self.modelVersions],
             "pagination": self.pagination.to_json(omit_unset),
         }
         return out
 
-class v1GetModelsRequestSortBy(enum.Enum):
+class v1GetModelsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     NAME = "SORT_BY_NAME"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     CREATION_TIME = "SORT_BY_CREATION_TIME"
     LAST_UPDATED_TIME = "SORT_BY_LAST_UPDATED_TIME"
     NUM_VERSIONS = "SORT_BY_NUM_VERSIONS"
     WORKSPACE = "SORT_BY_WORKSPACE"
@@ -4399,15 +4536,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "config": self.config,
             "notebook": self.notebook.to_json(omit_unset),
         }
         return out
 
-class v1GetNotebooksRequestSortBy(enum.Enum):
+class v1GetNotebooksRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     START_TIME = "SORT_BY_START_TIME"
     WORKSPACE_ID = "SORT_BY_WORKSPACE_ID"
 
 class v1GetNotebooksResponse:
@@ -4718,15 +4855,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "config": self.config,
             "shell": self.shell.to_json(omit_unset),
         }
         return out
 
-class v1GetShellsRequestSortBy(enum.Enum):
+class v1GetShellsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     START_TIME = "SORT_BY_START_TIME"
     WORKSPACE_ID = "SORT_BY_WORKSPACE_ID"
 
 class v1GetShellsResponse:
@@ -4808,37 +4945,33 @@
         out: "typing.Dict[str, typing.Any]" = {
         }
         if not omit_unset or "slots" in vars(self):
             out["slots"] = None if self.slots is None else [x.to_json(omit_unset) for x in self.slots]
         return out
 
 class v1GetTaskResponse:
-    task: "typing.Optional[v1Task]" = None
 
     def __init__(
         self,
         *,
-        task: "typing.Union[v1Task, None, Unset]" = _unset,
+        task: "v1Task",
     ):
-        if not isinstance(task, Unset):
-            self.task = task
+        self.task = task
 
     @classmethod
     def from_json(cls, obj: Json) -> "v1GetTaskResponse":
         kwargs: "typing.Dict[str, typing.Any]" = {
+            "task": v1Task.from_json(obj["task"]),
         }
-        if "task" in obj:
-            kwargs["task"] = v1Task.from_json(obj["task"]) if obj["task"] is not None else None
         return cls(**kwargs)
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
+            "task": self.task.to_json(omit_unset),
         }
-        if not omit_unset or "task" in vars(self):
-            out["task"] = None if self.task is None else self.task.to_json(omit_unset)
         return out
 
 class v1GetTasksResponse:
     allocationIdToSummary: "typing.Optional[typing.Dict[str, v1AllocationSummary]]" = None
 
     def __init__(
         self,
@@ -4911,15 +5044,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "template": self.template.to_json(omit_unset),
         }
         return out
 
-class v1GetTemplatesRequestSortBy(enum.Enum):
+class v1GetTemplatesRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     NAME = "SORT_BY_NAME"
 
 class v1GetTemplatesResponse:
 
     def __init__(
         self,
@@ -4967,15 +5100,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "config": self.config,
             "tensorboard": self.tensorboard.to_json(omit_unset),
         }
         return out
 
-class v1GetTensorboardsRequestSortBy(enum.Enum):
+class v1GetTensorboardsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     START_TIME = "SORT_BY_START_TIME"
     WORKSPACE_ID = "SORT_BY_WORKSPACE_ID"
 
 class v1GetTensorboardsResponse:
@@ -5026,15 +5159,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "metrics": [x.to_json(omit_unset) for x in self.metrics],
         }
         return out
 
-class v1GetTrialCheckpointsRequestSortBy(enum.Enum):
+class v1GetTrialCheckpointsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     UUID = "SORT_BY_UUID"
     BATCH_NUMBER = "SORT_BY_BATCH_NUMBER"
     END_TIME = "SORT_BY_END_TIME"
     STATE = "SORT_BY_STATE"
 
 class v1GetTrialCheckpointsResponse:
@@ -5243,15 +5376,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "settings": [x.to_json(omit_unset) for x in self.settings],
         }
         return out
 
-class v1GetUsersRequestSortBy(enum.Enum):
+class v1GetUsersRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     DISPLAY_NAME = "SORT_BY_DISPLAY_NAME"
     USER_NAME = "SORT_BY_USER_NAME"
     ADMIN = "SORT_BY_ADMIN"
     ACTIVE = "SORT_BY_ACTIVE"
     MODIFIED_TIME = "SORT_BY_MODIFIED_TIME"
     NAME = "SORT_BY_NAME"
@@ -5330,15 +5463,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "webhooks": [x.to_json(omit_unset) for x in self.webhooks],
         }
         return out
 
-class v1GetWorkspaceProjectsRequestSortBy(enum.Enum):
+class v1GetWorkspaceProjectsRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     CREATION_TIME = "SORT_BY_CREATION_TIME"
     LAST_EXPERIMENT_START_TIME = "SORT_BY_LAST_EXPERIMENT_START_TIME"
     NAME = "SORT_BY_NAME"
     DESCRIPTION = "SORT_BY_DESCRIPTION"
     ID = "SORT_BY_ID"
 
@@ -5386,15 +5519,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "workspace": self.workspace.to_json(omit_unset),
         }
         return out
 
-class v1GetWorkspacesRequestSortBy(enum.Enum):
+class v1GetWorkspacesRequestSortBy(DetEnum):
     UNSPECIFIED = "SORT_BY_UNSPECIFIED"
     ID = "SORT_BY_ID"
     NAME = "SORT_BY_NAME"
 
 class v1GetWorkspacesResponse:
 
     def __init__(
@@ -6369,15 +6502,15 @@
             "config": self.config,
             "tensorboard": self.tensorboard.to_json(omit_unset),
         }
         if not omit_unset or "warnings" in vars(self):
             out["warnings"] = None if self.warnings is None else [x.value for x in self.warnings]
         return out
 
-class v1LaunchWarning(enum.Enum):
+class v1LaunchWarning(DetEnum):
     UNSPECIFIED = "LAUNCH_WARNING_UNSPECIFIED"
     CURRENT_SLOTS_EXCEEDED = "LAUNCH_WARNING_CURRENT_SLOTS_EXCEEDED"
 
 class v1ListRolesRequest:
     offset: "typing.Optional[int]" = None
 
     def __init__(
@@ -6429,15 +6562,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "pagination": self.pagination.to_json(omit_unset),
             "roles": [x.to_json(omit_unset) for x in self.roles],
         }
         return out
 
-class v1LocationType(enum.Enum):
+class v1LocationType(DetEnum):
     UNSPECIFIED = "LOCATION_TYPE_UNSPECIFIED"
     EXPERIMENT = "LOCATION_TYPE_EXPERIMENT"
     HYPERPARAMETERS = "LOCATION_TYPE_HYPERPARAMETERS"
     VALIDATIONS = "LOCATION_TYPE_VALIDATIONS"
 
 class v1LogEntry:
 
@@ -6469,15 +6602,15 @@
             "id": self.id,
             "level": self.level.value,
             "message": self.message,
             "timestamp": self.timestamp,
         }
         return out
 
-class v1LogLevel(enum.Enum):
+class v1LogLevel(DetEnum):
     UNSPECIFIED = "LOG_LEVEL_UNSPECIFIED"
     TRACE = "LOG_LEVEL_TRACE"
     DEBUG = "LOG_LEVEL_DEBUG"
     INFO = "LOG_LEVEL_INFO"
     WARNING = "LOG_LEVEL_WARNING"
     ERROR = "LOG_LEVEL_ERROR"
     CRITICAL = "LOG_LEVEL_CRITICAL"
@@ -6616,15 +6749,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
         }
         if not omit_unset or "batches" in vars(self):
             out["batches"] = self.batches
         return out
 
-class v1MetricType(enum.Enum):
+class v1MetricType(DetEnum):
     UNSPECIFIED = "METRIC_TYPE_UNSPECIFIED"
     TRAINING = "METRIC_TYPE_TRAINING"
     VALIDATION = "METRIC_TYPE_VALIDATION"
 
 class v1Metrics:
     batchMetrics: "typing.Optional[typing.Sequence[typing.Dict[str, typing.Any]]]" = None
 
@@ -7245,15 +7378,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "data": self.data,
         }
         return out
 
-class v1OrderBy(enum.Enum):
+class v1OrderBy(DetEnum):
     UNSPECIFIED = "ORDER_BY_UNSPECIFIED"
     ASC = "ORDER_BY_ASC"
     DESC = "ORDER_BY_DESC"
 
 class v1Pagination:
     endIndex: "typing.Optional[int]" = None
     limit: "typing.Optional[int]" = None
@@ -7308,14 +7441,66 @@
             out["offset"] = self.offset
         if not omit_unset or "startIndex" in vars(self):
             out["startIndex"] = self.startIndex
         if not omit_unset or "total" in vars(self):
             out["total"] = self.total
         return out
 
+class v1PatchCheckpoint:
+    resources: "typing.Optional[PatchCheckpointOptionalResources]" = None
+
+    def __init__(
+        self,
+        *,
+        uuid: str,
+        resources: "typing.Union[PatchCheckpointOptionalResources, None, Unset]" = _unset,
+    ):
+        self.uuid = uuid
+        if not isinstance(resources, Unset):
+            self.resources = resources
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1PatchCheckpoint":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+            "uuid": obj["uuid"],
+        }
+        if "resources" in obj:
+            kwargs["resources"] = PatchCheckpointOptionalResources.from_json(obj["resources"]) if obj["resources"] is not None else None
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+            "uuid": self.uuid,
+        }
+        if not omit_unset or "resources" in vars(self):
+            out["resources"] = None if self.resources is None else self.resources.to_json(omit_unset)
+        return out
+
+class v1PatchCheckpointsRequest:
+
+    def __init__(
+        self,
+        *,
+        checkpoints: "typing.Sequence[v1PatchCheckpoint]",
+    ):
+        self.checkpoints = checkpoints
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1PatchCheckpointsRequest":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+            "checkpoints": [v1PatchCheckpoint.from_json(x) for x in obj["checkpoints"]],
+        }
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+            "checkpoints": [x.to_json(omit_unset) for x in self.checkpoints],
+        }
+        return out
+
 class v1PatchExperiment:
     checkpointStorage: "typing.Optional[PatchExperimentPatchCheckpointStorage]" = None
     description: "typing.Optional[str]" = None
     labels: "typing.Optional[typing.Sequence[str]]" = None
     name: "typing.Optional[str]" = None
     notes: "typing.Optional[str]" = None
     resources: "typing.Optional[PatchExperimentPatchResources]" = None
@@ -7996,15 +8181,15 @@
         }
         if not omit_unset or "name" in vars(self):
             out["name"] = self.name
         if not omit_unset or "scopeTypeMask" in vars(self):
             out["scopeTypeMask"] = None if self.scopeTypeMask is None else self.scopeTypeMask.to_json(omit_unset)
         return out
 
-class v1PermissionType(enum.Enum):
+class v1PermissionType(DetEnum):
     UNSPECIFIED = "PERMISSION_TYPE_UNSPECIFIED"
     ADMINISTRATE_USER = "PERMISSION_TYPE_ADMINISTRATE_USER"
     CREATE_EXPERIMENT = "PERMISSION_TYPE_CREATE_EXPERIMENT"
     VIEW_EXPERIMENT_ARTIFACTS = "PERMISSION_TYPE_VIEW_EXPERIMENT_ARTIFACTS"
     VIEW_EXPERIMENT_METADATA = "PERMISSION_TYPE_VIEW_EXPERIMENT_METADATA"
     UPDATE_EXPERIMENT = "PERMISSION_TYPE_UPDATE_EXPERIMENT"
     UPDATE_EXPERIMENT_METADATA = "PERMISSION_TYPE_UPDATE_EXPERIMENT_METADATA"
@@ -9264,14 +9449,40 @@
         out: "typing.Dict[str, typing.Any]" = {
             "addresses": self.addresses,
             "rank": self.rank,
             "slots": self.slots,
         }
         return out
 
+class v1ReportTrialMetricsRequest:
+
+    def __init__(
+        self,
+        *,
+        metrics: "v1TrialMetrics",
+        type: str,
+    ):
+        self.metrics = metrics
+        self.type = type
+
+    @classmethod
+    def from_json(cls, obj: Json) -> "v1ReportTrialMetricsRequest":
+        kwargs: "typing.Dict[str, typing.Any]" = {
+            "metrics": v1TrialMetrics.from_json(obj["metrics"]),
+            "type": obj["type"],
+        }
+        return cls(**kwargs)
+
+    def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
+        out: "typing.Dict[str, typing.Any]" = {
+            "metrics": self.metrics.to_json(omit_unset),
+            "type": self.type,
+        }
+        return out
+
 class v1ResourceAllocationAggregatedEntry:
 
     def __init__(
         self,
         *,
         byAgentLabel: "typing.Dict[str, float]",
         byExperimentLabel: "typing.Dict[str, float]",
@@ -9332,15 +9543,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "resourceEntries": [x.to_json(omit_unset) for x in self.resourceEntries],
         }
         return out
 
-class v1ResourceAllocationAggregationPeriod(enum.Enum):
+class v1ResourceAllocationAggregationPeriod(DetEnum):
     UNSPECIFIED = "RESOURCE_ALLOCATION_AGGREGATION_PERIOD_UNSPECIFIED"
     DAILY = "RESOURCE_ALLOCATION_AGGREGATION_PERIOD_DAILY"
     MONTHLY = "RESOURCE_ALLOCATION_AGGREGATION_PERIOD_MONTHLY"
 
 class v1ResourceAllocationRawEntry:
     endTime: "typing.Optional[str]" = None
     experimentId: "typing.Optional[int]" = None
@@ -9903,15 +10114,15 @@
             "defaultPriority": self.defaultPriority,
             "preemption": self.preemption,
         }
         if not omit_unset or "k8Priorities" in vars(self):
             out["k8Priorities"] = None if self.k8Priorities is None else [x.to_json(omit_unset) for x in self.k8Priorities]
         return out
 
-class v1ResourcePoolType(enum.Enum):
+class v1ResourcePoolType(DetEnum):
     UNSPECIFIED = "RESOURCE_POOL_TYPE_UNSPECIFIED"
     AWS = "RESOURCE_POOL_TYPE_AWS"
     GCP = "RESOURCE_POOL_TYPE_GCP"
     STATIC = "RESOURCE_POOL_TYPE_STATIC"
     K8S = "RESOURCE_POOL_TYPE_K8S"
 
 class v1ResourcesFailure:
@@ -10284,15 +10495,15 @@
         }
         if not omit_unset or "length" in vars(self):
             out["length"] = self.length
         if not omit_unset or "type" in vars(self):
             out["type"] = None if self.type is None else self.type.value
         return out
 
-class v1RunnableType(enum.Enum):
+class v1RunnableType(DetEnum):
     UNSPECIFIED = "RUNNABLE_TYPE_UNSPECIFIED"
     TRAIN = "RUNNABLE_TYPE_TRAIN"
     VALIDATE = "RUNNABLE_TYPE_VALIDATE"
 
 class v1SSOProvider:
 
     def __init__(
@@ -10315,20 +10526,20 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "name": self.name,
             "ssoUrl": self.ssoUrl,
         }
         return out
 
-class v1Scale(enum.Enum):
+class v1Scale(DetEnum):
     UNSPECIFIED = "SCALE_UNSPECIFIED"
     LINEAR = "SCALE_LINEAR"
     LOG = "SCALE_LOG"
 
-class v1SchedulerType(enum.Enum):
+class v1SchedulerType(DetEnum):
     UNSPECIFIED = "SCHEDULER_TYPE_UNSPECIFIED"
     PRIORITY = "SCHEDULER_TYPE_PRIORITY"
     FAIR_SHARE = "SCHEDULER_TYPE_FAIR_SHARE"
     ROUND_ROBIN = "SCHEDULER_TYPE_ROUND_ROBIN"
     KUBERNETES = "SCHEDULER_TYPE_KUBERNETES"
     SLURM = "SCHEDULER_TYPE_SLURM"
     PBS = "SCHEDULER_TYPE_PBS"
@@ -11152,53 +11363,53 @@
         out: "typing.Dict[str, typing.Any]" = {
             "metrics": [x.to_json(omit_unset) for x in self.metrics],
             "trial": self.trial.to_json(omit_unset),
         }
         return out
 
 class v1Task:
-    allocations: "typing.Optional[typing.Sequence[v1Allocation]]" = None
-    taskId: "typing.Optional[str]" = None
-    taskType: "typing.Optional[str]" = None
+    endTime: "typing.Optional[str]" = None
 
     def __init__(
         self,
         *,
-        allocations: "typing.Union[typing.Sequence[v1Allocation], None, Unset]" = _unset,
-        taskId: "typing.Union[str, None, Unset]" = _unset,
-        taskType: "typing.Union[str, None, Unset]" = _unset,
+        allocations: "typing.Sequence[v1Allocation]",
+        startTime: str,
+        taskId: str,
+        taskType: str,
+        endTime: "typing.Union[str, None, Unset]" = _unset,
     ):
-        if not isinstance(allocations, Unset):
-            self.allocations = allocations
-        if not isinstance(taskId, Unset):
-            self.taskId = taskId
-        if not isinstance(taskType, Unset):
-            self.taskType = taskType
+        self.allocations = allocations
+        self.startTime = startTime
+        self.taskId = taskId
+        self.taskType = taskType
+        if not isinstance(endTime, Unset):
+            self.endTime = endTime
 
     @classmethod
     def from_json(cls, obj: Json) -> "v1Task":
         kwargs: "typing.Dict[str, typing.Any]" = {
+            "allocations": [v1Allocation.from_json(x) for x in obj["allocations"]],
+            "startTime": obj["startTime"],
+            "taskId": obj["taskId"],
+            "taskType": obj["taskType"],
         }
-        if "allocations" in obj:
-            kwargs["allocations"] = [v1Allocation.from_json(x) for x in obj["allocations"]] if obj["allocations"] is not None else None
-        if "taskId" in obj:
-            kwargs["taskId"] = obj["taskId"]
-        if "taskType" in obj:
-            kwargs["taskType"] = obj["taskType"]
+        if "endTime" in obj:
+            kwargs["endTime"] = obj["endTime"]
         return cls(**kwargs)
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
+            "allocations": [x.to_json(omit_unset) for x in self.allocations],
+            "startTime": self.startTime,
+            "taskId": self.taskId,
+            "taskType": self.taskType,
         }
-        if not omit_unset or "allocations" in vars(self):
-            out["allocations"] = None if self.allocations is None else [x.to_json(omit_unset) for x in self.allocations]
-        if not omit_unset or "taskId" in vars(self):
-            out["taskId"] = self.taskId
-        if not omit_unset or "taskType" in vars(self):
-            out["taskType"] = self.taskType
+        if not omit_unset or "endTime" in vars(self):
+            out["endTime"] = self.endTime
         return out
 
 class v1TaskLogsFieldsResponse:
     agentIds: "typing.Optional[typing.Sequence[str]]" = None
     allocationIds: "typing.Optional[typing.Sequence[str]]" = None
     containerIds: "typing.Optional[typing.Sequence[str]]" = None
     rankIds: "typing.Optional[typing.Sequence[int]]" = None
@@ -11623,15 +11834,15 @@
 
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "reason": self.reason.value,
         }
         return out
 
-class v1TrialEarlyExitExitedReason(enum.Enum):
+class v1TrialEarlyExitExitedReason(DetEnum):
     UNSPECIFIED = "EXITED_REASON_UNSPECIFIED"
     INVALID_HP = "EXITED_REASON_INVALID_HP"
     INIT_INVALID_HP = "EXITED_REASON_INIT_INVALID_HP"
 
 class v1TrialExitedEarly:
 
     def __init__(
@@ -11654,15 +11865,15 @@
     def to_json(self, omit_unset: bool = False) -> typing.Dict[str, typing.Any]:
         out: "typing.Dict[str, typing.Any]" = {
             "exitedReason": self.exitedReason.value,
             "requestId": self.requestId,
         }
         return out
 
-class v1TrialExitedEarlyExitedReason(enum.Enum):
+class v1TrialExitedEarlyExitedReason(DetEnum):
     UNSPECIFIED = "EXITED_REASON_UNSPECIFIED"
     INVALID_HP = "EXITED_REASON_INVALID_HP"
     USER_REQUESTED_STOP = "EXITED_REASON_USER_REQUESTED_STOP"
     USER_CANCELED = "EXITED_REASON_USER_CANCELED"
 
 class v1TrialFilters:
     endTime: "typing.Optional[v1TimestampFieldFilter]" = None
@@ -12474,15 +12685,15 @@
             out["id"] = self.id
         if not omit_unset or "triggerType" in vars(self):
             out["triggerType"] = None if self.triggerType is None else self.triggerType.value
         if not omit_unset or "webhookId" in vars(self):
             out["webhookId"] = self.webhookId
         return out
 
-class v1TriggerType(enum.Enum):
+class v1TriggerType(DetEnum):
     UNSPECIFIED = "TRIGGER_TYPE_UNSPECIFIED"
     EXPERIMENT_STATE_CHANGE = "TRIGGER_TYPE_EXPERIMENT_STATE_CHANGE"
     METRIC_THRESHOLD_EXCEEDED = "TRIGGER_TYPE_METRIC_THRESHOLD_EXCEEDED"
 
 class v1UnarchiveExperimentsRequest:
     filters: "typing.Optional[v1BulkExperimentFilters]" = None
 
@@ -12955,15 +13166,15 @@
         }
         if not omit_unset or "id" in vars(self):
             out["id"] = self.id
         if not omit_unset or "triggers" in vars(self):
             out["triggers"] = None if self.triggers is None else [x.to_json(omit_unset) for x in self.triggers]
         return out
 
-class v1WebhookType(enum.Enum):
+class v1WebhookType(DetEnum):
     UNSPECIFIED = "WEBHOOK_TYPE_UNSPECIFIED"
     DEFAULT = "WEBHOOK_TYPE_DEFAULT"
     SLACK = "WEBHOOK_TYPE_SLACK"
 
 class v1WorkloadContainer:
     checkpoint: "typing.Optional[v1CheckpointWorkload]" = None
     training: "typing.Optional[v1MetricsWorkload]" = None
@@ -13088,15 +13299,15 @@
             out["agentUserGroup"] = None if self.agentUserGroup is None else self.agentUserGroup.to_json(omit_unset)
         if not omit_unset or "checkpointStorageConfig" in vars(self):
             out["checkpointStorageConfig"] = self.checkpointStorageConfig
         if not omit_unset or "pinnedAt" in vars(self):
             out["pinnedAt"] = self.pinnedAt
         return out
 
-class v1WorkspaceState(enum.Enum):
+class v1WorkspaceState(DetEnum):
     UNSPECIFIED = "WORKSPACE_STATE_UNSPECIFIED"
     DELETING = "WORKSPACE_STATE_DELETING"
     DELETE_FAILED = "WORKSPACE_STATE_DELETE_FAILED"
     DELETED = "WORKSPACE_STATE_DELETED"
 
 def post_AckAllocationPreemptionSignal(
     session: "api.Session",
@@ -13464,14 +13675,34 @@
         timeout=None,
         stream=False,
     )
     if _resp.status_code == 200:
         return v1CancelExperimentsResponse.from_json(_resp.json())
     raise APIHttpError("post_CancelExperiments", _resp)
 
+def post_CheckpointsRemoveFiles(
+    session: "api.Session",
+    *,
+    body: "v1CheckpointsRemoveFilesRequest",
+) -> None:
+    _params = None
+    _resp = session._do_request(
+        method="POST",
+        path="/api/v1/checkpoints/rm",
+        params=_params,
+        json=body.to_json(True),
+        data=None,
+        headers=None,
+        timeout=None,
+        stream=False,
+    )
+    if _resp.status_code == 200:
+        return
+    raise APIHttpError("post_CheckpointsRemoveFiles", _resp)
+
 def get_CompareTrials(
     session: "api.Session",
     *,
     endBatches: "typing.Optional[int]" = None,
     maxDatapoints: "typing.Optional[int]" = None,
     metricIds: "typing.Optional[typing.Sequence[str]]" = None,
     metricNames: "typing.Optional[typing.Sequence[str]]" = None,
@@ -13591,14 +13822,34 @@
         timeout=None,
         stream=False,
     )
     if _resp.status_code == 200:
         return v1CreateGroupResponse.from_json(_resp.json())
     raise APIHttpError("post_CreateGroup", _resp)
 
+def post_CreateTrial(
+    session: "api.Session",
+    *,
+    body: "v1CreateTrialRequest",
+) -> "v1CreateTrialResponse":
+    _params = None
+    _resp = session._do_request(
+        method="POST",
+        path="/api/v1/trials",
+        params=_params,
+        json=body.to_json(True),
+        data=None,
+        headers=None,
+        timeout=None,
+        stream=False,
+    )
+    if _resp.status_code == 200:
+        return v1CreateTrialResponse.from_json(_resp.json())
+    raise APIHttpError("post_CreateTrial", _resp)
+
 def post_CreateTrialsCollection(
     session: "api.Session",
     *,
     body: "v1CreateTrialsCollectionRequest",
 ) -> "v1CreateTrialsCollectionResponse":
     _params = None
     _resp = session._do_request(
@@ -16147,14 +16398,34 @@
         timeout=None,
         stream=False,
     )
     if _resp.status_code == 200:
         return v1NotifyContainerRunningResponse.from_json(_resp.json())
     raise APIHttpError("post_NotifyContainerRunning", _resp)
 
+def patch_PatchCheckpoints(
+    session: "api.Session",
+    *,
+    body: "v1PatchCheckpointsRequest",
+) -> None:
+    _params = None
+    _resp = session._do_request(
+        method="PATCH",
+        path="/api/v1/checkpoints",
+        params=_params,
+        json=body.to_json(True),
+        data=None,
+        headers=None,
+        timeout=None,
+        stream=False,
+    )
+    if _resp.status_code == 200:
+        return
+    raise APIHttpError("patch_PatchCheckpoints", _resp)
+
 def patch_PatchExperiment(
     session: "api.Session",
     *,
     body: "v1PatchExperiment",
     experiment_id: int,
 ) -> "v1PatchExperimentResponse":
     _params = None
@@ -16784,14 +17055,35 @@
         timeout=None,
         stream=False,
     )
     if _resp.status_code == 200:
         return
     raise APIHttpError("post_ReportCheckpoint", _resp)
 
+def post_ReportTrialMetrics(
+    session: "api.Session",
+    *,
+    body: "v1ReportTrialMetricsRequest",
+    metrics_trialId: int,
+) -> None:
+    _params = None
+    _resp = session._do_request(
+        method="POST",
+        path=f"/api/v1/trials/{metrics_trialId}/metrics",
+        params=_params,
+        json=body.to_json(True),
+        data=None,
+        headers=None,
+        timeout=None,
+        stream=False,
+    )
+    if _resp.status_code == 200:
+        return
+    raise APIHttpError("post_ReportTrialMetrics", _resp)
+
 def post_ReportTrialProgress(
     session: "api.Session",
     *,
     body: float,
     trialId: int,
 ) -> None:
     _params = None
```

## determined/common/experimental/checkpoint/_checkpoint.py

```diff
@@ -41,14 +41,15 @@
 
 class CheckpointState(enum.Enum):
     UNSPECIFIED = bindings.checkpointv1State.UNSPECIFIED.value
     ACTIVE = bindings.checkpointv1State.ACTIVE.value
     COMPLETED = bindings.checkpointv1State.COMPLETED.value
     ERROR = bindings.checkpointv1State.ERROR.value
     DELETED = bindings.checkpointv1State.DELETED.value
+    PARTIALLY_DELETED = bindings.checkpointv1State.PARTIALLY_DELETED.value
 
 
 @dataclasses.dataclass
 class CheckpointTrainingMetadata:
     experiment_config: Dict[str, Any]
     experiment_id: int
     trial_id: int
@@ -149,17 +150,20 @@
             path (string, optional): Top level directory to place the
                 checkpoint under. If this parameter is not set, the checkpoint will
                 be downloaded to ``checkpoints/<checkpoint_uuid>`` relative to the
                 current working directory.
             mode (DownloadMode, optional): Governs how a checkpoint is downloaded. Defaults to
                 ``AUTO``.
         """
-        if self.state != CheckpointState.COMPLETED:
+        if (
+            self.state != CheckpointState.COMPLETED
+            and self.state != CheckpointState.PARTIALLY_DELETED
+        ):
             raise errors.CheckpointStateException(
-                "Only COMPLETED checkpoints can be downloaded. "
+                "Only COMPLETED or PARTIALLY_DELETED checkpoints can be downloaded. "
                 f"Checkpoint state: {self.state.value}"
             )
         if path is not None:
             local_ckpt_dir = pathlib.Path(path)
         else:
             local_ckpt_dir = pathlib.Path("checkpoints", self.uuid)
 
@@ -331,14 +335,35 @@
         Master will delete checkpoint and all associated data in the checkpoint storage.
         """
 
         delete_body = bindings.v1DeleteCheckpointsRequest(checkpointUuids=[self.uuid])
         bindings.delete_DeleteCheckpoints(self._session, body=delete_body)
         logging.info(f"Deletion of checkpoint {self.uuid} is in progress.")
 
+    def remove_files(self, globs: List[str]) -> None:
+        """
+        Removes any files from the checkpoint in checkpoint storage that match one or more of
+        the provided ``globs``. The checkpoint resources and state will be updated in master
+        asynchronously to reflect checkpoint storage. If ``globs`` is the empty list then no
+        files will be deleted and the resources and state will only be refreshed in master.
+
+        Arguments:
+            globs (List[string]): Globs to match checkpoint files against.
+        """
+        remove_body = bindings.v1CheckpointsRemoveFilesRequest(
+            checkpointGlobs=globs,
+            checkpointUuids=[self.uuid],
+        )
+        bindings.post_CheckpointsRemoveFiles(self._session, body=remove_body)
+
+        if len(globs) == 0:
+            logging.info(f"Refresh of checkpoint {self.uuid} is in progress.")
+        else:
+            logging.info(f"Partial deletion of checkpoint {self.uuid} is in progress.")
+
     def __repr__(self) -> str:
         if self.training is not None:
             return (
                 f"Checkpoint(uuid={self.uuid}, task_id={self.task_id},"
                 f" trial_id={self.training.trial_id})"
             )
         else:
```

## determined/common/storage/__init__.py

```diff
@@ -3,15 +3,14 @@
 import uuid
 from typing import Any, Dict, Optional, Type
 
 from .base import StorageManager, Paths, Selector, from_string
 from .cloud import CloudStorageManager
 from .azure import AzureStorageManager
 from .gcs import GCSStorageManager
-from .hdfs import HDFSStorageManager
 from .s3 import S3StorageManager
 from .shared import SharedFSStorageManager
 
 __all__ = [
     "AzureStorageManager",
     "GCSStorageManager",
     "StorageManager",
@@ -21,15 +20,14 @@
 
 
 _STORAGE_MANAGERS = {
     "azure": AzureStorageManager,
     "gcs": GCSStorageManager,
     "s3": S3StorageManager,
     "shared_fs": SharedFSStorageManager,
-    "hdfs": HDFSStorageManager,
 }  # type: Dict[str, Type[StorageManager]]
 
 
 def build(config: Dict[str, Any], container_path: Optional[str]) -> StorageManager:
     """
     Return a checkpoint manager defined by the value of the `type` key in
     the configuration dictionary. Throws a `TypeError` if no storage manager
@@ -98,12 +96,12 @@
             f.write(storage_id)
 
     with manager.restore_path(storage_id) as path:
         with path.joinpath("VALIDATE.txt").open("r") as f:
             if f.read() != storage_id:
                 raise ValueError("Unable to properly load from storage")
 
-    manager.delete(storage_id)
+    manager.delete(storage_id, ["**/*"])
 
 
 def validate_config(config: Dict[str, Any], container_path: Optional[str]) -> None:
     validate_manager(build(config, container_path))
```

## determined/common/storage/azure.py

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import tempfile
-from typing import Optional, Union
+from typing import Dict, List, Optional, Union
 
 from determined import errors
 from determined.common import storage, util
 
 import posixpath  # isort:skip
 
 
@@ -87,13 +87,24 @@
             blob_dir, blob_base = posixpath.split(container_blob)
             self.client.get(blob_dir, blob_base, _dst)
 
         if not found:
             raise errors.CheckpointNotFound(f"Did not find checkpoint {src} in Azure Blob Storage")
 
     @util.preserve_random_state
-    def delete(self, tgt: str) -> None:
+    def delete(self, tgt: str, globs: List[str]) -> Dict[str, int]:
         storage_prefix = tgt
         logging.info(f"Deleting {tgt} from Azure Blob Storage")
 
-        files = self.client.list_files(self.container, file_prefix=storage_prefix)
-        self.client.delete_files(self.container, files)
+        objects = self.client.list_files(self.container, file_prefix=storage_prefix)
+
+        resources = {}
+        if "**/*" not in globs:  # Partial delete case.
+            prefixed_resources = self._apply_globs_to_resources(objects, storage_prefix, globs)
+            for obj in list(objects):
+                if obj in prefixed_resources:
+                    resources[obj.replace(f"{storage_prefix}/", "")] = objects[obj]
+                    del objects[obj]
+
+        self.client.delete_files(self.container, list(objects))
+
+        return resources
```

## determined/common/storage/azure_client.py

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from determined.common import util
 
 # Prevents Azure's HTTP logs from appearing in our trial logs.
 logging.getLogger("azure").setLevel(logging.ERROR)
 
 
@@ -66,14 +66,17 @@
         """Deletes the specified files from the specified container."""
         for file in files:
             self.client.get_blob_client(container_name, file).delete_blob()
 
     @util.preserve_random_state
     def list_files(
         self, container_name: str, file_prefix: Optional[Union[str, Path]] = None
-    ) -> List[str]:
+    ) -> Dict[str, int]:
         """Lists files within the specified container that have the specified file prefix.
         Lists all files if file_prefix is None.
         """
         container = self.client.get_container_client(container_name)
-        files = [blob["name"] for blob in container.list_blobs(name_starts_with=file_prefix)]
+        files = {
+            blob["name"]: blob["size"]
+            for blob in container.list_blobs(name_starts_with=file_prefix)
+        }
         return files
```

## determined/common/storage/base.py

```diff
@@ -1,14 +1,18 @@
 import abc
 import contextlib
+import copy
+import glob
 import os
 import pathlib
+import tempfile
 import urllib
-from typing import Any, Callable, Dict, Iterator, Optional, Set, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Set, Union
 
+from determined import util
 from determined.common import storage
 
 # Paths should be a set of paths relative to the checkpoint root that indicate what paths
 # should be uploaded. A directory should always appear in Paths if any subpath under that directory
 # appears in Paths.
 Paths = Set[str]
 
@@ -126,15 +130,15 @@
         `selector` should be a callable accepting a string parameter, ending in an os.sep if it is a
         directory, and should return True for files/directories that should be downloaded;
         False otherwise.
         """
         pass
 
     @abc.abstractmethod
-    def delete(self, tgt: str) -> None:
+    def delete(self, tgt: str, globs: List[str]) -> Dict[str, int]:
         """
         Delete the stored data from persistent storage.
         """
         pass
 
     @staticmethod
     def _list_directory(root: Union[str, os.PathLike]) -> Dict[str, int]:
@@ -159,14 +163,66 @@
             for f in files:
                 abs_path = os.path.join(cur_path, f)
                 rel_path = os.path.relpath(abs_path, root)
                 result[rel_path] = os.path.getsize(abs_path)
 
         return result
 
+    @staticmethod
+    def _apply_globs_to_resources(
+        file_paths_to_sizes: Dict[str, int],
+        prefix: str,
+        globs: List[str],
+    ) -> Dict[str, int]:
+        """
+        Returns remaining resources after glob has been applied. This is mostly a hack to
+        handle weird differences between glob.glob, fmatch.match, and pathlib.match.
+        We create a checkpoint path with empty files to all be able to use glob.glob across
+        all storage backends.
+        """
+        file_paths_to_sizes = copy.deepcopy(file_paths_to_sizes)
+
+        # Create dummy file system.
+        temp_dir = tempfile.mkdtemp()
+        try:
+            for f in file_paths_to_sizes:
+                path = pathlib.Path(temp_dir).joinpath(f)
+                path.parent.mkdir(parents=True, exist_ok=True)
+                if f.endswith("/"):  # path.is_dir() will return false always.
+                    path.mkdir(exist_ok=True)
+                else:
+                    path.touch()
+
+            # Do deletion so we propogate deletion,
+            # for example deleting `subdir` deletes `sub/text1.txt`.
+            to_delete_dirs = {}
+            to_delete_files = {}
+            for g in globs:
+                for path_str in glob.glob(
+                    f"{pathlib.Path(temp_dir).joinpath(prefix)}/{g}", recursive=True
+                ):
+                    if os.path.isfile(path_str):
+                        to_delete_files[path_str] = True
+                    elif os.path.isdir(path_str):
+                        to_delete_dirs[path_str] = True
+
+            for path_str in to_delete_files:
+                os.remove(path_str)
+            for path_str in to_delete_dirs:
+                util.rmtree_nfs_safe(path_str, ignore_errors=False)
+
+            prefixed_resources = StorageManager._list_directory(temp_dir)
+            for file_path in list(file_paths_to_sizes):
+                if file_path not in prefixed_resources:
+                    del file_paths_to_sizes[file_path]
+        finally:
+            util.rmtree_nfs_safe(temp_dir, ignore_errors=True)
+
+        return file_paths_to_sizes
+
 
 def from_string(shortcut: str) -> StorageManager:
     p: urllib.parse.ParseResult = urllib.parse.urlparse(shortcut)
     if any((p.params, p.query, p.fragment)):
         raise ValueError(f'Malformed checkpoint_storage string "{shortcut}"')
     scheme = p.scheme.lower()
     if scheme in ["", "file"]:
```

## determined/common/storage/gcs.py

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import tempfile
-from typing import Optional, Union, no_type_check
+from typing import Dict, List, Optional, Union, no_type_check
 
 import requests.exceptions
 import urllib3.exceptions
 
 from determined import errors
 from determined.common import storage, util
 from determined.common.storage.s3 import normalize_prefix
@@ -135,14 +135,27 @@
         ) as e:
             raise errors.NoDirectStorageAccess("Unable to access cloud checkpoint storage") from e
 
         if not found:
             raise errors.CheckpointNotFound(f"Did not find checkpoint {path} in GCS")
 
     @util.preserve_random_state
-    def delete(self, storage_id: str) -> None:
+    def delete(self, storage_id: str, globs: List[str]) -> Dict[str, int]:
         prefix = self.get_storage_prefix(storage_id)
         logging.info(f"Deleting checkpoint {prefix} from GCS")
 
-        for blob in self.bucket.list_blobs(prefix=prefix):
-            logging.debug(f"Deleting {blob.name} from GCS")
-            blob.delete()
+        blob_name_to_blob = {obj.name: obj for obj in self.bucket.list_blobs(prefix=prefix)}
+        blob_name_to_size = {obj.name: obj.size for obj in blob_name_to_blob.values()}
+
+        resources = {}
+        if "**/*" not in globs:
+            prefixed_resources = self._apply_globs_to_resources(blob_name_to_size, prefix, globs)
+            for obj in list(blob_name_to_size):
+                if obj in prefixed_resources:
+                    resources[obj.replace(f"{prefix}/", "")] = blob_name_to_size[obj]
+                    del blob_name_to_size[obj]
+
+        for blob_name in blob_name_to_size:
+            logging.debug(f"Deleting {blob_name} from GCS")
+            blob_name_to_blob[blob_name].delete()
+
+        return resources
```

## determined/common/storage/s3.py

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import re
 import tempfile
-from typing import Optional, Union
+from typing import Dict, List, Optional, Union
 
 import requests
 
 from determined import errors
 from determined.common import storage, util
 
 
@@ -145,17 +145,27 @@
         except botocore.exceptions.NoCredentialsError as e:
             raise errors.NoDirectStorageAccess("Unable to access cloud checkpoint storage") from e
 
         if not found:
             raise errors.CheckpointNotFound(f"Did not find {prefix} in S3")
 
     @util.preserve_random_state
-    def delete(self, tgt: str) -> None:
+    def delete(self, tgt: str, globs: List[str]) -> Dict[str, int]:
         prefix = self.get_storage_prefix(tgt)
         logging.info(f"Deleting {prefix} from S3")
 
-        objects = [{"Key": obj.key} for obj in self.bucket.objects.filter(Prefix=prefix)]
+        objects = {obj.key: obj.size for obj in self.bucket.objects.filter(Prefix=prefix)}
+
+        resources = {}
+        if "**/*" not in globs:  # Partial delete case.
+            prefixed_resources = self._apply_globs_to_resources(objects, prefix, globs)
+            for obj in list(objects):
+                if obj in prefixed_resources:
+                    resources[obj.replace(f"{prefix}/", "")] = objects[obj]
+                    del objects[obj]
 
         # S3 delete_objects has a limit of 1000 objects.
-        for chunk in util.chunks(objects, 1000):
+        for chunk in util.chunks([{"Key": o} for o in objects], 1000):
             logging.debug(f"Deleting {len(chunk)} objects from S3")
             self.bucket.delete_objects(Delete={"Objects": chunk})
+
+        return resources
```

## determined/common/storage/shared.py

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import glob
 import logging
 import os
 import pathlib
 import shutil
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
 from determined import errors, util
@@ -165,26 +166,55 @@
             "using the correct configuration value for checkpoint_storage.host_path",
         )
         storage_dir = os.path.join(self._base_path, src)
         if not os.path.exists(storage_dir):
             raise errors.CheckpointNotFound(f"Did not find checkpoint {src} in shared_fs storage")
         yield pathlib.Path(storage_dir)
 
-    def delete(self, tgt: str) -> None:
+    def delete(self, tgt: str, globs: List[str]) -> Dict[str, int]:
         """
         Delete the stored data from persistent storage.
         """
         storage_dir = os.path.join(self._base_path, tgt)
 
         if not os.path.exists(storage_dir):
             logging.info(f"Storage directory does not exist: {storage_dir}")
-            return
+            return {}
         if not os.path.isdir(storage_dir):
             raise errors.CheckpointNotFound(f"Storage path is not a directory: {storage_dir}")
-        util.rmtree_nfs_safe(storage_dir, ignore_errors=False)
+
+        # Optimize for the common case here. No need to iterate through files.
+        if "**/*" in globs:
+            util.rmtree_nfs_safe(storage_dir, ignore_errors=False)
+            return {}
+
+        to_delete_dirs = {}
+        to_delete_files = {}
+        for file_glob in globs:
+            for path in glob.glob(f"{storage_dir}/{file_glob}", recursive=True):
+                if os.path.commonpath([storage_dir, os.path.normpath(path)]) != storage_dir:
+                    logging.warning(f"tried to delete path outside checkpoint dir {path}")
+                    continue
+
+                if os.path.isfile(path) or os.path.islink(path):
+                    to_delete_files[path] = True
+                elif os.path.isdir(path):
+                    to_delete_dirs[path] = True
+
+        # Delete files first then delete paths.
+        for path in to_delete_files:
+            os.remove(path)
+        for path in to_delete_dirs:
+            util.rmtree_nfs_safe(path, ignore_errors=False)
+
+        resources = self._list_directory(storage_dir)
+
+        if len(resources) == 0:
+            util.rmtree_nfs_safe(storage_dir, ignore_errors=False)
+        return resources
 
     def upload(
         self, src: Union[str, os.PathLike], dst: str, paths: Optional[storage.Paths] = None
     ) -> None:
         src = os.fspath(src)
 
         if paths is None:
```

## determined/core/_checkpoint.py

```diff
@@ -175,15 +175,15 @@
 
     def __init__(
         self,
         dist: core.DistributedContext,
         storage_manager: storage.StorageManager,
         session: api.Session,
         task_id: str,
-        allocation_id: str,
+        allocation_id: Optional[str],
         tbd_sync_mode: core.TensorboardMode,
         tensorboard_manager: tensorboard.TensorboardManager,
     ) -> None:
         self._dist = dist
         self._storage_manager = storage_manager
         self._session = session
         self._task_id = task_id
@@ -258,18 +258,17 @@
         selector: Optional[Callable[[str], bool]] = None,
     ) -> str:
         logger.debug(
             f"Uploading content from checkpoint directory {ckpt_dir} to storage "
             f"(metadata={metadata})"
         )
         storage_id = str(uuid.uuid4())
-        resources = self._storage_manager._list_directory(ckpt_dir)
-
-        # Add metadata pre-upload but without counting it among resources.
+        # Write metadata first so we get it in resources.
         self._write_metadata_file(ckpt_dir, metadata or {})
+        resources = self._storage_manager._list_directory(ckpt_dir)
 
         paths = None
         if selector is not None:
             resources = {key: resources[key] for key in resources if selector(key)}
             paths = set(resources)
 
         self._storage_manager.upload(src=ckpt_dir, dst=storage_id, paths=paths)
@@ -317,34 +316,29 @@
         )
         # Collect and filter resources for all uploading ranks.
         if want_upload:
             assert ckpt_dir
             resources = self._storage_manager._list_directory(ckpt_dir)
             if selector is not None:
                 resources = {key: resources[key] for key in resources if selector(key)}
-
-            # Metadata.json is a special file that is created and uploaded separately.
-            resources.pop("metadata.json", None)
         else:
             resources = {}
 
         all_resources = self._dist.allgather(resources)
         merged_resources, conflicts = merge_resources(all_resources)
         resources = self._resolve_conflicts(resources, conflicts, ckpt_dir)
 
         # Merge and upload metadata.
         all_metadata = self._merge_metadata(metadata)
         upload_mask = self._dist.allgather(want_upload)
         metadata_upload_rank = upload_mask.index(True)
         if self._dist.rank == metadata_upload_rank:
             assert ckpt_dir
             self._write_metadata_file(ckpt_dir, all_metadata)
-            # Include metadata in resources of the metadata uploading rank.
-            # Set value to 0 since it is not used anywhere.
-            resources["metadata.json"] = 0
+            resources["metadata.json"] = os.path.getsize(os.path.join(ckpt_dir, "metadata.json"))
 
         if want_upload:
             assert ckpt_dir
             paths = set(resources.keys())
             self._storage_manager.upload(src=ckpt_dir, dst=storage_id, paths=paths)
 
         # Synchronize workers.
@@ -509,16 +503,16 @@
                 "cannot call CheckpointContext.store_path(shard=False) from non-chief worker "
                 f"(rank={self._dist.rank})"
             )
 
         storage_id = str(uuid.uuid4())
         with self._storage_manager.store_path(storage_id) as path:
             yield path, storage_id
-            resources = self._storage_manager._list_directory(path)
             self._write_metadata_file(os.fspath(path), metadata or {})
+            resources = self._storage_manager._list_directory(path)
 
         self._report_checkpoint(storage_id, resources, metadata)
 
     def _store_path_sharded(
         self, metadata: Optional[Dict[str, Any]] = None
     ) -> Iterator[Tuple[pathlib.Path, str]]:
         logger.debug(f"Getting path for sharded storage (metadata={metadata})")
@@ -536,17 +530,16 @@
         if self._storage_manager.store_path_is_direct_access():
             # Each rank saves files directly to ckpt_dir which means there is no conflict
             # detection on upload. Metadata still needs to be merged and saved,
             # and checkpoint has to be reported.
             all_metadata = self._merge_metadata(metadata)
 
             if self._dist.rank == 0:
-                resources = self._storage_manager._list_directory(ckpt_dir)
-
                 self._write_metadata_file(os.fspath(path), all_metadata)
+                resources = self._storage_manager._list_directory(ckpt_dir)
                 self._report_checkpoint(storage_id, resources, all_metadata)
 
             return
 
         # Deconflict locally-shared directories; if every worker uploads /tmp/ckpt, then only
         # the lowest rank on each node will actually upload this directory.
         st = os.stat(ckpt_dir)
@@ -555,15 +548,14 @@
         # Decide if our rank is the lowest rank trying to upload this ckpt_dir.
         want_upload = all_file_uids.index(file_uid) == self._dist.rank
 
         # Decide what we are going to upload.
         if want_upload:
             assert ckpt_dir
             resources = self._storage_manager._list_directory(ckpt_dir)
-            resources.pop("metadata.json", None)
         else:
             resources = {}
 
         # Merge resources, detect conflicts.
         all_resources = self._dist.allgather(resources)
 
         merged_resources, conflicts = merge_resources(all_resources)
@@ -670,15 +662,15 @@
                 # Tell local chief we're done.
                 _ = self._dist.gather_local(None)
 
     def delete(self, storage_id: str) -> None:
         """
         Delete a checkpoint from the storage backend.
         """
-        self._storage_manager.delete(storage_id)
+        self._storage_manager.delete(storage_id, ["**/*"])
 
     def _write_metadata_file(self, ckpt_dir: str, metadata: Dict[str, Any]) -> None:
         metadata_path = pathlib.Path(ckpt_dir).joinpath("metadata.json")
         with metadata_path.open("w") as f:
             json.dump(metadata, f, indent=2)
 
     def _report_checkpoint(
```

## determined/core/_context.py

```diff
@@ -1,11 +1,12 @@
 import logging
 import pathlib
 import signal
 import sys
+import threading
 import traceback
 from typing import Any, Dict, Optional, Union
 
 import appdirs
 
 import determined as det
 from determined import core, tensorboard
@@ -68,14 +69,18 @@
 
 
 def _install_stacktrace_on_sigusr1() -> None:
     """Install a SIGUSR1 handler that prints a stack trace to stderr."""
     if not hasattr(signal, "SIGUSR1"):
         return
 
+    # Signal handlers can only be registered on main threads.
+    if threading.current_thread() is threading.main_thread():
+        return
+
     old_handler = None
 
     def stacktrace_on_sigusr1(signum: Any, frame: Any) -> None:
         traceback.print_stack(frame, file=sys.stderr)
         # old_handler may be None, SIG_IGN, or SIG_DFL.  It happens that SIG_DFL would be a noop for
         # SIGUSR1 so we don't have to worry about that case.
         if callable(old_handler):
```

## determined/deploy/aws/cli.py

```diff
@@ -60,14 +60,15 @@
         "https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html",
     )
 
 
 def get_deployment_class(deployment_type: str) -> Type[base.DeterminedDeployment]:
     deployment_type_map = {
         constants.deployment_types.SIMPLE: simple.Simple,
+        constants.deployment_types.SIMPLE_RDS: simple.SimpleRDS,
         constants.deployment_types.SECURE: secure.Secure,
         constants.deployment_types.EFS: vpc.EFS,
         constants.deployment_types.FSX: vpc.FSx,
         constants.deployment_types.GOVCLOUD: govcloud.Govcloud,
     }  # type: Dict[str, Type[base.DeterminedDeployment]]
     return deployment_type_map[deployment_type]
 
@@ -135,15 +136,18 @@
         return
 
     if (args.cpu_env_image and not args.gpu_env_image) or (
         args.gpu_env_image and not args.cpu_env_image
     ):
         raise CliError("If a CPU or GPU environment image is specified, both should be.")
 
-    if args.deployment_type != constants.deployment_types.SIMPLE:
+    if (
+        args.deployment_type != constants.deployment_types.SIMPLE
+        or args.deployment_type != constants.deployment_types.SIMPLE_RDS
+    ):
         if args.agent_subnet_id is not None:
             raise ValueError(
                 f"The agent-subnet-id can only be set if the deployment-type=simple. "
                 f"The agent-subnet-id was set to '{args.agent_subnet_id}', but the "
                 f"deployment-type={args.deployment_type}."
             )
```

## determined/deploy/aws/constants.py

```diff
@@ -1,14 +1,15 @@
 class deployment_types:
     SIMPLE = "simple"
+    SIMPLE_RDS = "simple-rds"
     SECURE = "secure"
     EFS = "efs"
     FSX = "fsx"
     GOVCLOUD = "govcloud"
-    DEPLOYMENT_TYPES = [SIMPLE, SECURE, EFS, FSX, GOVCLOUD]
+    DEPLOYMENT_TYPES = [SIMPLE, SECURE, EFS, FSX, GOVCLOUD, SIMPLE_RDS]
     TYPE_TAG_KEY = "deployment-type"
 
 
 class defaults:
     DEPLOYMENT_TYPE = deployment_types.SIMPLE
     DB_PASSWORD = "postgres"
     REGION = "us-west-2"
```

## determined/deploy/aws/deployment_types/simple.py

```diff
@@ -27,7 +27,12 @@
             parameters=cfn_parameters,
             extra_tags=self.parameters[constants.cloudformation.EXTRA_TAGS],
             no_prompt=no_prompt,
             deployment_type=self.deployment_type,
             update_terminate_agents=update_terminate_agents,
         )
         self.print_results()
+
+
+class SimpleRDS(Simple):
+    template = "simple-rds.yaml"
+    deployment_type = constants.deployment_types.SIMPLE_RDS
```

## determined/deploy/aws/templates/efs.yaml

```diff
@@ -97,15 +97,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.22.2-rc1
+    Default: 0.23.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
@@ -235,17 +235,19 @@
         save_trial_latest: 1
 
       db:
         user: postgres
         password: "{{ .db.password }}"
         host: "{{ .db.host }}"
         port: 5432
-        name: determined
+        name: "{{ .db.name }}"
+        {{- if .db.ssl_root_cert }}
         ssl_mode: verify-ca
-        ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
+        ssl_root_cert: "{{ .db.ssl_root_cert }}"
+        {{- end }}
 
       enable_cors: {{ .enable_cors }}
 
       resource_manager:
         type: agent
         default_aux_resource_pool: aux-pool
         default_compute_resource_pool: compute-pool
@@ -584,26 +586,25 @@
   Database:
     Type: AWS::RDS::DBCluster
     DeletionPolicy: Delete
     Properties:
       Engine: aurora-postgresql
       EngineMode: serverless
       DatabaseName: determined
-      DBClusterParameterGroupName: 'default.aurora-postgresql10'
       DBSubnetGroupName: !Ref DatabaseSubnetGroup
       MasterUsername: postgres
       MasterUserPassword: !Ref DBPassword
       Tags:
         - Key: user
           Value: !Ref AWS::StackName
       VpcSecurityGroupIds:
         - !GetAtt DatabaseSecurityGroup.GroupId
       ScalingConfiguration:
         AutoPause: false
-        MinCapacity: 8
+        MinCapacity: 2
         MaxCapacity: 32
 
   LogGroup:
     Type: AWS::Logs::LogGroup
     Properties:
       LogGroupName: !Sub /${LogGroupPrefix}/${AWS::StackName}
 
@@ -817,14 +818,16 @@
             cat << EOF > /usr/local/determined/etc/master.yaml.context
             checkpoint_storage:
               bucket: ${CheckpointBucket}
 
             db:
               password: "${DBPassword}"
               host: "${Database.Endpoint.Address}"
+              name: determined
+              ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
 
             enable_cors: ${EnableCORS}
 
             resource_manager:
               scheduler:
                 type: ${SchedulerType}
                 preemption: ${PreemptionEnabled}
```

## determined/deploy/aws/templates/fsx.yaml

```diff
@@ -97,15 +97,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.22.2-rc1
+    Default: 0.23.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
@@ -235,17 +235,19 @@
         save_trial_latest: 1
 
       db:
         user: postgres
         password: "{{ .db.password }}"
         host: "{{ .db.host }}"
         port: 5432
-        name: determined
+        name: "{{ .db.name }}"
+        {{- if .db.ssl_root_cert }}
         ssl_mode: verify-ca
-        ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
+        ssl_root_cert: "{{ .db.ssl_root_cert }}"
+        {{- end }}
 
       enable_cors: {{ .enable_cors }}
 
       resource_manager:
         type: agent
         default_aux_resource_pool: aux-pool
         default_compute_resource_pool: compute-pool
@@ -590,26 +592,25 @@
   Database:
     Type: AWS::RDS::DBCluster
     DeletionPolicy: Delete
     Properties:
       Engine: aurora-postgresql
       EngineMode: serverless
       DatabaseName: determined
-      DBClusterParameterGroupName: 'default.aurora-postgresql10'
       DBSubnetGroupName: !Ref DatabaseSubnetGroup
       MasterUsername: postgres
       MasterUserPassword: !Ref DBPassword
       Tags:
         - Key: user
           Value: !Ref AWS::StackName
       VpcSecurityGroupIds:
         - !GetAtt DatabaseSecurityGroup.GroupId
       ScalingConfiguration:
         AutoPause: false
-        MinCapacity: 8
+        MinCapacity: 2
         MaxCapacity: 32
 
   FSx:
     Type: AWS::FSx::FileSystem
     Condition: CreateFSx
     Properties:
       FileSystemType: LUSTRE
@@ -837,14 +838,16 @@
             cat << EOF > /usr/local/determined/etc/master.yaml.context
             checkpoint_storage:
               bucket: ${CheckpointBucket}
 
             db:
               password: "${DBPassword}"
               host: "${Database.Endpoint.Address}"
+              name: determined
+              ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
 
             enable_cors: ${EnableCORS}
 
             resource_manager:
               scheduler:
                 type: ${SchedulerType}
                 preemption: ${PreemptionEnabled}
```

## determined/deploy/aws/templates/govcloud.yaml

```diff
@@ -63,15 +63,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master docker image
-    Default: 0.22.2-rc1
+    Default: 0.23.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   MaxAuxContainersPerAgent:
@@ -180,17 +180,19 @@
         save_trial_latest: 1
 
       db:
         user: postgres
         password: "{{ .db.password }}"
         host: "{{ .db.host }}"
         port: 5432
-        name: determined
+        name: "{{ .db.name }}"
+        {{- if .db.ssl_root_cert }}
         ssl_mode: verify-ca
-        ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
+        ssl_root_cert: "{{ .db.ssl_root_cert }}"
+        {{- end }}
 
       enable_cors: {{ .enable_cors }}
 
       resource_manager:
         type: agent
         default_aux_resource_pool: aux-pool
         default_compute_resource_pool: compute-pool
@@ -625,14 +627,16 @@
             cat << EOF > /usr/local/determined/etc/master.yaml.context
             checkpoint_storage:
               bucket: ${CheckpointBucket}
 
             db:
               password: "${DBPassword}"
               host: "${Database.Endpoint.Address}"
+              name: determined
+              ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
 
             enable_cors: ${EnableCORS}
 
             resource_manager:
               scheduler:
                 type: ${SchedulerType}
                 preemption: ${PreemptionEnabled}
```

## determined/deploy/aws/templates/secure.yaml

```diff
@@ -118,15 +118,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master image
-    Default: 0.22.2-rc1
+    Default: 0.23.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database
     NoEcho: true
 
   MaxAuxContainersPerAgent:
@@ -230,17 +230,19 @@
         save_trial_latest: 1
 
       db:
         user: postgres
         password: "{{ .db.password }}"
         host: "{{ .db.host }}"
         port: 5432
-        name: determined
+        name: "{{ .db.name }}"
+        {{- if .db.ssl_root_cert }}
         ssl_mode: verify-ca
-        ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
+        ssl_root_cert: "{{ .db.ssl_root_cert }}"
+        {{- end }}
 
       enable_cors: {{ .enable_cors }}
 
       resource_manager:
         type: agent
         default_aux_resource_pool: aux-pool
         default_compute_resource_pool: compute-pool
@@ -601,28 +603,26 @@
   Database:
     Type: AWS::RDS::DBCluster
     DeletionPolicy: Delete
     Properties:
       Engine: aurora-postgresql
       EngineMode: serverless
       DatabaseName: determined
-      DBClusterParameterGroupName: 'default.aurora-postgresql10'
       DBSubnetGroupName: !Ref DatabaseSubnetGroup
       MasterUsername: postgres
       MasterUserPassword: !Ref DBPassword
       Tags:
         - Key: user
           Value: !Ref AWS::StackName
       VpcSecurityGroupIds:
         - !GetAtt DatabaseSecurityGroup.GroupId
       ScalingConfiguration:
-        AutoPause: true
-        SecondsUntilAutoPause: 3600
+        AutoPause: false
         MinCapacity: 2
-        MaxCapacity: 8
+        MaxCapacity: 32
 
   LogGroup:
     Type: AWS::Logs::LogGroup
     Properties:
       LogGroupName: !Sub /${LogGroupPrefix}/${AWS::StackName}
 
   LogPolicy:
@@ -831,14 +831,16 @@
             cat << EOF > /usr/local/determined/etc/master.yaml.context
             checkpoint_storage:
               bucket: ${CheckpointBucket}
 
             db:
               password: "${DBPassword}"
               host: "${Database.Endpoint.Address}"
+              name: determined
+              ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
 
             enable_cors: ${EnableCORS}
 
             resource_manager:
               scheduler:
                 type: ${SchedulerType}
                 preemption: ${PreemptionEnabled}
```

## determined/deploy/aws/templates/simple.yaml

```diff
@@ -89,15 +89,15 @@
     Type: String
     Description: Docker password to pull images that need authentication
     Default: ""
 
   Version:
     Type: String
     Description: Determined version or commit for master docker image
-    Default: 0.22.2-rc1
+    Default: 0.23.0-rc0
 
   DBPassword:
     Type: String
     Description: Password for database (eg. "postgres")
     NoEcho: true
 
   MaxAuxContainersPerAgent:
@@ -226,17 +226,19 @@
         save_trial_latest: 1
 
       db:
         user: postgres
         password: "{{ .db.password }}"
         host: "{{ .db.host }}"
         port: 5432
-        name: determined
+        name: "{{ .db.name }}"
+        {{- if .db.ssl_root_cert }}
         ssl_mode: verify-ca
-        ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
+        ssl_root_cert: "{{ .db.ssl_root_cert }}"
+        {{- end }}
 
       enable_cors: {{ .enable_cors }}
 
       resource_manager:
         type: agent
         default_aux_resource_pool: aux-pool
         default_compute_resource_pool: compute-pool
@@ -444,27 +446,25 @@
   Database:
     Type: AWS::RDS::DBCluster
     DeletionPolicy: Delete
     Properties:
       Engine: aurora-postgresql
       EngineMode: serverless
       DatabaseName: determined
-      DBClusterParameterGroupName: 'default.aurora-postgresql10'
       MasterUsername: postgres
       MasterUserPassword: !Ref DBPassword
       Tags:
         - Key: user
           Value: !Ref AWS::StackName
       VpcSecurityGroupIds:
         - !GetAtt DatabaseSecurityGroup.GroupId
       ScalingConfiguration:
-        AutoPause: true
-        SecondsUntilAutoPause: 3600
+        AutoPause: false
         MinCapacity: 2
-        MaxCapacity: 8
+        MaxCapacity: 32
 
   RetainedLogGroup:
     Type: AWS::Logs::LogGroup
     Condition: RetainLogGroup
     DeletionPolicy: Retain
     Properties:
       LogGroupName: !Sub /${LogGroupPrefix}/${AWS::StackName}
@@ -665,14 +665,16 @@
             cat << EOF > /usr/local/determined/etc/master.yaml.context
             checkpoint_storage:
               bucket: ${CheckpointBucket}
 
             db:
               password: "${DBPassword}"
               host: "${Database.Endpoint.Address}"
+              name: determined
+              ssl_root_cert: /etc/determined/db_ssl_root_cert.pem
 
             enable_cors: ${EnableCORS}
 
             resource_manager:
               scheduler:
                 type: ${SchedulerType}
                 preemption: ${PreemptionEnabled}
```

## determined/exec/gc_checkpoints.py

```diff
@@ -2,39 +2,79 @@
 The entrypoint for the GC checkpoints job container.
 """
 import argparse
 import json
 import logging
 import os
 import sys
-from typing import Any, List
+from typing import Any, Dict, List
+
+import urllib3
 
 import determined as det
 from determined import errors, tensorboard
-from determined.common import constants, storage
+from determined.common import api, constants, storage, util
+from determined.common.api import bindings, certs
+
+
+def patch_checkpoints(storage_ids_to_resources: Dict[str, Dict[str, int]]) -> None:
+    info = det.ClusterInfo._from_file()
+    if info is None:
+        info = det.ClusterInfo._from_env()
+        info._to_file()
+
+    cert = certs.default_load(info.master_url)
+    sess = api.Session(
+        info.master_url,
+        util.get_det_username_from_env(),
+        None,
+        cert,
+        max_retries=urllib3.util.retry.Retry(
+            total=6,  # With backoff retries for 64 seconds
+            backoff_factor=0.5,
+        ),
+    )
+
+    checkpoints = []
+    for storage_id, resources in storage_ids_to_resources.items():
+        checkpoints.append(
+            bindings.v1PatchCheckpoint(
+                uuid=storage_id,
+                resources=bindings.PatchCheckpointOptionalResources(
+                    resources=resources,  # type: ignore
+                ),
+            )
+        )
+
+    bindings.patch_PatchCheckpoints(
+        sess, body=bindings.v1PatchCheckpointsRequest(checkpoints=checkpoints)
+    )
 
 
 def delete_checkpoints(
-    manager: storage.StorageManager, to_delete: List[str], dry_run: bool
-) -> None:
+    manager: storage.StorageManager, to_delete: List[str], globs: List[str], dry_run: bool
+) -> Dict[str, Dict[str, int]]:
     """
     Delete some of the checkpoints associated with a single experiment.
     """
     logging.info("Deleting {} checkpoints".format(len(to_delete)))
 
+    storage_id_to_resources: Dict[str, Dict[str, int]] = {}
     for storage_id in to_delete:
         if not dry_run:
             logging.info(f"Deleting checkpoint {storage_id}")
             try:
-                manager.delete(storage_id)
+                storage_id_to_resources[storage_id] = manager.delete(storage_id, globs)
             except errors.CheckpointNotFound as e:
                 logging.warn(e)
         else:
             logging.info(f"Dry run: deleting checkpoint {storage_id}")
 
+    return storage_id_to_resources
+
 
 def delete_tensorboards(manager: tensorboard.TensorboardManager, dry_run: bool = False) -> None:
     """
     Delete all Tensorboards associated with a single experiment.
     """
     if dry_run:
         logging.info(f"Dry run: deleting Tensorboards for {manager.sync_path}")
@@ -71,17 +111,23 @@
         "--storage-config",
         type=json_file_arg,
         default=os.getenv("DET_STORAGE_CONFIG", {}),
         help="Storage config (JSON-formatted file)",
     )
     parser.add_argument(
         "--delete",
-        type=str,
-        default=os.getenv("DET_DELETE", ""),
-        help="comma-separated list of checkpoints to delete",
+        type=json_file_arg,
+        default=os.getenv("DET_DELETE", []),
+        help="Checkpoints to delete (JSON-formatted file)",
+    )
+    parser.add_argument(
+        "--globs",
+        type=json_file_arg,
+        default=os.getenv("DET_GLOB", []),
+        help="Glob list to match against checkpoint list (JSON-formatted file)",
     )
     parser.add_argument(
         "--delete-tensorboards",
         action="store_true",
         default=os.getenv("DET_DELETE_TENSORBOARDS", False),
         help="Delete Tensorboards from storage",
     )
@@ -99,21 +145,24 @@
     )
 
     logging.info("Determined checkpoint GC, version {}".format(det.__version__))
 
     storage_config = args.storage_config
     logging.info("Using checkpoint storage: {}".format(storage_config))
 
+    storage_ids = [s.strip() for s in args.delete]
+    globs = [s.strip() for s in args.globs]
+
     manager = storage.build(storage_config, container_path=constants.SHARED_FS_CONTAINER_PATH)
 
-    args.delete = args.delete.strip()
-    storage_ids = []
-    if args.delete != "":
-        storage_ids = args.delete.split(",")
-    delete_checkpoints(manager, storage_ids, dry_run=args.dry_run)
+    if len(storage_ids) > 0:
+        storage_ids_to_resources = delete_checkpoints(
+            manager, storage_ids, globs, dry_run=args.dry_run
+        )
+        patch_checkpoints(storage_ids_to_resources)
 
     if args.delete_tensorboards:
         tb_manager = tensorboard.build(
             os.environ["DET_CLUSTER_ID"],
             args.experiment_id,
             None,
             storage_config,
```

## determined/experimental/__init__.py

```diff
@@ -6,7 +6,9 @@
     ModelOrderBy,
     ModelSortBy,
     TrialReference,
     TrialOrderBy,
     TrialSortBy,
 )
 from determined.experimental._native import test_one_batch
+
+from determined.experimental import client
```

## determined/experimental/client.py

```diff
@@ -391,25 +391,27 @@
     """
     Get a list of Oauth2 Scim clients.
     """
     assert _determined is not None
     return _determined.list_oauth_clients()
 
 
+@_require_singleton
 def add_oauth_client(domain: str, name: str) -> Oauth2ScimClient:
     """
     Add an oauth client.
     Arguments:
         domain: Domain of OAuth client.
         name: Name of OAuth client.
     """
     assert _determined is not None
     return _determined.add_oauth_client(domain, name)
 
 
+@_require_singleton
 def remove_oauth_client(client_id: str) -> None:
     """
     Arguments:
        client_id: Client id of OAuth client.
     """
     assert _determined is not None
     return _determined.remove_oauth_client(client_id)
@@ -435,7 +437,13 @@
     trial_id, trial_run_id and steps_completed.
 
     Arguments:
         trial_ids: List of trial IDs to get metrics for.
     """
     assert _determined is not None
     return _determined.stream_trials_validation_metrics(trial_ids)
+
+
+@_require_singleton
+def _get_singleton_session() -> Session:
+    assert _determined is not None
+    return _determined._session
```

## determined/pytorch/deepspeed/_deepspeed_context.py

```diff
@@ -7,26 +7,15 @@
 import deepspeed
 import torch
 from deepspeed.runtime import config_utils
 
 import determined as det
 from determined import profiler, pytorch
 from determined.pytorch import deepspeed as det_ds
-
-
-def merge_dicts(base_dict: Dict[str, Any], source_dict: Dict[str, Any]) -> Dict[str, Any]:
-    for key, value in source_dict.items():
-        if key in base_dict:
-            if isinstance(value, dict):
-                base_dict[key] = merge_dicts(base_dict[key], value)
-            else:
-                base_dict[key] = value
-        else:
-            base_dict[key] = value
-    return base_dict
+from determined.util import merge_dicts
 
 
 def overwrite_deepspeed_config(
     base_ds_config: Union[str, Dict], source_ds_dict: Dict[str, Any]
 ) -> Dict[str, Any]:
     """Overwrite a base_ds_config with values from a source_ds_dict.
```

## determined/pytorch/deepspeed/_deepspeed_trial.py

```diff
@@ -13,14 +13,15 @@
 import numpy as np
 import torch
 from deepspeed.runtime import dataloader as ds_loader
 
 import determined as det
 from determined import layers, pytorch, util, workload
 from determined.pytorch import deepspeed as det_ds
+from determined.pytorch import dsat
 
 
 # In most cases in which a user disables data reproducibility checks and chooses to return
 # their own data loader, it will most likely be one created as part of DeepSpeed model engine
 # initialization.  For the PipelineEngine, a RepeatingLoader is returned that does not have a
 # __len__ method.  We patch in a length method here to make sure we can compute epoch length
 # and validation length.
@@ -36,14 +37,20 @@
         super().__init__(*args, **kwargs)
 
         assert isinstance(
             trial_inst, DeepSpeedTrial
         ), "DeepSpeedTrialController needs a DeepSpeedTrial"
         self.trial = trial_inst
         self.context = cast(det_ds.DeepSpeedTrialContext, self.context)
+        self._dsat_mode = self.context.get_hparams().get(dsat._defaults.USE_DSAT_MODE_KEY, False)
+        if self._dsat_mode:
+            searcher_name = self.context.get_experiment_config()["searcher"]["name"]
+            assert (
+                searcher_name == "custom"
+            ), "`_dsat_mode` can only be set to true for Custom Searcher trials."
         self.context._set_determined_profiler(self.prof)
         if torch.cuda.is_available():
             self.prof._set_sync_device(self._sync_device)
         self.callbacks = self.trial.build_callbacks()
         for callback in self.callbacks.values():
             if util.is_overridden(callback.on_checkpoint_end, pytorch.PyTorchCallback):
                 warnings.warn(
@@ -287,14 +294,26 @@
                     with self.prof.record_timing(
                         f"callbacks.{callback.__class__.__name__}.on_training_start"
                     ):
                         callback.on_training_start()
                 self._run()
 
     def _run(self) -> None:
+        # Special code path only used for DeepSpeed Autotuning.
+        if self._dsat_mode:
+            ops = self.context._core.searcher.operations()
+            op = next(ops)
+            for _ in range(op.length):
+                with dsat.dsat_reporting_context(core_context=self.context._core, op=op):
+                    _ = self._train_for_step(
+                        step_id=self.steps_completed + 1,
+                        num_batches=1,
+                        total_batches_processed=self.steps_completed,
+                    )
+
         assert self.workloads is not None
         for w, response_func in self.workloads:
             try:
                 if w.kind == workload.Workload.Kind.RUN_STEP:
                     action = "training"
                     metrics = self._train_for_step(
                         w.step_id,
```

## determined/searcher/_remote_search_runner.py

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import pickle
-from typing import Any, Dict, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import determined as det
 from determined import searcher
 from determined.experimental import client
 
 logger = logging.getLogger("determined.searcher")
 
@@ -28,39 +29,45 @@
 
         self.latest_checkpoint = self.info.latest_checkpoint
 
     def run(
         self,
         exp_config: Union[Dict[str, Any], str],
         model_dir: Optional[str] = None,
+        includes: Optional[Iterable[Union[str, Path]]] = None,
     ) -> int:
         """
         Run custom search as a Core API experiment (on-cluster).
 
         Args:
             exp_config (dictionary, string): experiment config filename (.yaml) or a dict.
             model_dir (string): directory containing model definition.
+            includes (Iterable[Union[str, pathlib.Path]], optional): Additional files
+                or directories to include in the model definition.  (default: ``None``)
         """
         logger.info("RemoteSearchRunner.run")
 
         operations: Optional[List[searcher.Operation]] = None
 
         if model_dir is None:
             model_dir = os.getcwd()
 
         if self.latest_checkpoint is not None:
             experiment_id, operations = self.load_state(self.latest_checkpoint)
             logger.info(f"Resuming HP searcher for experiment {experiment_id}")
         else:
             logger.info("No latest checkpoint. Starting new experiment.")
-            exp = client.create_experiment(exp_config, model_dir)
+            exp = client.create_experiment(exp_config, model_dir, includes)
             self.state.experiment_id = exp.id
             self.state.last_event_id = 0
             self.save_state(exp.id, [])
             experiment_id = exp.id
+            # Note: Simulating the same print functionality as our CLI when making an experiment.
+            # This line is needed for the e2e tests
+            logger.info(f"Created experiment {exp.id}")
 
         # make sure client is initialized
         client._require_singleton(lambda: None)()
         assert client._determined is not None
         session = client._determined._session
         self.run_experiment(experiment_id, session, operations)
```

## determined/searcher/_search_method.py

```diff
@@ -1,7 +1,8 @@
+import abc
 import dataclasses
 import json
 import pathlib
 import uuid
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Dict, List, Optional, Set, Tuple
@@ -11,15 +12,15 @@
 
 STATE_FILE = "state"
 
 
 @dataclasses.dataclass
 class SearcherState:
     """
-    Mutable Searcher state.
+    Custom Searcher State.
 
     Search runners maintain this state that can be used by a ``SearchMethod``
     to inform event handling. In other words, this state can be taken into account
     when deciding which operations to return from your event handler. Do not
     modify ``SearcherState`` in your ``SearchMethod``. If your hyperparameter
     tuning algorithm needs additional state variables, add those variable to your
     ``SearchMethod`` implementation.
@@ -33,14 +34,15 @@
 
     failures: Set[uuid.UUID]
     trial_progress: Dict[uuid.UUID, float]
     trials_closed: Set[uuid.UUID]
     trials_created: Set[uuid.UUID]
     last_event_id: int = 0
     experiment_completed: bool = False
+    experiment_failed: bool = False
 
     def __init__(self) -> None:
         self.failures = set()
         self.trial_progress = {}
         self.trials_closed = set()
         self.trials_created = set()
 
@@ -49,27 +51,39 @@
             "failures": [str(f) for f in self.failures],
             "trialProgress": {str(k): v for k, v in self.trial_progress.items()},
             "trialsClosed": [str(t) for t in self.trials_closed],
             "trialsCreated": [str(t) for t in self.trials_created],
             "lastEventId": self.last_event_id,
             "experimentId": self.experiment_id,
             "experimentCompleted": self.experiment_completed,
+            "experimentFailed": self.experiment_failed,
         }
 
     def from_dict(self, d: Dict[str, Any]) -> None:
         self.failures = {uuid.UUID(f) for f in d.get("failures", [])}
         self.trial_progress = {uuid.UUID(k): v for k, v in d.get("trialProgress", {}).items()}
         self.trials_closed = {uuid.UUID(t) for t in d.get("trialsClosed", [])}
         self.trials_created = {uuid.UUID(t) for t in d.get("trialsCreated", [])}
         self.last_event_id = d.get("lastEventId", 0)
         self.experiment_id = d.get("experimentId")
         self.experiment_completed = d.get("experimentCompleted", False)
+        self.experiment_failed = d.get("experimentFailed", False)
 
 
 class ExitedReason(Enum):
+    """
+    The reason why a trial exited early
+
+    The following reasons are supported:
+
+    - `ERRORED`: The Trial encountered an exception
+    - `USER_CANCELLED`: The Trial was manually closed by the user
+    - `INVALID_HP`: The hyperparameters the trial was created with were invalid
+    """
+
     ERRORED = "ERRORED"
     USER_CANCELED = "USER_CANCELED"
     INVALID_HP = "INVALID_HP"
 
     @classmethod
     def _from_bindings(
         cls, bindings_exited_reason: bindings.v1TrialExitedEarlyExitedReason
@@ -79,20 +93,20 @@
         if bindings_exited_reason == bindings.v1TrialExitedEarlyExitedReason.USER_REQUESTED_STOP:
             return cls.USER_CANCELED
         if bindings_exited_reason == bindings.v1TrialExitedEarlyExitedReason.UNSPECIFIED:
             return cls.ERRORED
         raise RuntimeError(f"Invalid exited reason: {bindings_exited_reason}")
 
 
-class Operation:
+class Operation(metaclass=abc.ABCMeta):
     """
     Abstract base class for all Operations
     """
 
-    @abstractmethod
+    @abc.abstractmethod
     def _to_searcher_operation(self) -> bindings.v1SearcherOperation:
         pass
 
 
 class ValidateAfter(Operation):
     """
     Operation signaling the trial to train until its total units trained
@@ -113,41 +127,45 @@
                 ),
             )
         )
 
 
 class Close(Operation):
     """
-    Operation closing the specified trial
+    Operation for closing the specified trial
     """
 
     def __init__(self, request_id: uuid.UUID):
         super().__init__()
         self.request_id = request_id
 
     def _to_searcher_operation(self) -> bindings.v1SearcherOperation:
         return bindings.v1SearcherOperation(
             closeTrial=bindings.v1CloseTrialOperation(requestId=str(self.request_id))
         )
 
 
 class Progress(Operation):
+    """
+    Operation for signalling the relative progress of the hyperparameter search between 0 and 1
+    """
+
     def __init__(self, progress: float):
         super().__init__()
         self.progress = progress
 
     def _to_searcher_operation(self) -> bindings.v1SearcherOperation:
         return bindings.v1SearcherOperation(
             setSearcherProgress=bindings.v1SetSearcherProgressOperation(progress=self.progress)
         )
 
 
 class Shutdown(Operation):
     """
-    Operation shutting the experiment down
+    Operation for shutting the experiment down
     """
 
     def __init__(self, cancel: bool = False, failure: bool = False) -> None:
         super().__init__()
         self.cancel = cancel
         self.failure = failure
 
@@ -155,15 +173,15 @@
         return bindings.v1SearcherOperation(
             shutDown=bindings.v1ShutDownOperation(cancel=self.cancel, failure=self.failure)
         )
 
 
 class Create(Operation):
     """
-    Operation creating a trial with a specified combination of hyperparameter values
+    Operation for creating a trial with a specified combination of hyperparameter values
     """
 
     def __init__(
         self,
         request_id: uuid.UUID,
         hparams: Dict[str, Any],
         checkpoint: Optional[experimental.Checkpoint],
@@ -182,85 +200,246 @@
 
 
 class SearchMethod:
     """
     The implementation of a custom hyperparameter tuning algorithm.
 
     To implement your specific hyperparameter tuning approach, subclass ``SearchMethod``
-    overriding the event handler methods. Each event handler, except ``progress`` returns a list of
-    operations (``List[Operation]``) that will be submitted to master for processing.
+    overriding the event handler methods.
+
+    Each event handler, except :meth:`progress() <determined.searcher.SearchMethod.progress>`
+    returns a list of operations (``List[Operation]``) that will be submitted to master for
+    processing.
+
+    Currently, we support the following :class:`~Operation`:
+
+    - :class:`~Create` - starts a new trial with a unique trial id and a set of hyperparameter
+      values.
+    - :class:`~ValidateAfter` - sets number of steps (i.e., batches or epochs) after which a
+      validation is run for a trial with a given id.
+    - :class:`~Progress` - updates the progress of the multi-trial experiment to the master.
+    - :class:`~Close` - closes a trial with a given id.
+    - :class:`~Shutdown` - closes the experiment.
 
     .. note::
 
         Do not modify ``searcher_state`` passed into event handlers.
     """
 
     @abstractmethod
     def initial_operations(self, searcher_state: SearcherState) -> List[Operation]:
         """
-        Returns a set of initial operations that the searcher will perform.
-
-        Currently, we support the following operations:
-
-        - Create - starts a new trial with a unique trial id and a set of hyperparameter
-          values,
-        - ValidateAfter - sets number of steps (i.e., batches or epochs) after which a validation
-          is run for a trial with a given id,
-        - Close - closes a trial with a given id,
-        - Shutdown - closes the experiment.
+        Returns a list of initial operations that the custom hyperparameter search should
+        perform. This is called by the Custom Searcher :class:`~SearchRunner`
+        to initialize the trials
+
+        Example:
+
+        .. code:: python
+
+            def initial_operations(self, _: searcher.SearcherState) -> List[searcher.Operation]:
+                ops: List[searcher.Operation] = []
+                N = 100
+                hparams = {
+                    # ...
+                }
+                for _ in range(0, N):
+                    create = searcher.Create(
+                        request_id=uuid.uuid4(),
+                        hparams=hparams,
+                        checkpoint=None,
+                    )
+                    ops.append(create)
+                return ops
+
+        Args:
+            searcher_state(:class:`~SearcherState`): Read-only current searcher state
+
+        Returns:
+            List[Operation]: Initial list of :class:`~Operation` to start the Hyperparameter
+            search
         """
         pass
 
     @abstractmethod
     def on_trial_created(
         self, searcher_state: SearcherState, request_id: uuid.UUID
     ) -> List[Operation]:
         """
         Informs the searcher that a trial has been created
         as a result of Create operation.
+
+        Example:
+
+        .. code:: python
+
+            def on_trial_created(
+                self, _: SearcherState, request_id: uuid.UUID
+            ) -> List[Operation]:
+                return [
+                    searcher.ValidateAfter(
+                        request_id=request_id,
+                        length=1,  # Run for one unit of time (epoch, etc.)
+                    )
+                ]
+
+        In this example, we are choosing to deterministically train for one unit of time
+
+        Args:
+            searcher_state(:class:`~SearcherState`): Read-only current searcher state
+            request_id (uuid.UUID): Request UUID of the Trial that was created
+
+        Returns:
+            List[Operation]: List of :class:`~Operation` to run upon creation of the given
+            trial
         """
         pass
 
     @abstractmethod
     def on_validation_completed(
         self, searcher_state: SearcherState, request_id: uuid.UUID, metric: Any, train_length: int
     ) -> List[Operation]:
         """
-        Informs the searcher that the validation workload
-        initiated by the same searcher has completed after training for ``train_length`` units.
-        It returns any new operations as a result of this workload completing.
+        Informs the searcher that the validation workload has completed after training for
+        ``train_length`` units. It returns any new operations as a result of this workload
+        completing
+
+        Example:
+
+        .. code:: python
+
+            def on_validation_completed(
+                self,
+                searcher_state: SearcherState,
+                request_id: uuid.UUID,
+                metric: Any,
+                train_length: int
+            ) -> List[Operation]:
+                if train_length < self.max_train_length:
+                    return [
+                        searcher.ValidateAfter(
+                            request_id=request_id,
+                            length=train_length + 1,  # Run an additional unit of time
+                        )
+                    ]
+                return [searcher.Close(request_id=request_id)]
+
+        Args:
+            searcher_state (SearcherState): Read-only current searcher state
+            request_id (uuid.UUID): Request UUID of the Trial that was trained
+            metric (Any): Metric data returned by the trial
+            train_length (int): The cumulative units of time that that trial has finished
+                training for (epochs, etc.)
+
+        Returns:
+            List[Operation]: List of :class:`~Operation` to run upon completion of training for
+            the given trial
         """
         pass
 
     @abstractmethod
     def on_trial_closed(
         self, searcher_state: SearcherState, request_id: uuid.UUID
     ) -> List[Operation]:
         """
-        Informs the searcher that a trial has been closed as a result of a Close
-        operation.
+        Informs the searcher that a trial has been closed as a result of a :class:`~Close`
+
+        Example:
+
+        .. code:: python
+
+            def on_trial_closed(
+                self, searcher_state: SearcherState, request_id: uuid.UUID
+            ) -> List[Operation]:
+                if searcher_state.trials_created < self.max_num_trials:
+                    hparams = {
+                        # ...
+                    }
+                    return [
+                        searcher.Create(
+                            request_id=uuid.uuid4(),
+                            hparams=hparams,
+                            checkpoint=None,
+                        )
+                    ]
+                if searcher_state.trials_closed >= self.max_num_trials:
+                    return [searcher.Shutdown()]
+                return []
+
+        Args:
+            searcher_state (SearcherState): Read-only current searcher state
+            request_id (uuid.UUID): Request UUID of the Trial that was closed
+
+        Returns:
+            List[Operation]: List of :class:`~Operation` to run after closing the given
+            trial
         """
         pass
 
     @abstractmethod
     def progress(self, searcher_state: SearcherState) -> float:
         """
         Returns experiment progress as a float between 0 and 1.
+
+        Example:
+
+        .. code:: python
+
+            def progress(self, searcher_state: SearcherState) -> float:
+                return searcher_state.trials_closed / float(self.max_num_trials)
+
+        Args:
+            searcher_state (SearcherState): Read-only current searcher state
+
+        Returns:
+            float: Experiment progress as a float between 0 and 1.
         """
         pass
 
     @abstractmethod
     def on_trial_exited_early(
         self,
         searcher_state: SearcherState,
         request_id: uuid.UUID,
         exited_reason: ExitedReason,
     ) -> List[Operation]:
         """
         Informs the searcher that a trial has exited earlier than expected.
+
+        Example:
+
+        .. code:: python
+
+            def on_trial_exited_early(
+                self,
+                searcher_state: SearcherState,
+                request_id: uuid.UUID,
+                exited_reason: ExitedReason,
+            ) -> List[Operation]:
+                if exited_reason == searcher.ExitedReason.USER_CANCELED:
+                    return [searcher.Shutdown(cancel=True)]
+                if exited_reason == searcher.ExitedReason.INVALID_HP:
+                    return [searcher.Shutdown(failure=True)]
+                if searcher_state.failures >= self.max_failures:
+                    return [searcher.Shutdown(failure=True)]
+                return []
+
+        .. note::
+
+            The trial has already been internally closed when this callback is run.
+            You do not need to explicitly issue a :class:`~Close` operation
+
+        Args:
+            searcher_state (SearcherState): Read-only current searcher state
+            request_id (uuid.UUID): Request UUID of the Trial that exited early
+            exited_reason (ExitedReason): The reason that the trial exited early
+
+        Returns:
+            List[Operation]: List of :class:`~Operation` to run in response to the given
+            trial exiting early
         """
         pass
 
     def save(
         self, searcher_state: SearcherState, path: pathlib.Path, *, experiment_id: int
     ) -> None:
         """
```

## determined/searcher/_search_runner.py

```diff
@@ -1,18 +1,18 @@
 import json
 import logging
 import os
 import pickle
 import time
 import uuid
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 from determined import searcher
-from determined.common.api import bindings
+from determined.common.api import bindings, errors
 from determined.experimental import client
 
 EXPERIMENT_ID_FILE = "experiment_id.txt"
 logger = logging.getLogger("determined.searcher")
 
 
 class _ExperimentInactiveException(Exception):
@@ -45,17 +45,19 @@
             operations = self.search_method.on_trial_closed(self.state, request_id)
 
             # add progress operation
             progress = self.search_method.progress(self.state)
             operations.append(searcher.Progress(progress))
         elif event.trialExitedEarly:
             # duplicate exit accounting already performed by master
+            searcher_exit_reason = searcher.ExitedReason._from_bindings(
+                event.trialExitedEarly.exitedReason
+            )
             logger.info(
-                f"trialExitedEarly({event.trialExitedEarly.requestId},"
-                f" {event.trialExitedEarly.exitedReason})"
+                f"trialExitedEarly({event.trialExitedEarly.requestId}, {searcher_exit_reason})"
             )
             if event.trialExitedEarly.exitedReason is None:
                 raise RuntimeError("trialExitedEarly event is invalid without exitedReason")
             request_id = uuid.UUID(event.trialExitedEarly.requestId)
             if (
                 event.trialExitedEarly.exitedReason
                 == bindings.v1TrialExitedEarlyExitedReason.INVALID_HP
@@ -65,17 +67,15 @@
                 event.trialExitedEarly.exitedReason
                 == bindings.v1TrialExitedEarlyExitedReason.UNSPECIFIED
             ):
                 self.state.failures.add(request_id)
             operations = self.search_method.on_trial_exited_early(
                 self.state,
                 request_id,
-                exited_reason=searcher.ExitedReason._from_bindings(
-                    event.trialExitedEarly.exitedReason
-                ),
+                exited_reason=searcher_exit_reason,
             )
             # add progress operation
             progress = self.search_method.progress(self.state)
             operations.append(searcher.Progress(progress))
         elif event.validationCompleted:
             # duplicate completion accounting already performed by master
             logger.info(
@@ -116,21 +116,21 @@
         return operations
 
     def run_experiment(
         self,
         experiment_id: int,
         session: client.Session,
         prior_operations: Optional[List[searcher.Operation]],
+        sleep_time: float = 1.0,
     ) -> None:
         experiment_is_active = True
-
         try:
             while experiment_is_active:
                 time.sleep(
-                    1
+                    sleep_time
                 )  # we don't want to call long polling API more often than every second.
                 events = self.get_events(session, experiment_id)
                 if not events:
                     continue
                 logger.info(json.dumps([SearchRunner._searcher_event_as_dict(e) for e in events]))
                 # the first event is an event we have already processed and told master about it
                 # however, we may not have saved the state after that event if we crashed
@@ -153,14 +153,19 @@
                                 f"inactive; state={event.experimentInactive.experimentState}"
                             )
                             if (
                                 event.experimentInactive.experimentState
                                 == bindings.experimentv1State.COMPLETED
                             ):
                                 self.state.experiment_completed = True
+                            elif (
+                                event.experimentInactive.experimentState
+                                == bindings.experimentv1State.ERROR
+                            ):
+                                self.state.experiment_failed = True
 
                             if (
                                 event.experimentInactive.experimentState
                                 == bindings.experimentv1State.PAUSED
                             ):
                                 self._show_experiment_paused_msg()
                             else:
@@ -187,19 +192,36 @@
         operations: List[searcher.Operation],
     ) -> None:
         body = bindings.v1PostSearcherOperationsRequest(
             experimentId=self.state.experiment_id,
             searcherOperations=[op._to_searcher_operation() for op in operations],
             triggeredByEvent=event,
         )
-        bindings.post_PostSearcherOperations(
-            session,
-            body=body,
-            experimentId=experiment_id,
-        )
+
+        # This try/except is intended to catch a specific error which occurs for DeepSpeed Autotune.
+        # DeepSpeed makes an explicit `exit()` call internally when autotuning flags are enabled in
+        # the DS config. When we also post a `Close` operation, there is a resulting race condition
+        # and intermittently the process and its corresponding agent die before the `Close`
+        # operation reaches the agent, resulting in a `APIException` with a `failed to post
+        # operations: rpc error: code = NotFound desc = actor /experiments/xxx could not be found`
+        # message. This try/except allows the experiment to continue uninterrupted in such cases.
+        try:
+            bindings.post_PostSearcherOperations(
+                session,
+                body=body,
+                experimentId=experiment_id,
+            )
+        except errors.APIException as e:
+            logging.warning(f"Catching errors.APIException: {str(e)}")
+            close_op_in_operations = any((isinstance(o, searcher.Close) for o in operations))
+            logging.warning(f"operations: {operations}")
+            if close_op_in_operations and "could not be found" in str(e):
+                pass
+            else:
+                raise e
 
     def get_events(
         self,
         session: client.Session,
         experiment_id: int,
     ) -> Optional[Sequence[bindings.v1SearcherEvent]]:
         # API is implemented with long polling.
@@ -243,45 +265,49 @@
                 f"searcher_dir={self.searcher_dir} already exists and is not a directory"
             )
 
     def run(
         self,
         exp_config: Union[Dict[str, Any], str],
         model_dir: Optional[str] = None,
+        includes: Optional[Iterable[Union[str, Path]]] = None,
     ) -> int:
         """
         Run custom search.
 
         Args:
             exp_config (dictionary, string): experiment config filename (.yaml) or a dict.
             model_dir (string): directory containing model definition.
+            includes (Iterable[Union[str, pathlib.Path]], optional): Additional files
+                or directories to include in the model definition.  (default: ``None``)
         """
         logger.info("LocalSearchRunner.run")
 
         if model_dir is None:
             model_dir = os.getcwd()
         experiment_id_file = self.searcher_dir.joinpath(EXPERIMENT_ID_FILE)
         operations: Optional[List[searcher.Operation]] = None
         if experiment_id_file.exists():
             with experiment_id_file.open("r") as f:
                 experiment_id = int(f.read())
             logger.info(f"Resuming HP searcher for experiment {experiment_id}")
             # load searcher state and search method state
             _, operations = self.load_state(experiment_id)
         else:
-            exp = client.create_experiment(exp_config, model_dir)
+            exp = client.create_experiment(exp_config, model_dir, includes)
             with experiment_id_file.open("w") as f:
                 f.write(str(exp.id))
             state_path = self._get_state_path(exp.id)
             state_path.mkdir(parents=True)
-            logger.info(f"Starting HP searcher for experiment {exp.id}")
             self.state.experiment_id = exp.id
             self.state.last_event_id = 0
             self.save_state(exp.id, [])
             experiment_id = exp.id
+            # Note: Simulating the same print functionality as our CLI when making an experiment.
+            logger.info(f"Created experiment {experiment_id}")
 
         # make sure client is initialized
         client._require_singleton(lambda: None)()
         assert client._determined is not None
         session = client._determined._session
         self.run_experiment(experiment_id, session, operations)
         return experiment_id
```

## determined/tensorboard/build.py

```diff
@@ -1,13 +1,13 @@
 import os
 import pathlib
 from typing import Any, Dict, Optional
 
 from determined.common.storage.shared import _full_storage_path
-from determined.tensorboard import azure, base, gcs, hdfs, s3, shared
+from determined.tensorboard import azure, base, gcs, s3, shared
 
 
 def get_sync_path(cluster_id: str, experiment_id: str, trial_id: str) -> pathlib.Path:
     return pathlib.Path(
         get_experiment_sync_path(cluster_id, experiment_id),
         "trial",
         trial_id,
@@ -113,22 +113,9 @@
             checkpoint_config.get("access_url", None),
             checkpoint_config.get("credential", None),
             base_path,
             sync_path,
             async_upload=async_upload,
         )
 
-    # Return the base_path.TensorboardManager for known but unsupported storage
-    # backends. This will result in a noop action when the workload_manager
-    # attempts to sync the tfevent files to persistent storage.
-    elif type_name == "hdfs":
-        return hdfs.HDFSTensorboardManager(
-            checkpoint_config["hdfs_url"],
-            checkpoint_config["hdfs_path"],
-            checkpoint_config.get("user"),
-            base_path,
-            sync_path,
-            async_upload=async_upload,
-        )
-
     else:
         raise TypeError(f"Unknown storage type: {type_name}")
```

## Comparing `determined-0.22.2rc1.dist-info/METADATA` & `determined-0.23.0rc0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: determined
-Version: 0.22.2rc1
+Version: 0.23.0rc0
 Summary: Determined Deep Learning Training Platform
 Home-page: https://determined.ai/
 Author: Determined AI
 Author-email: hello@determined.ai
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
@@ -13,15 +13,14 @@
 Requires-Dist: numpy (>=1.16.2)
 Requires-Dist: psutil
 Requires-Dist: pyzmq (>=18.1.0)
 Requires-Dist: yogadl (==0.1.4)
 Requires-Dist: certifi
 Requires-Dist: filelock
 Requires-Dist: google-cloud-storage
-Requires-Dist: hdfs (>=2.2.2)
 Requires-Dist: lomond (>=0.3.3)
 Requires-Dist: pathspec (>=0.6.0)
 Requires-Dist: azure-core
 Requires-Dist: azure-storage-blob
 Requires-Dist: termcolor (>=1.1.0)
 Requires-Dist: boto3
 Requires-Dist: argcomplete (>=1.9.4)
```

## Comparing `determined-0.22.2rc1.dist-info/RECORD` & `determined-0.23.0rc0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 determined/__init__.py,sha256=YP_VEqU7NSA2jILM39YzVkXHiEiHElFWAvQMqF8hA0A,1131
-determined/__version__.py,sha256=nCnRk3Y86wjkY36cdY6zwZll0XF04O1SXof6Uq1Yb3g,27
+determined/__version__.py,sha256=YsGhwJUyijTWl7Ln7Bg2SBgrl40_xsM77gtjUWkZCVE,27
 determined/_env_context.py,sha256=vG1rREr-gp-rVjGUn_5mzKhRxC8qv0RwpNY4rABT_h4,1664
 determined/_execution.py,sha256=sFxJSNK3WnFxVfwCL_O8ZYOKjIvnPVi3pCQYq99Xy5w,8804
 determined/_experiment_config.py,sha256=kkHvFHQzkI3HlckUozKwjfaieWIgeEot9jyPtvQuLjs,2779
 determined/_import.py,sha256=czaz1MQU8w2tfkeD3rIAVDpRyS_7lH0K9Sn-_zm2luQ,4781
 determined/_info.py,sha256=Xm-H3VpeZwYWRPHMmg2Ig1jSeKVU5jekCnuUiqrzrXA,14901
 determined/_tf_rng.py,sha256=Z96_dEFOB2BRWyrthYN1A2FKxGe-fi0XKS_AEupLAnM,1272
 determined/_trial.py,sha256=5GAT_OKfXumm3ykuSRxY8ImTZAUTUBZ9agBVpcMjIEw,1214
@@ -14,63 +14,63 @@
 determined/gpu.py,sha256=WwjXm7jWoLYCxwhPBizcZe_lWMZ3hCFy0PoHG3y9NS0,5431
 determined/horovod.py,sha256=mCY6Ori3zjHQc5CROrkG7PwjJwtC_tAdycIoUOdd9qI,6182
 determined/ipc.py,sha256=kUHkABY-h4rjyphygWCHt_y4Lx0psmSfefOpU33Zbi4,19382
 determined/load.py,sha256=4dSCrArKAatIPhyDT9ofzwBFZ2GC1_0Lvj5jYymFcPc,3065
 determined/monkey_patch.py,sha256=bw-kPbWew541z1G4W4HA7q-zQ5GJwKoysDC4bKk5q9Q,737
 determined/profiler.py,sha256=u9k319yKX2tc5NaY82z2NDZ1eKJPdEcjhn7ySWnDk_M,39670
 determined/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-determined/util.py,sha256=2bQn9GtL1L1Ydc3wfCmlvO2LNbQBoorTuFZEvRmaXEs,15909
+determined/util.py,sha256=h1PrNSiFYCMArxmvkHX_v6U2Ir-uueTky5iRulNPqfU,16449
 determined/workload.py,sha256=UG-9Dt5vGf3mfz4No77o-XjBAXGc4TmUfE1BIYJMveE,6578
-determined/cli/__init__.py,sha256=bQTdOCnCglaql6QQf6i6bUVBCujBAnfpXZItfXmj-78,476
+determined/cli/__init__.py,sha256=m71OR0GjOn7pJvsNLEM3JKFfJLw8mzij7aKdAOXak4o,497
 determined/cli/__main__.py,sha256=xd-S-mXqQ92a37G50DzPszQZ5y1FYXMcQGR52GnTQVA,75
-determined/cli/_util.py,sha256=JAGG_HGeBRRELnOkE9XmGFe0fQtK3ttoZLi0Bt7Jdyo,3423
+determined/cli/_util.py,sha256=Pla9BU9pqOSToi3KtDXGhbFdLVfPG9iHJK8dXr-CS00,4002
 determined/cli/agent.py,sha256=N5N1hJCTODgJZSde3v8pJS2rFYKgqJXz2fpoYw4iDM0,9810
-determined/cli/checkpoint.py,sha256=x6WE71x59AQoDo8zQuwC_-oAgcaKon5HDmzElbZCa3E,6409
-determined/cli/cli.py,sha256=v92SUkawi0sDUrkG7Auw-wEHst-UIjwuyUPQS8CtbVM,12530
-determined/cli/command.py,sha256=X6J05UVhYEZAU2kkQj3VBa0dLdZud3jbINHTX_etRAY,14081
+determined/cli/checkpoint.py,sha256=xGmaH1WXmpj4o8NoH3mD4hAVmXevcfTkFHK9cfFP0U8,8025
+determined/cli/cli.py,sha256=C-K-hpem2SObjfzPJrt0mVX3t3VvGr_P6F3M2yeNlTo,12532
+determined/cli/command.py,sha256=l7S1ew2A9gknEC5WXTajjdRIidJaWx1azCj-JogO0X0,12930
 determined/cli/dev.py,sha256=ekDh1KhnoNM_LcAYmgcucxiQuGr-W9IneZc2BYBnhMA,2138
 determined/cli/errors.py,sha256=VdmkMdIuW4bmU-kFeiPTu6SSTDzBQHxDsEGoKF7ePWY,739
-determined/cli/experiment.py,sha256=_eaOtiGsThhoh8ZcfSdOB9yGN-rLe3QczdbSSkOunXU,50931
+determined/cli/experiment.py,sha256=8HXp_0whfuO0hRbFWAmnLeqqOINZaZ0u-W6udRwT-iI,50903
 determined/cli/job.py,sha256=cmg2s0lKimkguADkUjwfVhhEjKJNvB897lXjaA543ZE,8291
-determined/cli/master.py,sha256=ddeXOYMoy03AkVWp2MYMEqSlPv8Np_I9thItrBVmoGs,2137
+determined/cli/master.py,sha256=TcYshcqgs9rZiCW9FndY5tobSJt7A89-VMcGK8QP_ws,2105
 determined/cli/model.py,sha256=Kw6NGLNhAJYjzj72AMQFwovdcH55lmwQunODdb3ospY,8747
-determined/cli/notebook.py,sha256=F-8oWkReE7kgRLu2UOt3N_o9ZZmm-s9gFAafzjDZ-FQ,5641
+determined/cli/notebook.py,sha256=4yJ7jtG380gtB1-fjQiBQcVQuCrUZ9p4BQASsCgM8aA,5531
 determined/cli/oauth.py,sha256=dN5gSlQAO1V8WXiULqjBefA9xZXuqqibemaXXgQHTN4,1761
-determined/cli/project.py,sha256=J9zrJ2Hl3CCX4XqWP9a-1QzgfNzIqxPmr3I2kxx5PK4,12190
+determined/cli/project.py,sha256=bktia9zo7KL72N0Ml2eHZpWkXUGjpzYuAq-BFuwuQ6M,12162
 determined/cli/proxy.py,sha256=it_szkamnkVje9DI47RKeb5nhFhTpEFBXXFpsxvwGAA,10219
 determined/cli/rbac.py,sha256=jh9wZdHhYwWOiGgteKIDqjG_880AONbyeh1fEHrb5dQ,18787
-determined/cli/remote.py,sha256=4VYwJniNNyzmnNY-5_aVouJ_jGM5ibhdXKryOYQcejQ,3783
-determined/cli/render.py,sha256=iDIOfBX4eLlnmHFETXGDLBrrr30_kBDOpi4TvfiXYFs,4847
+determined/cli/remote.py,sha256=2GWQ2f4f0SVsKIBHnvzD3QSv43jLlGtOp2iEP5loz2g,3846
+determined/cli/render.py,sha256=1f2-31Mczo9xlmr31U2IxwXe820HrRZgGLS18F9HYk4,5948
 determined/cli/resources.py,sha256=31ovXQuf7S9Mpbuf5ueul2fKhBIa1Q3iH3OpMDAqiP4,2372
-determined/cli/shell.py,sha256=lNVpt9smd2ZPKW46_bETXxp7jQpFyvTtn5RiJiFvWqw,9718
+determined/cli/shell.py,sha256=3YhXc1mVDqGRRPfen6pXGmRl_HzuJwK-risWbgXXwnQ,9442
 determined/cli/sso.py,sha256=J1tFaxUn6rlzJH2MGuZ6uIUnRuQGWzT4LyYf_6wJeiQ,5240
-determined/cli/task.py,sha256=f1S-t5c6hw5hVchgWUwd0UYAWikLuXdvjANGAmcRYGE,6400
+determined/cli/task.py,sha256=Bec3KXYBhIDcHnBTce7le-NJkWMMsyso9SjSTWPupOQ,6406
 determined/cli/template.py,sha256=A3y5fxN-COzeZdZ5FMuKB_kzRf8nvx837mghlmKwkig,5354
-determined/cli/tensorboard.py,sha256=mcqwAWvUlCOuu3p6OwkJOYMhDCXA4V3NT4FhE-PNQ4s,8240
+determined/cli/tensorboard.py,sha256=roREWn9DUvfzTpO5zvoU-zrHxo0_lbC2ldFCJ2LsWM0,7525
 determined/cli/top_arg_descriptions.py,sha256=ql_tbzsAmniYKlZ3YQ4bbCNKtDDmkp9Rf8V5dnED3c8,135
-determined/cli/trial.py,sha256=33RVMSSViTT6yt_xgxuqVTwj9X9BYqsM7FNB3bYPhY0,15112
+determined/cli/trial.py,sha256=J1P6XFQ6_l47JNBOtSgMsqVj6BY9o8PozQtQxteRkAA,15033
 determined/cli/tunnel.py,sha256=zCWKTZ0C060XsA5Dc6-g0mqbV4Ll9PmQW9yA76ub_n8,1448
-determined/cli/user.py,sha256=wUgkkIQtgqYG4RNXOktenvJtB0rKsbb2cH2985c_MZI,6875
+determined/cli/user.py,sha256=gKNLaeEPpwgYVS2bslLpfyspr0Ioj-fdW0O7DJmOhsQ,7309
 determined/cli/user_groups.py,sha256=gMWRSCDNoeYIWjuUMUPlKx73buQnmHdxYyb42p0Z_Z8,9754
 determined/cli/version.py,sha256=PaKvNqv3SWlJy8jmX33pqoG5ylVINVPRHNbUgPU3mlA,2557
 determined/cli/workspace.py,sha256=1PFqimxMJuOCBp1047_G8EF_7QTViWcOP3JlUwglqXk,15179
 determined/common/__init__.py,sha256=c9lF3AufKAwXW8_PMl3lbVtBN6yXmPzxI-8IsbS5RTE,352
 determined/common/_logging.py,sha256=q8wQXSRXRv0dAM5QaS8b374juPz2V3txi786PdCgSRM,498
 determined/common/check.py,sha256=7eK_uJj86VR473TCeYUgultitGJGWEGDKXC7PlU_pVM,8593
-determined/common/constants.py,sha256=nlIn6UueZ9-aIsWjDax2KbpDn7nJo6FE-WAzxcLfxvo,2255
+determined/common/constants.py,sha256=IuXKrY7ufO4_u7jwqzO4Su6M3pFfaGDI5TYRKtals0w,2154
 determined/common/context.py,sha256=1P9_iyXKs4fqiWxATpH9Mx17TtmGZ2iWN1cB4nlRl30,8222
 determined/common/declarative_argparse.py,sha256=5BbwY5JUATEMsNbGWj0Ph-6e7oQKi9ydaZz_uCfTXZo,8612
 determined/common/requests.py,sha256=M6NYyQDiXxHq0lHc_OcTrnC4cGQYuXT57V8JNSIon14,1662
-determined/common/util.py,sha256=Jnf-40P5Kf8e2hixJ5Qf0kVwVck33eSlDU0pHBm-1zE,6349
-determined/common/api/__init__.py,sha256=rqCSau19J0fSunDQsIfaUUlpFpspQMPV16JXXKoF2zk,778
+determined/common/util.py,sha256=w_HW8FHdDAVyYiM-CzNJKJeJIs4IXMz1yd_Zd-fFFFI,6867
+determined/common/api/__init__.py,sha256=81IfWqgw6HuKZslOvsKtyym844RE6PobfH25-ZS66zk,821
 determined/common/api/_session.py,sha256=k6j7joLzPUt-nfz99LFswd_FwQiMrWzw_qunBDO3TTI,3383
-determined/common/api/_util.py,sha256=bWa9qzxN2hHmyNfqndVWV8kVXwEG4I5mSCeNn6IMX2I,2840
+determined/common/api/_util.py,sha256=rFR426jWagZpggwhOQwi6DKo47YtGw0iMOVD2L4LPe4,3644
 determined/common/api/analytics.py,sha256=ijoLQ1XHYty88SBpYjTUM-4793lxFfyLM9rnEE15Ghk,1450
 determined/common/api/authentication.py,sha256=pLnS6kpaI32RYnesxHyAlBwTEM2MVM2dkR5CWhDAdGw,16070
-determined/common/api/bindings.py,sha256=2nkGgBptjQodbK4VSc_FMlS3S_JwZyuti0tkO4DZjJ4,619513
+determined/common/api/bindings.py,sha256=hhN-DB9GPQqHegvAX2nzH77lXAdMUlVvbbBOVA4oIGk,627696
 determined/common/api/certs.py,sha256=sltCyZYaGRxnS8LtBpDAMgGTBHaDF_9amKn7UID4-nw,7415
 determined/common/api/errors.py,sha256=WBftwTV5A0CW8erUGtMN1wGYIsVoQjK31FlTFxk0hto,2555
 determined/common/api/logs.py,sha256=gavGnESDPo2v7zJsqRuLOohzYlT975d3fmuzu2wrhIc,3235
 determined/common/api/metric.py,sha256=dR6Opp8sZjRsB3fhZkLKYxLrGkiq1se1Pxsf39udtNw,247
 determined/common/api/profiler.py,sha256=pJ2G9oGFfWrWNmqLXxDlcNfak4C_vgAtUkSEM58cbYY,3147
 determined/common/api/request.py,sha256=Q5w-Slj2Jl8V8gFbL5EPaW8m4AEWI0b2X709ex2BQRs,10416
 determined/common/api/checkpoint/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -80,57 +80,57 @@
 determined/common/experimental/experiment.py,sha256=yKB_Wkgoe_9XKWMg61qnPdCtFWKG-OEzO9WcwntSDl8,11398
 determined/common/experimental/model.py,sha256=6yxsrjQOYv_bTDvi5xw8WNfAv7l4UHgl2bVEJLpRP-k,12639
 determined/common/experimental/oauth2_scim_client.py,sha256=m1wWw4M_QRIyYXc2CC5Mi6aeyaLSIGrAr9wig4bV8qc,306
 determined/common/experimental/session.py,sha256=bcqZPDrznB_BupdqziJCpzvUuxsM4OaowXR7IIcRxs4,466
 determined/common/experimental/trial.py,sha256=vZfKp5Sot5HNGfXsfl5ImkQinnVDgfiNdzA1VL8o_9o,15743
 determined/common/experimental/user.py,sha256=WbDJyBM87bWnE5UYUKdOZlUUUrOoQUoJaBTqREhHrO8,3503
 determined/common/experimental/checkpoint/__init__.py,sha256=aoILZ_tqIFDai-EadxakaCBVkNLEzLBTw7_7X0l1R4I,125
-determined/common/experimental/checkpoint/_checkpoint.py,sha256=9lNT6hA3A5uM7QiwniAVPWnqdYukgW3iwb_lZyTCLC4,13827
-determined/common/storage/__init__.py,sha256=fKv8g8rTvIm40VCTMxOTYpUNeG09xfZ_oy5rT2m1Kwg,3868
-determined/common/storage/azure.py,sha256=ABXIr4sv2fQSrSfKIQ1KS8M-SRCzmOwgof-upwtB5TQ,3822
-determined/common/storage/azure_client.py,sha256=-d_-VhFNagZSzj8LKmO33wdqzxoDjlficVXjL2nUhjE,3514
-determined/common/storage/base.py,sha256=gaj3ysQH56ZYLo9EsJowkGlTN5EZkLdk5uZGmdGFL2k,7152
+determined/common/experimental/checkpoint/_checkpoint.py,sha256=KanidM8OSOwTbZc2GST9O4jKcsO90cPWE-7BxWbi-cg,14995
+determined/common/storage/__init__.py,sha256=F3T8O5r6IpCDHxF94MSCIga2iAvAz9VWev-TTc_Fw-c,3809
+determined/common/storage/azure.py,sha256=KSv5YkhWYcOAOhKyNUIHktcLfGZ5fP9RFfNDJRRfurc,4280
+determined/common/storage/azure_client.py,sha256=Dd04TFhvhupW1RhioWZV1YMV5BOv31tEjPNKaRrFNro,3573
+determined/common/storage/base.py,sha256=8HC7h3RZIrjry56DfpS8669AnPu5l7Vht6W3a_APMH4,9368
 determined/common/storage/boto3_credential_manager.py,sha256=pKb5OabIB53P-Q28Ba-_Vf9LzUgIcgaFhtfBTmDTyqY,4447
 determined/common/storage/cloud.py,sha256=gfv026i7syfE3rVS-1_bFXEGixagKZ7DeopG4l6DNF4,1014
-determined/common/storage/gcs.py,sha256=8-A37OF7pkDViZKWYkO55CI54_eghgEGcto-PAvHfFw,5789
-determined/common/storage/hdfs.py,sha256=LoGxgzXaOHwMv7DXwJndVYq1PRj4eXLLBiYi-ZLrtY0,2070
-determined/common/storage/s3.py,sha256=Q1BEmZJ-rKTnDG_WH8sGuPJ-JFeERH9-HOZ6Ckpc3Xs,6195
-determined/common/storage/shared.py,sha256=NjIAzl09iw4UTkZWUGnFmhBzvzLm946Cu5PqfrbfXAo,7816
+determined/common/storage/gcs.py,sha256=9pkCsxrStgX7aXtz_QbsOMwaN2h0aENH84m1QFxAIjM,6426
+determined/common/storage/s3.py,sha256=kLwEsMowM8X4DD8kanVtHdcGyg7974BRpJWDobYqnj4,6649
+determined/common/storage/shared.py,sha256=iG1Cc6GZb6HZnsqu47G_7aejdPJdRXQPyCitPkLafn0,8972
 determined/core/__init__.py,sha256=DojWVPUz2esaYHa6Ew1ul4pDG5Kw5tM2jxLGb_HyW68,747
-determined/core/_checkpoint.py,sha256=3pd2DP2zH561817wSZxo4v3kW39n7V3_jwpDQ95cImQ,29691
-determined/core/_context.py,sha256=q8EM0DO28q3JlObF8pnn1teD2WZcZFbuk1uzweThiwM,10984
+determined/core/_checkpoint.py,sha256=cNRmw6sbxI1EHLaZGXF6Sd1R7-tXXjdgUKGpC1jzvCY,29425
+determined/core/_context.py,sha256=f629N8EynzFGWF6mZHejyld4GoBRIK3b_ft6divvBcI,11141
 determined/core/_distributed.py,sha256=ittb2-UpitI0vD4nMTKlYd86aB4A4eX-dhDyOSxjfv4,16194
 determined/core/_preempt.py,sha256=PRSTglEO5Rrf-QDm0HLNvuZYV2XDZGwifSGHMj6eVqQ,12738
 determined/core/_searcher.py,sha256=3xHycD5l1UPALTgukcUckjUVGtIo5me5EzY7XEPIAPk,15041
 determined/core/_tensorboard_mode.py,sha256=9A9FKYB77F26wkDTe4LNJWKBn9_4Th3cFzCMWjkl7Lc,932
 determined/core/_train.py,sha256=vfXmBAYCplIKiqRfgarfxnmQxcmseE8dlZSmoPrGYHg,10462
 determined/deploy/__init__.py,sha256=ws1TqRk5eBmOWyQ2zS5wL7-_-QU4pbC4ZJBapG7OvR4,40
 determined/deploy/cli.py,sha256=52jC9NDzNg0dl-voz_fClyW2Ac5kFW95Od50_MVb-2g,1031
 determined/deploy/errors.py,sha256=6PPO8hrAczDcv3pklrGJRG-8bE1ydHP8BmGHx5T0UOg,94
 determined/deploy/healthcheck.py,sha256=8d_YE6I17pndG9PWDBM1Gs3AKxHUzSUFixPExhFPdDM,1472
 determined/deploy/aws/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/aws/aws.py,sha256=8grVdGM2oNDCX1_XHddroQ4kLcla_wSqkLYiHRMbSTU,19597
-determined/deploy/aws/cli.py,sha256=QbWQYTtpLrfovyw6wPFcwaThk09aMYnXHx8sAkznaqA,24035
-determined/deploy/aws/constants.py,sha256=V5aOrV8SvW_ZrNZO4IvwGBB9L60FLELhtkSVR6io_1w,2998
+determined/deploy/aws/cli.py,sha256=IJAiv8C5wxuUt0_lsW2CyxcFMbGgZ1K1kuOQF3dbnxg,24189
+determined/deploy/aws/constants.py,sha256=cqZftqXDzOrn386xv5_ncfY_BHMNM-tRVGZGjTyNqh4,3040
 determined/deploy/aws/gen_vcpu_mapping.py,sha256=XmbbozPADD7RxXhEc1Nkyqm7cElpCgDM_hYo4HB3ezg,1420
 determined/deploy/aws/master_config_inject.py,sha256=_ISaZQIfvDsAyOeDzA7ssE40s6RA-7kMJxqgFiu4k3w,2201
 determined/deploy/aws/preflight.py,sha256=M5T-DYr_wkn2mSjHj2irjq80Br5ODKBmQ7_kTQ9ac1w,4911
 determined/deploy/aws/vcpu_mapping.yaml,sha256=czutxPBg3wIocgCYIKTiv1u8xZtH61hFFqiVig74tPM,17324
 determined/deploy/aws/deployment_types/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/aws/deployment_types/base.py,sha256=4fv1ivcYs43L5qEcG99uiJmfMig4b4gyc7-uhuN1xos,5624
 determined/deploy/aws/deployment_types/govcloud.py,sha256=BjLMhQy9QreojfjBacO2Lg-g-fIVvq4cSDQc_HsDDC4,1593
 determined/deploy/aws/deployment_types/secure.py,sha256=E-EHO1PnlZoi4dXf17PLhSE18ceRjPklTf__2PsHGgQ,3094
-determined/deploy/aws/deployment_types/simple.py,sha256=tNzqZyyWSjkHaAi8OHJJ10B6wTHN4SclOwrx3RHv4BY,1349
+determined/deploy/aws/deployment_types/simple.py,sha256=ocTsYNTcbjW7wMutfyHwy173rTL2qvGcIyMq8H_IESA,1469
 determined/deploy/aws/deployment_types/vpc.py,sha256=4k4pb8ehXO_INC88KMhvwPdqzOI3U4RQtyqpR8n5gRo,1400
 determined/deploy/aws/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-determined/deploy/aws/templates/efs.yaml,sha256=L2Bsi0sFGIWBn8uAXcFir_A7pC4SiT-3NlLAV6I0piU,29259
-determined/deploy/aws/templates/fsx.yaml,sha256=92o-PDrrkULk675Mxtzd5NdKllkoKqB86d7Cuia0HnA,29969
-determined/deploy/aws/templates/govcloud.yaml,sha256=Ope0W2mkaUYuvAG3q8NnCsqXbCIYJCGUNn2MGAwJaVQ,23518
-determined/deploy/aws/templates/secure.yaml,sha256=Dxv6WCuq06KVNF48nR66U8GXaWmeEwgeo_qVWdUgd9U,29153
-determined/deploy/aws/templates/simple.yaml,sha256=DQMkqst0dB_XTiBogHQR9-jOUNnJnGUEZsz-OJgpRzE,24926
+determined/deploy/aws/templates/efs.yaml,sha256=vURpw3cTQlJ11tx6JkZYPn9Y2JoEtr0Ydg3bA99M3to,29341
+determined/deploy/aws/templates/fsx.yaml,sha256=t67J8zaD9tp4SU2YLCSobbWO29-35RJRDs6VN4FSasg,30051
+determined/deploy/aws/templates/govcloud.yaml,sha256=IGIGEbbGSVQw_thCJEhk6FuMAI-vJlukjo8fUFxKUKo,23665
+determined/deploy/aws/templates/secure.yaml,sha256=jNOz5AiKXr3urIUB7zI5F-UobJJ5KvVE0WI9aJxxkuk,29201
+determined/deploy/aws/templates/simple-rds.yaml,sha256=zwgE359tfq7RRDUIW262Lp9_n5wuBHEj2BrD-q0unHA,24822
+determined/deploy/aws/templates/simple.yaml,sha256=IuB__3fVmgJYSXyjPQ_i3mB9j_cf9cDVnBZFWMVOg_E,24974
 determined/deploy/gcp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 determined/deploy/gcp/cli.py,sha256=Ww4a7FSRSDVFy8Qd01oqaZHG6O3BewOula9SqjcsyuU,19015
 determined/deploy/gcp/constants.py,sha256=yEVXwcPybx-R0F2Foj0DCcbAYmCZePKLn3avCP0PS4o,772
 determined/deploy/gcp/gcp.py,sha256=f_Z5roqcXDQzYFH5OZhHFB6bzdkrAAwpZFCcSSQYiXY,12420
 determined/deploy/gcp/preflight.py,sha256=pITWn2fxVKr154OVJA4iPnvYEnNuZVd03dPyaGDX8IM,2380
 determined/deploy/gcp/terraform/main.tf,sha256=5VaCs9G0Fc4U4ypATT_6Ra9tasz398XdrkhIYTdcDNk,5376
 determined/deploy/gcp/terraform/master.yaml.tmpl,sha256=YPrqZ5sJeX_TJ-T3TUR98ov9tX_lNBXhpghSXC-3zMY,1569
@@ -171,24 +171,25 @@
 determined/estimator/_callback.py,sha256=zXdIxEkmxg4HUnXJLD7juHzKmo2MjwzJaEYii4wSsDM,1288
 determined/estimator/_estimator_context.py,sha256=6KLc5mCtY-PxrvkdaiZjKy_V6-JcdjOCvzycpN2A6fU,7375
 determined/estimator/_estimator_trial.py,sha256=RR8lU4B5HGrkLqFlDNfe3lyUPoS3sZDsTxC_vV0SHBk,40175
 determined/estimator/_load.py,sha256=sQy3LfLMkFFwU0YyPS9rYRU3TlMaM0Qu9jdDs3_0HnA,3086
 determined/estimator/_reducer.py,sha256=IV5ErvXlJtgylYkdRf7U-V50rWObTLEQirvow4lsWsg,13742
 determined/estimator/_util.py,sha256=wZ80Iky7WTtoDBkh2r2YVXOE5-DUvEt8kNnb0N5Gayc,9600
 determined/exec/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-determined/exec/gc_checkpoints.py,sha256=u3hVhGhhbd94HZIELtFApHWbxJ0roKIYIXeuqhpdtHQ,3836
+determined/exec/gc_checkpoints.py,sha256=NUxpZYmQmghf20G0Iu2mD7v_E92DhzAKlR5nElPzD_I,5434
 determined/exec/harness.py,sha256=wd_AX84iEpNbaDPljpb9htZmUGLW4U81RIu5m5akN7M,8857
 determined/exec/launch.py,sha256=Tmcl-x0iOqluYdjWlCHi629HUPiT2PFo3X9KiN41cIk,4233
 determined/exec/pid_client.py,sha256=il2K2dxhDcyG1Dt9JnTnrZHCkRy1C0Tdvby_XaqiIa0,389
 determined/exec/pid_server.py,sha256=qJ7l-vPbq7EUTCTOs0tLcItcEpRVrQsF057Om9_OqVU,1476
 determined/exec/prep_container.py,sha256=LPGzLiZRRKM60Aj70CVjVjBi7FRHGu1kTlalABgDiNo,13479
 determined/exec/tensorboard.py,sha256=UgBSPKStCvwkSIFxBv0iAvYyO33o6kr4Bc9FvSSi2zE,10994
-determined/experimental/__init__.py,sha256=bCqcU0cZjPULjjqWUfHr2myj8QNHeCknvxywbOPHS4Y,264
+determined/experimental/__init__.py,sha256=3jgeqlfsb1Kfp4iNNlE-kpqACefiphGh8ul7NFP9kTQ,308
 determined/experimental/_native.py,sha256=yNr0UgfrgI1pICD1nzXprr8vpLIwjV8TLc-o67_X3ls,3473
-determined/experimental/client.py,sha256=2fjLt-VLATf8j_vzx2mxiY4qjMcAOBaDkj7_Ra7zwWU,15160
+determined/experimental/client.py,sha256=guG7MJ9UmlZL3gIiakBwYBVIA3nQpmXFyGLTRhuens4,15330
+determined/experimental/unmanaged.py,sha256=j6MhizobU5NlK4eOku_dY3svl7dmPypKiRR7xgE1VLc,7673
 determined/keras/__init__.py,sha256=qY5vSLMwmjfT3zeBool6fUSxIsFcuj_IhpbdXS42P-0,744
 determined/keras/_data.py,sha256=whHIL5Ky1iIYAQP2LWEWIjJ2jD-yPF-xDll4Pq8V4f8,7579
 determined/keras/_enqueuer.py,sha256=Ocm7bXQPgh9pb25uYTUZbEaQv6PSqx8Ks5fBKrs1WHg,11491
 determined/keras/_load.py,sha256=pFxVc769H70CSPj1s_JjS7X5Siqta_HabpXXszIBRso,4020
 determined/keras/_tensorboard_callback.py,sha256=Tq82-HEeYFKN37A4oq5S0MopPfYqfFF08PWO5I-y1rc,486
 determined/keras/_tf_keras_context.py,sha256=H3bvMo4hVDXK_FYY0ZxiBaIc6fnJnQdu-h_AhsCOEeU,19042
 determined/keras/_tf_keras_multi_gpu.py,sha256=mRO696HAs2ohkZ6JELUgA-TziVveLKhlGP8vWSofa1s,1204
@@ -210,40 +211,47 @@
 determined/pytorch/_metric_utils.py,sha256=4LBvaec5GCLpPki8vmFerH8L0H6OriVUQDByiW_lPwY,8275
 determined/pytorch/_pytorch_context.py,sha256=cUTn2CkC9hVFUIiw6XYff1p9CAqeUa5Ca0GdlTuORbA,45136
 determined/pytorch/_pytorch_trial.py,sha256=Erb1ANq128rqiWvho9sW-tE_a_Bv7SERcNnnTBqhIJM,68474
 determined/pytorch/_reducer.py,sha256=B24ubjL1rrQE-7Lp0ObDikShaO-eN5Dp_jp8Sc_kzRI,21406
 determined/pytorch/_trainer.py,sha256=jo5tXhOTX5JVcCZOajS6jUksW0gVk4l6OrfcFHmAgSQ,13510
 determined/pytorch/samplers.py,sha256=I4fU64xjwGi2PRGyznsqHe_QUmlWBHNsTVfe_2OzwDQ,9561
 determined/pytorch/deepspeed/__init__.py,sha256=loC0PUxi7Y21cFjeP3KFxV3omSaTpw4TwOQb1sTp0q8,347
-determined/pytorch/deepspeed/_deepspeed_context.py,sha256=peq9-vLRcmbQCkUNd3AekzRH7c_oj3OIg_Idc6w0cIk,17524
-determined/pytorch/deepspeed/_deepspeed_trial.py,sha256=xeeNOM8wRT4--uPP72ZHg5u2oyi2ljXVC1cNXALNqZo,42777
+determined/pytorch/deepspeed/_deepspeed_context.py,sha256=8r5bOhXy0bbDqiZm8zKh7rkX4cdO4Q1DzKDUHjsua6Q,17164
+determined/pytorch/deepspeed/_deepspeed_trial.py,sha256=5XgIXumIkQPQKEw98sLui5_U58Tb5HVAzeSfcnXfnrE,43712
 determined/pytorch/deepspeed/_mpu.py,sha256=NFyfpLc12wv5HT13WlkN7uos-YgKu08px-ksycPuABE,1987
+determined/pytorch/dsat/__init__.py,sha256=-QZ-kMyfk7B8sjQO5I2O2P4_i1yFWyPN7DnYxUl8R1k,409
+determined/pytorch/dsat/__main__.py,sha256=pT7E5rd8Ok8gkrPYKIbEh9Edg_YA_AJn1ARnxS5pdNk,1738
+determined/pytorch/dsat/_defaults.py,sha256=KyRdNpLavu0QNND1UX5NArGiSMSp04bFPNUwfinSeyg,2541
+determined/pytorch/dsat/_dsat_search_method.py,sha256=oFpNJfw7iwMAiow5cnD4bpsWAYUlxQxn0EAF1KU8Yd8,60199
+determined/pytorch/dsat/_run_dsat.py,sha256=aMMqjDB7rtyyDLKXLSy5sNnNJHb_89u7s1W6gs9jVfE,3736
+determined/pytorch/dsat/_utils.py,sha256=Q-3s9sUIykrQDKvHvaoL676dNinzy_dEf03O_d452KQ,20100
 determined/pytorch/lightning/__init__.py,sha256=hEeHjZvrU6v8nwpuCA_z096_epOeQgY6JcGbob2kazA,67
 determined/pytorch/lightning/_adapter.py,sha256=vVZib7VrO_s1Cp_xXqoc72zkzz1HfVaIad3qMzmaF80,18157
 determined/searcher/__init__.py,sha256=-Sm5zl0JICEArfNcAdo6Zz6sodpNDC5uQY5z1DPPz-Y,343
-determined/searcher/_remote_search_runner.py,sha256=2DZ71x0dUddaEYoDsC01Xai3TkPKoA7kwe2yGTCXcIw,3563
-determined/searcher/_search_method.py,sha256=opv4CuaAco4yw3OTP-ZjTOmsOu96yJTdGY3SsIxMSNI,10081
-determined/searcher/_search_runner.py,sha256=2g48Ea8zSIgx4FkhcyFBm3OJjifIuxvDyK1y1qyfUOc,14053
+determined/searcher/_remote_search_runner.py,sha256=JgH5Zsc4t6noAvjrM93B-GL-QQX3OHN_Vhqzknenc90,4051
+determined/searcher/_search_method.py,sha256=Vc7lKMisQKLLCJ92CZLiEsbYy0YDJ_lpcfLdP9JpZRw,16443
+determined/searcher/_search_runner.py,sha256=Vqlb1CbvrTkpv4fkML8hFp67PRgcBlYP-_1QSZjAJQg,15851
 determined/tensorboard/__init__.py,sha256=y462s2t7U1mJ8qu_cOkL4lFO7Z6_P5665E1uoZ2_HB4,512
 determined/tensorboard/azure.py,sha256=JS7cKd0WJqtyRNC5ruHrjcK2mYrpnsh26MbJe8blOAs,1573
 determined/tensorboard/base.py,sha256=WXgvr-SI9P-gt8b6hinn65qzyNVhaY1Z_83VCv86VDs,5884
-determined/tensorboard/build.py,sha256=8HSDqruyncw21cFx45JUfE1g52pTglW-ObOMvPLAD6w,4534
+determined/tensorboard/build.py,sha256=avpyfw6njPCeCapmGv5afYvqQwmk89UsIqZG7vul_GU,4008
 determined/tensorboard/gcs.py,sha256=PlMMve-jX1xOWPImTIWdKBSJmBdl1EsF04FVop_q22Q,2305
-determined/tensorboard/hdfs.py,sha256=sDk9amJtPclfid-ANEdCql6WoSGmx3s3_JbWXSRK5nM,1333
 determined/tensorboard/s3.py,sha256=kwil2SLZA2Jow1jS6BrDt8dTP_tN-J7LgG58HqfnAPA,1892
 determined/tensorboard/shared.py,sha256=mY0p0ROgNdVMBxATQPA4bfHu-IRXUm96JC2gbgII3BI,1747
 determined/tensorboard/util.py,sha256=OyjE7wQciwNpoyRTLy4l1Yt4LIiw2BG_EPiBxHaib1M,3734
 determined/tensorboard/fetchers/__init__.py,sha256=RJwajFxJjfEYaao52IL7Nm9GvqI13KL-s0fkNvjmBo8,780
 determined/tensorboard/fetchers/azure.py,sha256=koGdyJa0W0SYvw4Vw0HJ9_jyp9Owy1Gu5Vi_odnn6UA,2534
 determined/tensorboard/fetchers/base.py,sha256=rtCswUPmHTNr2f7hejAaibfqcgU1pTypl6zXeKekiEc,1670
 determined/tensorboard/fetchers/gcs.py,sha256=TBCIKfdT6NsDiWRtWuo3NP-YKV2l6hf8zAVyOrFopWY,1733
 determined/tensorboard/fetchers/s3.py,sha256=8Vprb72laPQfPAwr48RMBCzei2IShcAsrQqYxxizTCA,2476
 determined/tensorboard/fetchers/shared.py,sha256=7p-l7hyCuViVaf4hiqxjBmB4Sxl3_F61ojFtaFmX3cc,1634
 determined/tensorboard/metric_writers/__init__.py,sha256=QBZlDYJslTPnllbOOwzbV_XtKlsLwf9SR8YcL3MdJtY,91
 determined/tensorboard/metric_writers/callback.py,sha256=pwNoskesXSRWaU7EimdhwEq0QP3HkkqgyCjrwd9Mc0g,2113
 determined/tensorboard/metric_writers/pytorch.py,sha256=dfEZRibe9Tkps768n_uLrYOWe8TOtrg9hfCsI2pKayc,2936
 determined/tensorboard/metric_writers/tensorflow.py,sha256=fQA1jtA6xCFEGoT5bf2YgZ4YBr9KbWRewfMOwTyCxh4,4385
-determined-0.22.2rc1.dist-info/METADATA,sha256=-pbnqtCW-uMV7QNQshrqelNbS7Rf3nTIAwH3uB5J3wI,1262
-determined-0.22.2rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-determined-0.22.2rc1.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
-determined-0.22.2rc1.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
-determined-0.22.2rc1.dist-info/RECORD,,
+determined/transformers/__init__.py,sha256=WJSvfLUkyIXjrbAKEe-SRXYdl8ZuDceqztiZ0ASJKIA,70
+determined/transformers/_hf_callback.py,sha256=wlnHXPtdQ_U2HrqhhydY096x1W75NJlaTSbMQem6dI8,12727
+determined-0.23.0rc0.dist-info/METADATA,sha256=6CQ_ydzCeX-3TJ8EG6gEtZefeoL2Vgew4Lo5Forf4Ws,1232
+determined-0.23.0rc0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined-0.23.0rc0.dist-info/entry_points.txt,sha256=77kPxwpCZJKt-eI0btTdFhbgHTB1vYCIeaxnrbu9cPg,53
+determined-0.23.0rc0.dist-info/top_level.txt,sha256=6KMmvfzgIXKT6XhfIA5qmqlIv8-Yk90UBTekhDjhk0U,11
+determined-0.23.0rc0.dist-info/RECORD,,
```


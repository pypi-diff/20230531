# Comparing `tmp/agixt-1.1.74b0.tar.gz` & `tmp/agixt-1.1.75b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.74b0.tar", max compression
+gzip compressed data, was "agixt-1.1.75b0.tar", max compression
```

## Comparing `agixt-1.1.74b0.tar` & `agixt-1.1.75b0.tar`

### file list

```diff
@@ -1,106 +1,105 @@
--rw-r--r--   0        0        0     1087 2023-05-28 13:13:33.049862 agixt-1.1.74b0/LICENSE
--rw-r--r--   0        0        0    19453 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    14134 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Agent.py
--rw-r--r--   0        0        0     6918 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Chain.py
--rw-r--r--   0        0        0     6224 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Commands.py
--rw-r--r--   0        0        0     1101 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Config.py
--rw-r--r--   0        0        0     1960 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/CustomPrompt.py
--rw-r--r--   0        0        0     7045 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Embedding.py
--rw-r--r--   0        0        0      606 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Main.py
--rw-r--r--   0        0        0     9619 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Memories.py
--rw-r--r--   0        0        0     7128 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      236 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12742 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/app.py
--rw-r--r--   0        0        0     1609 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1410 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/auth_libs/Login.py
--rw-r--r--   0        0        0     5840 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/auth_libs/Profile.py
--rw-r--r--   0        0        0     1165 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     1866 2023-05-28 13:13:33.049862 agixt-1.1.74b0/agixt/auth_libs/Register.py
--rw-r--r--   0        0        0     3229 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0     1624 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/audio_text.py
--rw-r--r--   0        0        0      555 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/chain_commands.py
--rw-r--r--   0        0        0     3826 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/cicd.py
--rw-r--r--   0        0        0     1074 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/create_new_command.py
--rw-r--r--   0        0        0     2862 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/discord_commands.py
--rw-r--r--   0        0        0     3242 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/execute_code.py
--rw-r--r--   0        0        0     4285 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/file_operations.py
--rw-r--r--   0        0        0     1823 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/github.py
--rw-r--r--   0        0        0     2899 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/google.py
--rw-r--r--   0        0        0     2254 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/image_generator.py
--rw-r--r--   0        0        0     4198 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/microsoft_365_email.py
--rw-r--r--   0        0        0     1561 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/searxng_commands.py
--rw-r--r--   0        0        0      989 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/sendgrid_email.py
--rw-r--r--   0        0        0      303 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/times.py
--rw-r--r--   0        0        0     1157 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/twitter.py
--rw-r--r--   0        0        0     2899 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/voice.py
--rw-r--r--   0        0        0     2269 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/web_playwright.py
--rw-r--r--   0        0        0     3432 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/web_requests.py
--rw-r--r--   0        0        0     4357 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/web_selenium.py
--rw-r--r--   0        0        0      949 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/commands/work_with_ai.py
--rw-r--r--   0        0        0     1566 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/config.yaml
--rw-r--r--   0        0        0    11963 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/example.ipynb
--rw-r--r--   0        0        0     1132 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/model-prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1132 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/model-prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      777 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/model-prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      569 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/model-prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0    10456 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     1726 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2779 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/2-Chat.py
--rw-r--r--   0        0        0     2887 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/3-Instructions.py
--rw-r--r--   0        0        0     1571 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/4-Tasks.py
--rw-r--r--   0        0        0    11954 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/5-Chains.py
--rw-r--r--   0        0        0     2513 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/pages/6-Custom_Prompts.py
--rw-r--r--   0        0        0      145 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1018 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1132 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      424 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      316 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      441 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      474 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      270 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      782 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0      730 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0     2147 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1385 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1035 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-05-28 13:13:33.053862 agixt-1.1.74b0/agixt/starchat.sh
--rw-r--r--   0        0        0    13595 2023-05-28 13:13:33.057862 agixt-1.1.74b0/docs/README.md
--rw-r--r--   0        0        0     2806 2023-05-28 13:13:33.069862 agixt-1.1.74b0/pyproject.toml
--rw-r--r--   0        0        0    16397 1970-01-01 00:00:00.000000 agixt-1.1.74b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-31 00:15:01.082069 agixt-1.1.75b0/LICENSE
+-rw-r--r--   0        0        0    19540 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    14146 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Agent.py
+-rw-r--r--   0        0        0     7187 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Config.py
+-rw-r--r--   0        0        0     7045 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6462 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Main.py
+-rw-r--r--   0        0        0     9750 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7128 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12677 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1566 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     5982 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      854 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1168 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1164 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6605 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1829 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2036 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      533 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2451 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      616 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4198 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1887 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0      995 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      309 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1163 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2275 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     1970 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13354 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2779 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     2887 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1571 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      424 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      308 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3100 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0    13585 2023-05-31 00:15:01.090069 agixt-1.1.75b0/docs/README.md
+-rw-r--r--   0        0        0     2806 2023-05-31 00:15:01.098069 agixt-1.1.75b0/pyproject.toml
+-rw-r--r--   0        0        0    16387 1970-01-01 00:00:00.000000 agixt-1.1.75b0/PKG-INFO
```

### Comparing `agixt-1.1.74b0/LICENSE` & `agixt-1.1.75b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/AGiXT.py` & `agixt-1.1.75b0/agixt/AGiXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import asyncio
 import regex
 import json
 import time
 import spacy
 from datetime import datetime
 from Agent import Agent
-from CustomPrompt import CustomPrompt
-from commands.searxng_commands import searxng_commands
+from Prompts import Prompts
+from extensions.searxng import searxng
 from urllib.parse import urlparse
 import logging
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
@@ -61,15 +61,15 @@
         task: str = "",
         top_results: int = 5,
         prompt="",
         chain_name="",
         step_number=0,
         **kwargs,
     ):
-        cp = CustomPrompt()
+        cp = Prompts()
         if prompt == "":
             prompt = task
         else:
             try:
                 prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
             except:
                 prompt = prompt
@@ -407,41 +407,40 @@
                                     task=task,
                                     prompt="Validation",
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=command_output,
                                     **kwargs,
                                 )
+                                if validate_command.startswith("Yes"):
+                                    # Failed command execution
+                                    return self.revalidation_agent(
+                                        task=task,
+                                        command_name=command_name,
+                                        command_args=command_args,
+                                        command_output=command_output,
+                                        context_results=context_results,
+                                        **kwargs,
+                                    )
+                                else:
+                                    # Successful command execution
+                                    logging.info(
+                                        f"Command {command_name} executed successfully with args {command_args}. Command Output: {command_output}"
+                                    )
+                                    response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
+                                    return response
                             except:
                                 return self.revalidation_agent(
-                                    task,
-                                    command_name,
-                                    command_args,
-                                    command_output,
-                                    **kwargs,
-                                )
-
-                            if validate_command.startswith("Y"):
-                                logging.info(
-                                    f"Command {command_name} executed successfully with args {command_args}."
-                                )
-                                response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
-                                return response
-                            else:
-                                revalidate = self.run(
                                     task=task,
-                                    prompt="ValidationFailed",
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=command_output,
+                                    context_results=context_results,
                                     **kwargs,
                                 )
-                                return self.execution_agent(
-                                    execution_response, task, context_results, **kwargs
-                                )
                 else:
                     if command_name == "None.":
                         return "\nNo commands were executed.\n"
                     else:
                         return f"\Command not recognized: {command_name} ."
         except:
             logging.info("\nERROR IN EXECUTION_AGENT, validated_response:\n")
@@ -500,16 +499,14 @@
         for result in results:
             search_string = result.lstrip("0123456789. ")
             try:
                 searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
             except:
                 searx_server = ""
             try:
-                links = searxng_commands(
-                    SEARXNG_INSTANCE_URL=searx_server
-                ).search_searx(search_string)
+                links = searxng(SEARXNG_INSTANCE_URL=searx_server).search(search_string)
                 if len(links) > depth:
                     links = links[:depth]
             except:
                 links = None
             if links is not None:
                 await resursive_browsing(task, links)
```

### Comparing `agixt-1.1.74b0/agixt/Agent.py` & `agixt-1.1.75b0/agixt/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 import yaml
 import time
 from pathlib import Path
 from inspect import signature, Parameter
 from provider import Provider
 from Memories import Memories
-from Commands import Commands
+from Extensions import Extensions
 
 DEFAULT_SETTINGS = {
     "provider": "gpt4free",
     "AI_MODEL": "gpt-4",
     "AI_TEMPERATURE": "0.7",
     "MAX_TOKENS": "4000",
     "embedder": "default",
@@ -24,17 +24,17 @@
 class Agent:
     def __init__(self, agent_name=None):
         # General Configuration
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
         self.commands = self.load_commands()
-        self.available_commands = Commands(self.AGENT_CONFIG).get_available_commands()
+        self.available_commands = Extensions(self.AGENT_CONFIG).get_available_commands()
         self.clean_agent_config_commands()
-        self.execute = Commands(self.AGENT_CONFIG).execute_command
+        self.execute = Extensions(self.AGENT_CONFIG).execute_command
         # AI Configuration
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
             self._load_agent_config_keys(["AI_MODEL", "AI_TEMPERATURE", "MAX_TOKENS"])
@@ -153,18 +153,18 @@
                 params[name] = None
             else:
                 params[name] = param.default
         return params
 
     def load_commands(self):
         commands = []
-        command_files = glob.glob("commands/*.py")
+        command_files = glob.glob("extensions/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
-            module = importlib.import_module(f"commands.{module_name}")
+            module = importlib.import_module(f"extensions.{module_name}")
             command_class = getattr(module, module_name.lower())()
             if hasattr(command_class, "commands"):
                 for command_name, command_function in command_class.commands.items():
                     params = self.get_command_params(command_function)
                     commands.append((command_name, command_function.__name__, params))
         return commands
```

### Comparing `agixt-1.1.74b0/agixt/Chain.py` & `agixt-1.1.75b0/agixt/Chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 from AGiXT import AGiXT
 import argparse
-from CustomPrompt import CustomPrompt
-from Commands import Commands
+from Prompts import Prompts
+from Extensions import Extensions
 import logging
 
 
 class Chain:
     def get_chain(self, chain_name):
         with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
             chain_data = json.load(f)
@@ -27,80 +27,84 @@
     def rename_chain(self, chain_name, new_name):
         os.rename(
             os.path.join("chains", f"{chain_name}.json"),
             os.path.join("chains", f"{new_name}.json"),
         )
 
     def add_chain_step(self, chain_name, step_number, agent_name, prompt_type, prompt):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         chain_data["steps"].append(
             {
                 "step": step_number,
                 "agent_name": agent_name,
                 "prompt_type": prompt_type,
                 "prompt": prompt,
             }
         )
         with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
             json.dump(chain_data, f)
 
     def update_step(self, chain_name, step_number, agent_name, prompt_type, prompt):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         for step in chain_data["steps"]:
             if step["step"] == step_number:
                 step["agent_name"] = agent_name
                 step["prompt_type"] = prompt_type
                 step["prompt"] = prompt
                 break
         with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
             json.dump(chain_data, f)
 
     def delete_step(self, chain_name, step_number):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         chain_data["steps"] = [
             step for step in chain_data["steps"] if step["step"] != step_number
         ]
         with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
             json.dump(chain_data, f)
 
     def delete_chain(self, chain_name):
         os.remove(os.path.join("chains", f"{chain_name}.json"))
 
     def get_step(self, chain_name, step_number):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         for step in chain_data["steps"]:
             if step["step"] == step_number:
                 return step
         return None
 
     def get_steps(self, chain_name):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         return chain_data["steps"]
 
     def run_chain(self, chain_name):
-        chain_data = self.get_chain(chain_name)
+        chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
                 step_response = self.run_chain_step(
-                    step_data, chain_name
+                    step=step_data, chain_name=chain_name
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
+                logging.info(f"Response: {step_response}")
         # Write the responses to the json file.
         with open(os.path.join("chains", f"{chain_name}_responses.json"), "w") as f:
             json.dump(responses, f)
         return responses
 
-    def get_step_response(self, chain_name, step_number):
+    def get_step_response(self, chain_name, step_number="all"):
         try:
-            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+            with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
                 responses = json.load(f)
-            return responses.get(str(step_number))
+            if step_number == "all":
+                return responses
+            else:
+                return responses.get(str(step_number))
         except:
             return ""
 
     def get_step_content(self, chain_name, step_number, prompt_content):
         if "{STEP" in prompt_content:
             # get the step number from the prompt content
             step_number = int(
@@ -114,37 +118,37 @@
             )
             # replace the {STEPx} with the response
             prompt_content = prompt_content.replace(
                 f"{{STEP{step_number}}}", step_response
             )
         return prompt_content
 
-    def run_chain_step(self, step, chain_name):
+    def run_chain_step(self, step: dict = {}, chain_name=""):
         logging.info(step)
         if step:
             if "prompt_type" in step:
                 prompt_type = step["prompt_type"]
                 prompt = step["prompt"]
                 agent_name = step["agent_name"]
                 step_number = step["step"]
                 try:
                     command_name = prompt["command_name"]
                 except:
                     command_name = ""
                 if prompt_type == "Command":
-                    commands_args = prompt
-                    for prompt_content in prompt:
-                        commands_args[prompt_content] = self.get_step_content(
-                            chain_name, step_number, prompt_content
+                    commands_args = prompt.copy()
+                    for arg in commands_args:
+                        commands_args[arg] = self.get_step_content(
+                            chain_name, step_number, commands_args[arg]
                         )
-                    return Commands(agent_name=agent_name).execute_command(
-                        command_name, commands_args
+                    return Extensions(agent_config=agent_name).execute_command(
+                        command_name=command_name, command_args=commands_args
                     )
                 try:
-                    prompt_content = CustomPrompt().get_prompt(
+                    prompt_content = Prompts().get_prompt(
                         prompt_name=prompt["prompt_name"]
                     )
                     prompt_content = self.get_step_content(
                         chain_name, step_number, prompt_content
                     )
                     agent = AGiXT(agent_name)
                 except:
@@ -171,8 +175,8 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--chain", type=str, default="")
     args = parser.parse_args()
     chain_name = args.chain
-    Chain().run_chain(chain_name)
+    Chain().run_chain(chain_name=chain_name)
```

### Comparing `agixt-1.1.74b0/agixt/Commands.py` & `agixt-1.1.75b0/agixt/Extensions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import importlib
 import os
 import glob
+import json
 from inspect import signature, Parameter
 import logging
 
 
-class Commands:
-    def __init__(self, agent_config, load_commands_flag: bool = True):
+class Extensions:
+    def __init__(self, agent_config, load_commands_flag: bool = True, agent_name=""):
         self.agent_config = agent_config
         if load_commands_flag:
             self.commands = self.load_commands()
         else:
             self.commands = []
         self.available_commands = self.get_available_commands()
 
@@ -61,19 +62,19 @@
 
     def load_commands(self):
         try:
             settings = self.agent_config["settings"]
         except:
             settings = {}
         commands = []
-        command_files = glob.glob("commands/*.py")
+        command_files = glob.glob("extensions/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
-            module = importlib.import_module(f"commands.{module_name}")
-            if issubclass(getattr(module, module_name), Commands):
+            module = importlib.import_module(f"extensions.{module_name}")
+            if issubclass(getattr(module, module_name), Extensions):
                 command_class = getattr(module, module_name)(**settings)
                 if hasattr(command_class, "commands"):
                     for (
                         command_name,
                         command_function,
                     ) in command_class.commands.items():
                         params = self.get_command_params(command_function)
@@ -88,19 +89,19 @@
                         )
         # Return the commands list
         logging.debug(f"loaded commands: {commands}")
         return commands
 
     def get_extension_settings(self):
         settings = {}
-        command_files = glob.glob("commands/*.py")
+        command_files = glob.glob("extensions/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
-            module = importlib.import_module(f"commands.{module_name}")
-            if issubclass(getattr(module, module_name), Commands):
+            module = importlib.import_module(f"extensions.{module_name}")
+            if issubclass(getattr(module, module_name), Extensions):
                 command_class = getattr(module, module_name)()
                 params = self.get_command_params(command_class.__init__)
                 # Remove self and kwargs from params
                 if "self" in params:
                     del params["self"]
                 if "kwargs" in params:
                     del params["kwargs"]
@@ -118,39 +119,39 @@
                 params[name] = None
             else:
                 params[name] = param.default
         return params
 
     def find_command(self, command_name: str):
         for name, module, function_name, params in self.commands:
-            if function_name == command_name:
+            if name == command_name:
                 command_function = getattr(module, function_name)
                 return command_function, module, params  # Updated return statement
         return None, None, None  # Updated return statement
 
     def get_commands_list(self):
         self.commands = self.load_commands(agent_name=self.agent_name)
         commands_list = [command_name for command_name, _, _ in self.commands]
         return commands_list
 
     def execute_command(self, command_name: str, command_args: dict = None):
-        command_function, module, params = self.find_command(command_name)
+        command_function, module, params = self.find_command(command_name=command_name)
+        logging.info(
+            f"Executing command: {command_name} with args: {command_args}. Command Function: {command_function}"
+        )
         if command_function is None:
+            logging.error(f"Command {command_name} not found")
             return False
-
-        if command_args is None:
-            command_args = {}
-
-        if not isinstance(command_args, dict):
-            return f"Error: command_args should be a dictionary, but got {type(command_args).__name__}"
-
-        for name, value in command_args.items():
-            if name in params:
-                params[name] = value
-
+        for param in params:
+            if param not in command_args:
+                if param != "self" and param != "kwargs":
+                    command_args[param] = None
+        args = command_args.copy()
+        for param in command_args:
+            if param not in params:
+                del args[param]
         try:
-            command_class = module()
-            output = getattr(command_class, command_function.__name__)(**params)
+            output = getattr(module(), command_function.__name__)(**args)
         except Exception as e:
             output = f"Error: {str(e)}"
-
+        logging.info(f"Command Output: {output}")
         return output
```

### Comparing `agixt-1.1.74b0/agixt/Config.py` & `agixt-1.1.75b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/CustomPrompt.py` & `agixt-1.1.75b0/agixt/Prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 
 
-class CustomPrompt:
+class Prompts:
     def add_prompt(self, prompt_name, prompt):
         # if prompts folder does not exist, create it
         if not os.path.exists("prompts"):
             os.mkdir("prompts")
         # if prompt file does not exist, create it
         if not os.path.exists(os.path.join("prompts", f"{prompt_name}.txt")):
             with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
                 f.write(prompt)
 
     def get_prompt(self, prompt_name, model="default"):
         try:
-            with open(f"model-prompts/{model}/{prompt_name}.txt", "r") as f:
+            with open(f"prompts/{model}/{prompt_name}.txt", "r") as f:
                 return f.read()
         except:
             try:
                 with open(os.path.join("prompts", f"{prompt_name}.txt"), "r") as f:
                     prompt = f.read()
                 return prompt
             except:
@@ -44,9 +44,9 @@
         os.remove(os.path.join("prompts", f"{prompt_name}.txt"))
 
     def update_prompt(self, prompt_name, prompt):
         with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
             f.write(prompt)
 
     def get_model_prompt(self, prompt_name, model="default"):
-        with open(f"model-prompts/{model}/{prompt_name}.txt", "r") as f:
+        with open(f"prompts/{model}/{prompt_name}.txt", "r") as f:
             return f.read()
```

### Comparing `agixt-1.1.74b0/agixt/Embedding.py` & `agixt-1.1.75b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/Main.py` & `agixt-1.1.75b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/Memories.py` & `agixt-1.1.75b0/agixt/Memories.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from collections import Counter
 import pandas as pd
 import docx2txt
 import pdfplumber
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup
 import logging
+import asyncio
+import sys
+
+if sys.platform == "win32":
+    asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
 
 
 class Memories:
     def __init__(self, agent_name: str = "AGiXT", agent_config=None):
         self.agent_name = agent_name
         self.agent_config = agent_config
         self.chroma_client = None
```

### Comparing `agixt-1.1.74b0/agixt/Tasks.py` & `agixt-1.1.75b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/app.py` & `agixt-1.1.75b0/agixt/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from Config import Config
 from AGiXT import AGiXT
 from Agent import Agent
-from Commands import Commands
 from Chain import Chain
 from Tasks import Tasks
-from CustomPrompt import CustomPrompt
+from Prompts import Prompts
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
 import os
 import logging
 
 CFG = Config()
@@ -366,48 +365,48 @@
     Chain().delete_step(chain_name, step_number)
     return {"message": f"Step {step_number} deleted from chain '{chain_name}'."}
 
 
 @app.post("/api/prompt", tags=["Prompt"])
 async def add_prompt(prompt: CustomPromptModel) -> ResponseMessage:
     try:
-        CustomPrompt().add_prompt(prompt.prompt_name, prompt.prompt)
+        Prompts().add_prompt(prompt.prompt_name, prompt.prompt)
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' added.")
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @app.get("/api/prompt/{prompt_name}", tags=["Prompt"], response_model=CustomPromptModel)
 async def get_prompt(prompt_name: str):
     try:
-        prompt_content = CustomPrompt().get_prompt(prompt_name)
+        prompt_content = Prompts().get_prompt(prompt_name)
         return {"prompt_name": prompt_name, "prompt": prompt_content}
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.get("/api/prompt", response_model=PromptList, tags=["Prompt"])
 async def get_prompts():
-    prompts = CustomPrompt().get_prompts()
+    prompts = Prompts().get_prompts()
     return {"prompts": prompts}
 
 
 @app.delete("/api/prompt/{prompt_name}", tags=["Prompt"])
 async def delete_prompt(prompt_name: str) -> ResponseMessage:
     try:
-        CustomPrompt().delete_prompt(prompt_name)
+        Prompts().delete_prompt(prompt_name)
         return ResponseMessage(message=f"Prompt '{prompt_name}' deleted.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.put("/api/prompt/{prompt_name}", tags=["Prompt"])
 async def update_prompt(prompt: CustomPromptModel) -> ResponseMessage:
     try:
-        CustomPrompt().update_prompt(prompt.prompt_name, prompt.prompt)
+        Prompts().update_prompt(prompt.prompt_name, prompt.prompt)
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' updated.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=7437)
```

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.75b0/agixt/auth_libs/Cfig.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,7 +51,14 @@
         """
         Sets the authentication setup configuration.
         """
         config = self.load_config()
         config["auth_setup_config"] = setup_config
         config["auth_setup"] = True
         self.save_config(config)
+
+    def get_admin_email(self):
+        config = self.load_config()
+        if "admin_email" in config:
+            return config["admin_email"]
+        else:
+            return False
```

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Login.py` & `agixt-1.1.75b0/agixt/pages/Login.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import streamlit as st
 import bcrypt
+import time
 from auth_libs.Cfig import Cfig
 from auth_libs.Users import (
     load_users,
     save_user_data,
     configure_auth_settings,
     check_admin_configured,
 )
 from auth_libs.Users import check_auth_status
 
+logged = st.session_state.get("logged_in")
+if logged:
+    st.session_state["login_page"] = True
 check_auth_status()
 CFIG = Cfig()
 
 
 # Login form
 def login_form():
     """
@@ -29,24 +33,28 @@
     st.write("Please log in")
     email = st.text_input("Email")
     password = st.text_input("Password", type="password")
 
     if st.button("Login"):
         for user in user_data["users"]:
             if user["email"] == email:
+                # st.write("Email: " + str(user["email"]))
+                # st.write(" Input Pass: " + str(bcrypt.hashpw(password.encode(),user["password_hash"].encode(),)))
+                # st.write(" Saved Pass: " + str(user["password_hash"].encode("utf-8")))
                 if bcrypt.checkpw(
                     password.encode("utf-8"), user["password_hash"].encode("utf-8")
                 ):
                     st.success("Login successful!")
                     st.session_state["logged_in"] = True
                     st.session_state["email"] = email
+                    time.sleep(1)
                     st.experimental_rerun()  # Redirect to UI
-                    break
         else:
             st.error("Incorrect email or password.")
+        st.stop()
 
 
 # Check if admin configuration is needed
 if not check_admin_configured():
     configure_auth_settings()
     st.stop()
```

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Profile.py` & `agixt-1.1.75b0/agixt/pages/Profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 import streamlit as st
 import bcrypt
 from auth_libs.Users import load_users, save_user_data
 from auth_libs.Cfig import Cfig
-from auth_libs.Users import check_auth_status
+from auth_libs.Users import check_auth_status, logout_button
 from components.agent_selector import agent_selector
+import logging
 
-check_auth_status()
-agent_name, agent = agent_selector()
-CFG = Cfig()
 
 # Check if the user is logged in
-
-
-def logout_button():
-    """
-    Renders the logout button.
-    """
-    if st.button("Logout"):
-        # Clear session state and redirect to the login page
-        st.session_state.clear()
-        st.experimental_rerun()  # Redirect to the login page
+st.session_state["login_page"] = "Profile_Page"
+check_auth_status()
+st.session_state["login_page"] = False
+agent_name, agent = agent_selector()
+CFIG = Cfig()
 
 
 # Toggle public registrations
-def toggle_value(val, to_toggle="allow_reg"):
-    setup_cfg = CFG.load_cfg_data()
-    for config in setup_cfg["config"]:
-        config[to_toggle] = val
-    CFG.save_cfg_data(setup_cfg)
+def toggle_value(val, to_toggle=0):
+    setup_CFIG = CFIG.load_config()
+    setup_CFIG["config"][to_toggle] = val
+    CFIG.save_config(setup_CFIG)
 
     if val == False:
         st.success("Setting Disabled!")
     else:
         st.success("Setting Enabled!")
 
     st.session_state["regCheck"] = val
@@ -63,15 +55,17 @@
                 else:
                     st.error("Incorrect current password.")
                 break
 
 
 # Create user form (admin only)
 def create_user_form():
-    admin_email = CFG.get_admin_email()
+    admin_email = CFIG.get_admin_email()
+    if not admin_email:
+        st.write("You are not logged in, or login is not enabled.")
     if st.session_state["email"] != admin_email:
         st.error("Only the admin can create new users.")
         return
     st.write("Create User")
     email = st.text_input("Email")
     password = st.text_input("Password", type="password")
     confirm_password = st.text_input("Confirm Password", type="password")
@@ -93,85 +87,93 @@
                 "password_hash": hashed_password.decode("utf-8"),
                 "admin": "False",
             }
             user_data["users"].append(new_user)
             save_user_data(user_data)
             st.success("User created successfully!")
 
+    admin_email = CFIG.get_admin_email()
 
-try:
-    admin_email = CFG.get_admin_email()
-    logout_button()
-    if st.session_state["email"] == admin_email and CFG.auth != "SUL":
-        setup_cfg = CFG.load_cfg_data()
-        for config in setup_cfg["config"]:
-            allow_reg = config["allow_reg"]
-            allow_uac = config["allow_uac"]
-            allow_ucp = config["allow_ucp"]
-            allow_uaa = config["allow_uaa"]
 
-        st.session_state["regCheck"] = allow_reg
+admin_email = CFIG.get_admin_email()
+if (
+    st.session_state["email"] == admin_email
+    and CFIG.load_config()["auth_setup_config"] != "SUL"
+):
+    setup_CFIG = CFIG.load_config()
+    if not setup_CFIG["config"]:
+        allow_reg = False
+        allow_uac = False
+        allow_ucp = False
+        allow_uaa = False
+    else:
+        config = setup_CFIG["config"]
+        allow_reg = config[0]
+        allow_uac = config[1]
+        allow_ucp = config[2]
+        allow_uaa = config[3]
 
-        if allow_reg == True:
-            ar_opposite = False
-        else:
-            ar_opposite = True
+    st.session_state["regCheck"] = allow_reg
 
-        if allow_uac == True:
-            uac_opposite = False
-        else:
-            uac_opposite = True
+    if allow_reg == True:
+        ar_opposite = False
+    else:
+        ar_opposite = True
 
-        if allow_ucp == True:
-            ucp_opposite = False
-        else:
-            ucp_opposite = True
+    if allow_uac == True:
+        uac_opposite = False
+    else:
+        uac_opposite = True
 
-        if allow_uaa == True:
-            uaa_opposite = False
-        else:
-            uaa_opposite = True
+    if allow_ucp == True:
+        ucp_opposite = False
+    else:
+        ucp_opposite = True
 
-        col1, col2 = st.columns(2)
+    if allow_uaa == True:
+        uaa_opposite = False
+    else:
+        uaa_opposite = True
 
-        with col1:
-            if CFG.auth == "MPBR":
-                st.checkbox(
-                    "Enable Public Registration",
-                    value=allow_reg,
-                    on_change=toggle_value,
-                    args=(ar_opposite, "allow_reg"),
-                )
-            else:
-                st.checkbox(
-                    "Enable Public Registration",
-                    value=allow_reg,
-                    on_change=toggle_value,
-                    args=(ar_opposite, "allow_reg"),
-                    disabled=True,
-                )
-            st.checkbox(
-                "Enable Users to Create Public Agents",
-                value=allow_uac,
-                on_change=toggle_value,
-                args=(uac_opposite, "allow_uac"),
-            )
+    col1, col2 = st.columns(2)
 
-        with col2:
+    with col1:
+        if setup_CFIG["auth_setup_config"] == "Multi-User Public Registration":
             st.checkbox(
-                "Enable Users To Create Private Agents",
-                value=allow_ucp,
+                "Enable Public Registration",
+                value=allow_reg,
                 on_change=toggle_value,
-                args=(ucp_opposite, "allow_ucp"),
+                args=(ar_opposite, 0),
             )
+        else:
             st.checkbox(
-                "Enable Users To Use Admin's Agents",
-                value=allow_uaa,
+                "Enable Public Registration",
+                value=allow_reg,
                 on_change=toggle_value,
-                args=(uaa_opposite, "allow_uaa"),
+                args=(ar_opposite, 0),
+                disabled=True,
             )
+        st.checkbox(
+            "Enable Users to Create Public Agents",
+            value=allow_uac,
+            on_change=toggle_value,
+            args=(uac_opposite, 1),
+        )
+
+    with col2:
+        st.checkbox(
+            "Enable Users To Create Private Agents",
+            value=allow_ucp,
+            on_change=toggle_value,
+            args=(ucp_opposite, 2),
+        )
+        st.checkbox(
+            "Enable Users To Use Admin's Agents",
+            value=allow_uaa,
+            on_change=toggle_value,
+            args=(uaa_opposite, 3),
+        )
 
     change_password_form()
-    if st.session_state["email"] == admin_email and CFG.auth != "SUL":
-        create_user_form()
-except:
+    create_user_form()
+else:
     st.write("You are not logged in, or login is not enabled.")
```

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.75b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Register.py` & `agixt-1.1.75b0/agixt/pages/Register.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import streamlit as st
 import auth_libs.Redirect as redir
 import bcrypt
+import logging
 from auth_libs.Cfig import Cfig
 from auth_libs.Users import load_users, save_user_data
 
 CFIG = Cfig()
 conf = CFIG.load_config()
 
 # Check if the user is logged in
 if st.session_state.get("logged_in"):
     # Redirect to the Profile page if so
     redir.nav_page("Profile")
 
 
-def registration_form():
+def registration_form(auth):
     user_data = load_users()
 
-    if conf["auth_setup"] == "True" and not conf["auth_setup_config"] == "No Login":
+    if auth and not conf["auth_setup_config"] == "No Login":
         st.write("Registration Form")
         email = st.text_input("Email")
         password = st.text_input("Password", type="password")
         confirm_password = st.text_input("Confirm Password", type="password")
 
         if st.button("Register"):
             if password == confirm_password:
@@ -43,14 +44,14 @@
                 st.error("Passwords do not match.")
 
         st.stop()
     else:
         st.write("Registration Is Not Enabled!")
 
 
-if "allow_reg" in CFIG.load_config():
-    if CFIG.load_config()["allow_reg"] == "True":
-        registration_form()
-    else:
-        st.write("Registration Is Not Enabled!")
+setup_CFIG = CFIG.load_config()
+config = setup_CFIG["config"]
+logging.info(config[0])
+if config[0]:
+    registration_form(auth=config[0])
 else:
-    st.write("Registration Not Enabled")
+    st.write("Registration Is Not Enabled!")
```

### Comparing `agixt-1.1.74b0/agixt/auth_libs/Users.py` & `agixt-1.1.75b0/agixt/auth_libs/Users.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import json
 import bcrypt
 import streamlit as st
 from auth_libs.Cfig import Cfig
 import auth_libs.Redirect as redir
 import logging
+import time
 
 CFIG = Cfig()
 
 USER_FILE = "user_data.json"
 
 
 def load_users():
@@ -23,23 +24,41 @@
         admin_email = st.text_input("Enter the admin email")
         admin_password = st.text_input("Enter the admin password", type="password")
         confirm_password = st.text_input("Confirm the admin password", type="password")
         if st.button("Create Admin Account"):
             if admin_password != confirm_password:
                 st.error("Password and confirm password do not match.")
             else:
-                admin_password_hash = bcrypt.hashpw(admin_password, bcrypt.gensalt())
+                admin_password_hash = str(
+                    bcrypt.hashpw(
+                        admin_password.encode("utf-8"), bcrypt.gensalt()
+                    ).decode()
+                )
                 admin_data = {
                     "email": admin_email,
                     "password_hash": admin_password_hash,
                     "admin": True,
                 }
                 user_data = {"users": [admin_data]}
                 save_user_data(user_data)
+                config = CFIG.load_config()
+                config["admin_email"] = admin_email
+                config["config"] = ["", "", "", ""]
+                # allow_reg = False
+                config["config"][0] = False
+                # allow_uac = False
+                config["config"][1] = False
+                # allow_ucp = False
+                config["config"][2] = False
+                # allow_uaa = False
+                config["config"][3] = False
+                CFIG.save_config(config)
                 st.success("Admin account created successfully!")
+                # Clear session state and redirect to the login page
+                st.session_state.clear()
                 st.experimental_rerun()
         st.stop()
     else:
         with open(USER_FILE, "r") as file:
             user_data = json.load(file)
     try:
         return user_data
@@ -96,16 +115,23 @@
 
 
 def check_auth_status():
     # Check if the user is logged in
     if (
         not st.session_state.get("logged_in")
         and os.path.exists("config.yaml")
-        and (CFIG.load_config()["auth_setup"] == "True")
+        and (CFIG.load_config()["auth_setup"] == True)
     ):
         # Redirect to the login page if not
-        # redir.nav_page("Login")
+        redir.nav_page("Login")
         logging.info("Not logged in")
     else:
-        if CFIG.load_config()["auth_setup"] == "True":
-            logging.info("Logged in")
-            # logout_button()
+        if CFIG.load_config()["auth_setup"] == True:
+            if (
+                st.session_state.get("logged_in")
+                and st.session_state.get("login_page") == True
+            ):
+                logging.info("Logged In!")
+                redir.nav_page("Profile")
+            logout_button()
+        elif st.session_state.get("login_page") == "Profile_Page":
+            redir.nav_page("Login")
```

### Comparing `agixt-1.1.74b0/agixt/chains/Smart Chat.json` & `agixt-1.1.75b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/commands/discord_commands.py` & `agixt-1.1.75b0/agixt/extensions/discord.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # pip install discord.py
-import discord
+import discord as dc
 from discord.ext import commands
-from Commands import Commands
-from Config import Config
+from Extensions import Extensions
 import logging
 
-CFG = Config()
 
-
-class discord_commands(Commands):
+class discord(Extensions):
     def __init__(
         self,
         DISCORD_API_KEY: str = "",
         DISCORD_COMMAND_PREFIX: str = "/AGiXT",
         **kwargs,
     ):
         self.DISCORD_API_KEY = DISCORD_API_KEY
@@ -24,15 +21,15 @@
                 "Delete Discord Message": self.delete_message,
                 "Create Discord Invite": self.create_invite,
                 "Get Discord Servers": self.get_servers,
                 "Get Discord Server Information": self.get_server_info,
             }
 
             try:
-                intents = discord.Intents.default()
+                intents = dc.Intents.default()
                 intents.typing = False
                 intents.presences = False
                 if self.DISCORD_API_KEY != "None" and self.DISCORD_API_KEY != "":
                     self.bot = commands.Bot(
                         command_prefix=self.DISCORD_COMMAND_PREFIX, intents=intents
                     )
                     self.bot.run(self.DISCORD_API_KEY)
```

### Comparing `agixt-1.1.74b0/agixt/commands/file_operations.py` & `agixt-1.1.75b0/agixt/extensions/file_system.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import os.path
-from typing import Generator, List
-from Commands import Commands
+from typing import List
+from Extensions import Extensions
+import os
+import subprocess
+import docker
+from docker.errors import ImageNotFound
+import logging
 
 
-class file_operations(Commands):
+class file_system(Extensions):
     def __init__(
         self,
         WORKING_DIRECTORY: str = "./WORKSPACE",
         WORKING_DIRECTORY_RESTRICTED: bool = True,
         **kwargs,
     ):
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
@@ -17,15 +22,99 @@
             os.makedirs(self.WORKING_DIRECTORY)
         self.commands = {
             "Read File": self.read_file,
             "Write to File": self.write_to_file,
             "Append to File": self.append_to_file,
             "Delete File": self.delete_file,
             "Search Files": self.search_files,
+            "Execute Python File": self.execute_python_file,
+            "Execute Shell": self.execute_shell,
         }
+        self.WORKING_DIRECTORY = WORKING_DIRECTORY
+
+    def execute_python_file(self, file: str):
+        logging.info(f"Executing file '{file}' in workspace '{self.WORKING_DIRECTORY}'")
+
+        if not file.endswith(".py"):
+            return "Error: Invalid file type. Only .py files are allowed."
+
+        file_path = os.path.join(self.WORKING_DIRECTORY, file)
+
+        if not os.path.isfile(file_path):
+            return f"Error: File '{file}' does not exist."
+
+        if self.we_are_running_in_a_docker_container():
+            result = subprocess.run(
+                f"python {file_path}", capture_output=True, encoding="utf8", shell=True
+            )
+            if result.returncode == 0:
+                return result.stdout
+            else:
+                return f"Error: {result.stderr}"
+
+        try:
+            client = docker.from_env()
+
+            image_name = "python:3.10"
+            try:
+                client.images.get(image_name)
+                logging.info(f"Image '{image_name}' found locally")
+            except ImageNotFound:
+                logging.info(
+                    f"Image '{image_name}' not found locally, pulling from Docker Hub"
+                )
+                low_level_client = docker.APIClient()
+                for line in low_level_client.pull(image_name, stream=True, decode=True):
+                    status = line.get("status")
+                    progress = line.get("progress")
+                    if status and progress:
+                        logging.info(f"{status}: {progress}")
+                    elif status:
+                        logging.info(status)
+
+            container = client.containers.run(
+                image_name,
+                f"python {file}",
+                volumes={
+                    os.path.abspath(self.WORKING_DIRECTORY): {
+                        "bind": "/workspace",
+                        "mode": "ro",
+                    }
+                },
+                working_dir="/workspace",
+                stderr=True,
+                stdout=True,
+                detach=True,
+            )
+
+            container.wait()
+            logs = container.logs().decode("utf-8")
+            container.remove()
+
+            return logs
+
+        except Exception as e:
+            return f"Error: {str(e)}"
+
+    def execute_shell(self, command_line: str) -> str:
+        current_dir = os.getcwd()
+        os.chdir(current_dir)
+        logging.info(
+            f"Executing command '{command_line}' in working directory '{os.getcwd()}'"
+        )
+        result = subprocess.run(command_line, capture_output=True, shell=True)
+        output = f"STDOUT:\n{result.stdout}\nSTDERR:\n{result.stderr}"
+
+        os.chdir(current_dir)
+
+        return output
+
+    @staticmethod
+    def we_are_running_in_a_docker_container() -> bool:
+        return os.path.exists("/.dockerenv")
 
     def safe_join(self, base: str, paths) -> str:
         if "/path/to/" in paths:
             paths = paths.replace("/path/to/", "")
         if str(self.WORKING_DIRECTORY_RESTRICTED).lower() == "true":
             new_path = os.path.normpath(os.path.join(base, *paths.split("/")))
             if not os.path.exists(new_path):
@@ -33,84 +122,60 @@
                     os.makedirs(new_path)
         else:
             new_path = os.path.normpath(os.path.join("/", *paths))
             if not os.path.exists(new_path):
                 os.makedirs(new_path)
         return new_path
 
-    @staticmethod
-    def split_file(
-        content: str, max_length: int = 4000, overlap: int = 0
-    ) -> Generator[str, None, None]:
-        start = 0
-        content_length = len(content)
-
-        while start < content_length:
-            end = start + max_length
-            if end + overlap < content_length:
-                chunk = content[start : end + overlap]
-            else:
-                chunk = content[start:content_length]
-            yield chunk
-            start += max_length - overlap
-
     def read_file(self, filename: str) -> str:
         try:
-            filepath = file_operations.safe_join(
-                self=self, base=self.WORKING_DIRECTORY, paths=filename
-            )
+            filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             with open(filepath, "r", encoding="utf-8") as f:
                 content = f.read()
             return content
         except Exception as e:
             return f"Error: {str(e)}"
 
     def write_to_file(self, filename: str, text: str) -> str:
         try:
-            filepath = file_operations.safe_join(
-                self=self, base=self.WORKING_DIRECTORY, paths=filename
-            )
+            filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             directory = os.path.dirname(filepath)
             if not os.path.exists(directory):
                 os.makedirs(directory)
             with open(filepath, "w", encoding="utf-8") as f:
                 f.write(text)
             return "File written to successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
     def append_to_file(self, filename: str, text: str) -> str:
         try:
-            filepath = file_operations.safe_join(
-                self=self, base=self.WORKING_DIRECTORY, paths=filename
-            )
+            filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             with open(filepath, "a") as f:
                 f.write(text)
             return "Text appended successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
     def delete_file(self, filename: str) -> str:
         try:
-            filepath = file_operations.safe_join(
-                self=self, base=self.WORKING_DIRECTORY, paths=filename
-            )
+            filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             os.remove(filepath)
             return "File deleted successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
     def search_files(self, directory: str) -> List[str]:
         found_files = []
 
         if directory in {"", "/"}:
             search_directory = self.WORKING_DIRECTORY
         else:
-            search_directory = file_operations.safe_join(
-                self=self, base=self.WORKING_DIRECTORY, paths=directory
+            search_directory = self.safe_join(
+                base=self.WORKING_DIRECTORY, paths=directory
             )
 
         for root, _, files in os.walk(search_directory):
             for file in files:
                 if file.startswith("."):
                     continue
                 relative_path = os.path.relpath(
```

### Comparing `agixt-1.1.74b0/agixt/commands/github.py` & `agixt-1.1.75b0/agixt/extensions/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import git
 from github import Github
-from Commands import Commands
+from Extensions import Extensions
 
 
-class github(Commands):
+class github(Extensions):
     def __init__(
         self,
         GITHUB_USERNAME: str = "",
         GITHUB_API_KEY: str = "",
         WORKING_DIRECTORY: str = "./WORKSPACE",
         **kwargs,
     ):
```

### Comparing `agixt-1.1.74b0/agixt/commands/google.py` & `agixt-1.1.75b0/agixt/extensions/google.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,19 @@
 from typing import Union, List
 import json
-from duckduckgo_search import DDGS
-from Commands import Commands
-import logging
+from Extensions import Extensions
 
-ddgs = DDGS()
 
-
-class google(Commands):
+class google(Extensions):
     def __init__(self, GOOGLE_API_KEY: str = "", **kwargs):
         self.GOOGLE_API_KEY = GOOGLE_API_KEY
-        self.commands = {
-            "Google Search": self.google_search,
-        }
         if self.GOOGLE_API_KEY:
-            self.commands["Google Official Search"] = self.google_official_search
-
-    @staticmethod
-    def google_search(query: str, num_results: int = 8) -> str:
-        search_results = []
-        if not query:
-            return json.dumps(search_results)
-        try:
-            results = ddgs.text(query)
-            if len(results) > num_results:
-                results = results[:num_results]
-        except:
-            logging.info(
-                "Duck Duck Go Search module broke. You may need to try to do `pip install duckduckgo_search --upgrade` to fix this."
-            )
-            results = None
-        if not results:
-            return json.dumps(search_results)
-        for j in results:
-            search_results.append(j)
-        return json.dumps(search_results, ensure_ascii=False, indent=4)
+            self.commands = {
+                "Google Search": self.google_official_search,
+            }
 
     def google_official_search(
         self, query: str, num_results: int = 8
     ) -> Union[str, List[str]]:
         from googleapiclient.discovery import build
         from googleapiclient.errors import HttpError
```

### Comparing `agixt-1.1.74b0/agixt/commands/image_generator.py` & `agixt-1.1.75b0/agixt/extensions/huggingface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,34 @@
+import requests
+import json
+import os
+from Extensions import Extensions
 from io import BytesIO
-import os.path
-import uuid
-from base64 import b64decode
-import openai
 import requests
 from PIL import Image
-from Commands import Commands
 import logging
 
 
-class image_generator(Commands):
+class huggingface(Extensions):
     def __init__(
         self,
         HUGGINGFACE_API_KEY: str = "",
-        OPENAI_API_KEY: str = "",
+        HUGGINGFACE_AUDIO_TO_TEXT_MODEL: str = "facebook/wav2vec2-large-960h-lv60-self",
         WORKING_DIRECTORY: str = "./WORKSPACE",
         **kwargs,
     ):
         self.HUGGINGFACE_API_KEY = HUGGINGFACE_API_KEY
-        self.OPENAI_API_KEY = OPENAI_API_KEY
+        self.HUGGINGFACE_AUDIO_TO_TEXT_MODEL = HUGGINGFACE_AUDIO_TO_TEXT_MODEL
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
-        if self.HUGGINGFACE_API_KEY or self.OPENAI_API_KEY:
-            self.commands = {"Generate Image": self.generate_image}
-
-    def generate_image(self, prompt: str) -> str:
-        filename = f"{str(uuid.uuid4())}.jpg"
-
-        if self.OPENAI_API_KEY:
-            return self.generate_image_with_dalle(prompt, filename)
-        elif self.HUGGINGFACE_API_KEY:
-            return self.generate_image_with_hf(prompt, filename)
-        else:
-            return "No Image Provider Set"
+        if self.HUGGINGFACE_API_KEY is not None:
+            self.commands = {
+                "Read Audio from File": self.read_audio_from_file,
+                "Read Audio": self.read_audio,
+                "Generate Image with Stable Diffusion": self.generate_image_with_hf,
+            }
 
     def generate_image_with_hf(self, prompt: str, filename: str) -> str:
         API_URL = (
             "https://api-inference.huggingface.co/models/CompVis/stable-diffusion-v1-4"
         )
         headers = {"Authorization": f"Bearer {self.HUGGINGFACE_API_TOKEN}"}
 
@@ -50,25 +43,32 @@
         image = Image.open(BytesIO(response.content))
         logging.info(f"Image Generated for prompt:{prompt}")
 
         image.save(os.path.join(self.WORKING_DIRECTORY, filename))
 
         return f"Saved to disk:{filename}"
 
-    def generate_image_with_dalle(self, prompt: str, filename: str) -> str:
-        openai.api_key = self.OPENAI_API_KEY
+    def read_audio_from_file(self, audio_path: str):
+        audio_path = os.path.join(self.WORKING_DIRECTORY, audio_path)
+        with open(audio_path, "rb") as audio_file:
+            audio = audio_file.read()
+        return self.read_audio(audio)
+
+    def read_audio(self, audio):
+        model = self.HUGGINGFACE_AUDIO_TO_TEXT_MODEL
+        api_url = f"https://api-inference.huggingface.co/models/{model}"
+        api_token = self.HUGGINGFACE_API_KEY
+        headers = {"Authorization": f"Bearer {api_token}"}
+
+        if api_token is None:
+            raise ValueError(
+                "You need to set your Hugging Face API token in the config file."
+            )
 
-        response = openai.Image.create(
-            prompt=prompt,
-            n=1,
-            size="256x256",
-            response_format="b64_json",
+        response = requests.post(
+            api_url,
+            headers=headers,
+            data=audio,
         )
 
-        logging.info(f"Image Generated for prompt:{prompt}")
-
-        image_data = b64decode(response["data"][0]["b64_json"])
-
-        with open(f"{self.WORKING_DIRECTORY}/{filename}", mode="wb") as png:
-            png.write(image_data)
-
-        return f"Saved to disk:{filename}"
+        text = json.loads(response.content.decode("utf-8"))["text"]
+        return "The audio says: " + text
```

### Comparing `agixt-1.1.74b0/agixt/commands/microsoft_365_email.py` & `agixt-1.1.75b0/agixt/extensions/microsoft_365.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
-from Commands import Commands
+from Extensions import Extensions
 
 
-class microsoft_365_email(Commands):
+class microsoft_365(Extensions):
     def __init__(
         self,
         MICROSOFT_365_CLIENT_ID: str = "",
         MICROSOFT_365_CLIENT_SECRET: str = "",
         MICROSOFT_365_REDIRECT_URI: str = "",
         **kwargs,
     ):
```

### Comparing `agixt-1.1.74b0/agixt/commands/sendgrid_email.py` & `agixt-1.1.75b0/agixt/extensions/sendgrid_email.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 from sendgrid import SendGridAPIClient
 from sendgrid.helpers.mail import Mail
-from Commands import Commands
+from Extensions import Extensions
 
 
-class sendgrid_email(Commands):
+class sendgrid_email(Extensions):
     def __init__(self, SENDGRID_API_KEY: str = "", SENDGRID_EMAIL: str = "", **kwargs):
         self.SENDGRID_API_KEY = SENDGRID_API_KEY
         self.SENDGRID_EMAIL = SENDGRID_EMAIL
         if self.SENDGRID_API_KEY:
             self.commands = {"Send Email with Sendgrid": self.send_email}
 
     def send_email(self, to_email: str, subject: str, content: str) -> List[str]:
```

### Comparing `agixt-1.1.74b0/agixt/commands/twitter.py` & `agixt-1.1.75b0/agixt/extensions/twitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tweepy
-from Commands import Commands
+from Extensions import Extensions
 import logging
 
 
-class twitter(Commands):
+class twitter(Extensions):
     def __init__(
         self,
         TW_CONSUMER_KEY: str = "",
         TW_CONSUMER_SECRET: str = "",
         TW_ACCESS_TOKEN: str = "",
         TW_ACCESS_TOKEN_SECRET: str = "",
         **kwargs
```

### Comparing `agixt-1.1.74b0/agixt/commands/web_playwright.py` & `agixt-1.1.75b0/agixt/extensions/web_playwright.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Union
 from requests.compat import urljoin
 from bs4 import BeautifulSoup
-from Commands import Commands
+from Extensions import Extensions
 from playwright.sync_api import sync_playwright
 
 
-class web_playwright(Commands):
+class web_playwright(Extensions):
     def __init__(self, **kwargs):
         self.commands = {
             "Scrape Text with Playwright": self.scrape_text_with_playwright,
             "Scrape Links with Playwright": self.scrape_links_with_playwright,
         }
 
     def scrape_text_with_playwright(self, url: str) -> str:
```

### Comparing `agixt-1.1.74b0/agixt/components/agent_selector.py` & `agixt-1.1.75b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/example.ipynb` & `agixt-1.1.75b0/agixt/example.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981595604727398%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from AGiXT import AGiXT, Prompts\\n'), (5, "*

 * *            "'Prompts().add_prompt(\\n'), (19, ')')], delete: [19, 5, 0]}}, 3: {'source': {insert: "*

 * *            "[(0, 'from AGiXT import AGiXT, Prompts\\n'), (4, 'cp = Prompts()\\n'), (24, "*

 * *            "'chain.add_chain(chain_name)\\n')], delete: [24, 4, 0]}}, 5: {'source': {insert: "*

 * *            "[(14, ')')], delete: [14]}}, 7: {'source': {insert: [(22, ')')], delete: [22]}}, 9: "*

 * *            "{'source': {insert: [(22 […]*

```diff
@@ -40,34 +40,34 @@
                         "Collaboration also involves encouraging feedback and input from all stakeholders. This includes not only team members but also clients and end-users. By soliciting feedback from these groups, software projects can be tailored to meet their specific needs and requirements. This also ensures that the final product is user-friendly and meets the needs of the intended audience.\n",
                         "\n",
                         "In conclusion, collaboration is critical for the success of software products and the growth of the industry. It starts with communication, teamwork, and feedback, and requires a culture of inclusiveness and mutual respect. At our software company, we strive to foster collaboration at every level of our organization to deliver the best possible software solutions to our clients and end-users. We believe that by working together, we can achieve success and innovation in the software industry.\n"
                     ]
                 }
             ],
             "source": [
-                "from AGiXT import AGiXT, CustomPrompt\n",
+                "from AGiXT import AGiXT, Prompts\n",
                 "\n",
                 "agent_name = \"gpt4free\"\n",
                 "ai = AGiXT(agent_name)\n",
                 "\n",
-                "CustomPrompt().add_prompt(\n",
+                "Prompts().add_prompt(\n",
                 "    prompt_name=\"Write a blog post\",\n",
                 "    prompt=\"Write a blog post for the {industry} instustry. For context, here is a description of my business: {business_description}\",\n",
                 ")\n",
                 "\n",
                 "response = ai.run(\n",
                 "    prompt=\"Write a blog post\",\n",
                 "    industry=\"software\",\n",
                 "    business_description=\"I am a software company that makes software for software companies.\",\n",
                 "    # Other available options:\n",
                 "    # context_results = 5,  # Number of memories to inject into context\n",
                 "    # websearch = False,   # Use websearch to find context\n",
                 "    # websearch_depth = 3,  # Number of websearch results to use\n",
                 "    # learn_file: str = \"/path/to/file/to/learn/from.txt\",  # File to learn from\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -87,19 +87,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from AGiXT import AGiXT, CustomPrompt\n",
+                "from AGiXT import AGiXT, Prompts\n",
                 "from Chain import Chain\n",
                 "\n",
                 "chain = Chain()\n",
-                "cp = CustomPrompt()\n",
+                "cp = Prompts()\n",
                 "\n",
                 "# Set your agent, we'll use gpt4free as the default for now unless you have an agent set up.\n",
                 "agent_name = \"gpt4free\"\n",
                 "# Name the chain, we'll call this one \"Blog Writer\" because we're super original and creative alll the time.\n",
                 "chain_name = \"Blog Writer\"\n",
                 "\n",
                 "# Now we can define some custom variables that well want to use in our custom prompts\n",
@@ -111,15 +111,15 @@
                 "business_description = \"We're a artificial intelligence software development company.\"\n",
                 "website = \"https://devxt.com\"\n",
                 "\n",
                 "# Set up your ai agent\n",
                 "ai = AGiXT(agent_name)\n",
                 "\n",
                 "# Create the new chain to start adding steps to.\n",
-                "chain.add_chain(chain_name)"
+                "chain.add_chain(chain_name)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -144,15 +144,15 @@
                 ")\n",
                 "\n",
                 "cp.add_prompt(\n",
                 "    prompt_name=\"Good email subject for blog post\",\n",
                 "    prompt=\"\"\"\n",
                 "    I need a good email subject for this blog post, I'm going to send it out to customers, so I need something that is attractive. Please respond only with the subject line.\n",
                 "    Blog post: {blog_post}\"\"\",\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -185,15 +185,15 @@
                 "    agent_name=agent_name,\n",
                 "    step_number=2,\n",
                 "    prompt_type=\"Prompt\",\n",
                 "    prompt={\n",
                 "        \"prompt_name\": \"Good email subject for blog post\",\n",
                 "        \"blog_post\": \"{STEP1}\",  # <- Intentionally not an f-string, we want to use the response from the previous step in the chain.\n",
                 "    },\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -226,15 +226,15 @@
                 "    prompt_type=\"Command\",\n",
                 "    prompt={\n",
                 "        \"command_name\": \"send_email\",\n",
                 "        \"email\": f\"your@customers-email.com\",\n",
                 "        \"subject\": \"{STEP2}\",\n",
                 "        \"body\": \"{STEP1}\",\n",
                 "    },\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -243,15 +243,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "chain.run_chain(chain_name)\n"
+                "chain.run_chain(chain_name)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `agixt-1.1.74b0/agixt/model-prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.75b0/agixt/prompts/Instruction.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 You have the following resources:
 1. Internet access for searches and information gathering.
 2. Long Term memory management.
 3. GPT-3.5 powered Agents for delegation of simple tasks.
 4. File output.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
-
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
     "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 
 Your task: {task}
```

### Comparing `agixt-1.1.74b0/agixt/model-prompts/gpt-4/instruct.txt` & `agixt-1.1.75b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 You have the following resources:
 1. Internet access for searches and information gathering.
 2. Long Term memory management.
 3. GPT-3.5 powered Agents for delegation of simple tasks.
 4. File output.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
-
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
     "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 
 Your task: {task}
```

### Comparing `agixt-1.1.74b0/agixt/model-prompts/starchat/instruct.txt` & `agixt-1.1.75b0/agixt/prompts/starchat/instruct.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 <|system|>
 {COMMANDS}
 You have the following constraints:
 ~500 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
 If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
 No user assistance.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
-
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
-    "response": "Your response to the task",
+    "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 <|end|><|user|>Your task: {task}<|end|>\n<|assistant|>
```

### Comparing `agixt-1.1.74b0/agixt/model-prompts/vicuna/instruct.txt` & `agixt-1.1.75b0/agixt/prompts/vicuna/instruct.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 ###Human:
 {AGENT_NAME}, follow constraints:
 {COMMANDS}
 500-word memory limit. Save important info.
 Recall by considering similar events.
 No user assistance.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
-
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
-    "response": "Your response to the task",
+    "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 
 Task: {task}
 ###Assistant:
```

### Comparing `agixt-1.1.74b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.75b0/agixt/pages/0-Agent_Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import streamlit as st
 from Config import Config
 from Agent import Agent
-from Commands import Commands
+from Extensions import Extensions
 from Embedding import get_embedding_providers
 from provider import get_provider_options
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 
@@ -135,15 +135,15 @@
                     # Check if the user value exists before saving the setting
                     if user_val:
                         rendered_settings[key] = user_val
 
             return rendered_settings
 
         st.subheader("Extension Settings")
-        extension_setting_keys = Commands(agent_config).get_extension_settings()
+        extension_setting_keys = Extensions(agent_config).get_extension_settings()
         extension_settings = render_extension_settings(
             extension_setting_keys, agent_settings
         )
 
         # Update the extension settings in the agent_settings directly
         agent_settings.update(extension_settings)
 
@@ -196,15 +196,15 @@
                 for custom_setting in st.session_state.custom_settings_list
                 if custom_setting and ":" in custom_setting
             }
         )
 
         st.subheader("Agent Commands")
         # Fetch the available commands using the `Commands` class
-        available_commands = Commands(agent_config).get_available_commands()
+        available_commands = Extensions(agent_config).get_available_commands()
 
         # Save the existing command state to prevent duplication
         existing_command_states = {
             command["friendly_name"]: command["enabled"]
             for command in available_commands
         }
```

### Comparing `agixt-1.1.74b0/agixt/pages/1-Learning.py` & `agixt-1.1.75b0/agixt/pages/1-Learning.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,24 +12,32 @@
 # Initialize session state for stop events and agent status if not exist
 if "agent_status" not in st.session_state:
     st.session_state.agent_status = {}
 
 if agent_name:
     st.markdown("## Learn from a file")
     learn_file_upload = st.file_uploader(
-        "Upload a file for the agent to learn from.",
+        "Upload a file for the agent to learn from.", accept_multiple_files=True
     )
     if learn_file_upload is not None:
-        learn_file_path = os.path.join("data", "uploaded_files", learn_file_upload.name)
-        if not os.path.exists(os.path.dirname(learn_file_path)):
-            os.makedirs(os.path.dirname(learn_file_path))
-        with open(learn_file_path, "wb") as f:
-            f.write(learn_file_upload.getbuffer())
-        agent.memories.read_file(learn_file_path)
-        st.success(f"Agent '{agent_name}' has learned from the uploaded file.")
+        for learn_file_upload in learn_file_upload.copy():
+            learn_file_path = os.path.join(
+                "data", "uploaded_files", learn_file_upload.name
+            )
+            if not os.path.exists(os.path.dirname(learn_file_path)):
+                os.makedirs(os.path.dirname(learn_file_path))
+            with open(learn_file_path, "wb") as f:
+                f.write(learn_file_upload.getbuffer())
+            agent.memories.mem_read_file(learn_file_path)
+            st.success(
+                "Agent '"
+                + agent_name
+                + "' has learned from file: "
+                + learn_file_upload.name
+            )
 
     st.markdown("## Learn from a URL")
     learn_url = st.text_input("Enter a URL for the agent to learn from..")
     if st.button("Learn from URL"):
         if learn_url:
             _, _ = agent.memories.read_website(learn_url)
             st.success(f"Agent '{agent_name}' has learned from the URL.")
```

### Comparing `agixt-1.1.74b0/agixt/pages/2-Chat.py` & `agixt-1.1.75b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/pages/3-Instructions.py` & `agixt-1.1.75b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/pages/4-Tasks.py` & `agixt-1.1.75b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/pages/5-Chains.py` & `agixt-1.1.75b0/agixt/pages/3-Chains.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import streamlit as st
 import auth_libs.Redirect as redir
 from Config import Config
 from Chain import Chain
-from Commands import Commands
+from Extensions import Extensions
 from Agent import Agent
-from CustomPrompt import CustomPrompt
+from Prompts import Prompts
+import logging
 from auth_libs.Users import check_auth_status
+from components.agent_selector import agent_selector
 
 check_auth_status()
 
+agent_name, agent = agent_selector()
 CFG = Config()
 
 st.header("Manage Chains")
 st.markdown("### Predefined Injection Variables")
 st.markdown(
     """
     Any of these variables can be used in command arguments or prompt arguments to inject data into the prompt. These can also be used inside of any Custom Prompt.
@@ -20,40 +23,71 @@
 - `{context}` will cause the current context from memory to be injected.
 - `{date}` will cause the current date and timestamp to be injected.
 - `{COMMANDS}` will cause the available commands list to be injected and for automatic commands execution from the agent based on its suggestions.
 - `{command_list}` will cause the available commands list to be injected, but will not execute any commands the AI chooses. Useful on validation steps.
 - `{STEPx}` will cause the step `x` response from a chain to be injected. For example, `{STEP1}` will inject the first step's response in a chain.
 """
 )
-chain_name = st.text_input("Chain Name")
+
 chain_action = st.selectbox("Action", ["Create Chain", "Delete Chain", "Run Chain"])
+if chain_action == "Create Chain":
+    chain_name = st.text_input("Chain Name")
+else:
+    chain_name = st.selectbox("Chains", Chain().get_chains())
 
 if st.button("Perform Action"):
     if chain_name:
         if chain_action == "Create Chain":
-            Chain().add_chain(chain_name)
+            Chain().add_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' created.")
             st.experimental_rerun()
         elif chain_action == "Delete Chain":
-            Chain().delete_chain(chain_name)
+            Chain().delete_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' deleted.")
             st.experimental_rerun()
         elif chain_action == "Run Chain":
-            Chain().run_chain(chain_name)
+            Chain().run_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' executed.")
     else:
         st.error("Chain name is required.")
 
-st.header("Manage Chain Steps")
+st.header("Manage Chain Steps & View Responses")
 
 chain_names = Chain().get_chains()
 selected_chain_name = st.selectbox("Select Chain", [""] + chain_names)
 
 if selected_chain_name:
-    chain = Chain().get_steps(selected_chain_name)
+    try:
+        chain = Chain().get_steps(chain_name=selected_chain_name)
+    except:
+        st.write(selected_chain_name + " Responses: ")
+        try:
+            if "_responses" in selected_chain_name:
+                chain_commands_executed = Chain().get_step_response(
+                    chain_name=selected_chain_name.replace("_responses", "")
+                )
+            else:
+                chain_commands_executed = False
+            chain_response = Chain().get_step_response(
+                chain_name=selected_chain_name,
+            )
+            if chain_response and chain_commands_executed:
+                for exec in chain_commands_executed["steps"]:
+                    logging.info("----------exec: " + str(exec["step"]))
+                    logging.info("----------Chain_Response " + str(chain_response["1"]))
+                    st.write(exec)
+                    st.write(chain_response[str(exec["step"])])
+            elif chain_response:
+                st.write(chain_response)
+            else:
+                raise ValueError("End of responses!", "None Found!")
+        except ValueError as err:
+            st.write(err.args)
+            loop = False
+        st.stop()
 
     st.subheader(f"Selected Chain: {selected_chain_name}")
 
     def modify_step(step):
         step_number = step["step"]
         agent_name = step["agent_name"]
         prompt_type = step["prompt_type"]
@@ -80,50 +114,50 @@
             index=["", "Command", "Prompt"].index(prompt_type),
             key=f"prompt_type_{step_number}",
         )
 
         if modify_prompt_type == "Command":
             available_commands = [
                 cmd["friendly_name"]
-                for cmd in Commands(agent_config).get_enabled_commands()
+                for cmd in Extensions(agent_config).get_enabled_commands()
             ]
             command_name = st.selectbox(
                 "Select Command",
                 [""] + available_commands,
                 key=f"command_name_{step_number}",
                 index=available_commands.index(prompt.get("command_name", "")) + 1
                 if "command_name" in prompt
                 else 0,
             )
 
             if command_name:
-                command_args = Commands(agent_config).get_command_args(command_name)
+                command_args = Extensions(agent_config).get_command_args(command_name)
                 formatted_command_args = ", ".join(
                     [
                         f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
                         for arg in command_args
                         if arg != "context"
                         and arg != "command_list"
                         and arg != "COMMANDS"
                     ]
                 )
                 modify_prompt = f"{command_name}({formatted_command_args})"
         elif modify_prompt_type == "Prompt":
-            available_prompts = CustomPrompt().get_prompts()
+            available_prompts = Prompts().get_prompts()
             modify_prompt_name = st.selectbox(
                 "Select Custom Prompt",
                 [""] + available_prompts,
                 key=f"prompt_name_{step_number}",
                 index=available_prompts.index(prompt.get("prompt_name", "")) + 1
                 if "prompt_name" in prompt
                 else 0,
             )
 
             if modify_prompt_name:
-                prompt_args = CustomPrompt().get_prompt_args(modify_prompt_name)
+                prompt_args = Prompts().get_prompt_args(modify_prompt_name)
                 formatted_prompt_args = ", ".join(
                     [
                         f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
                         for arg in prompt_args
                         if arg != "context"
                         and arg != "command_list"
                         and arg != "COMMANDS"
@@ -175,42 +209,42 @@
         key="add_step_prompt_type",
     )
 
     if prompt_type == "Command":
         agent_config = Agent(agent_name).agent_config
         available_commands = [
             cmd["friendly_name"]
-            for cmd in Commands(agent_config).get_enabled_commands()
+            for cmd in Extensions(agent_config).get_enabled_commands()
         ]
         command_name = st.selectbox(
             "Select Command",
             [""] + available_commands,
             key="add_step_command_name",
         )
 
         if command_name:
-            command_args = Commands(agent_config).get_command_args(command_name)
+            command_args = Extensions(agent_config).get_command_args(command_name)
             formatted_command_args = ", ".join(
                 [
                     f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
                     for arg in command_args
                     if arg != "context" and arg != "command_list" and arg != "COMMANDS"
                 ]
             )
             prompt = f"{command_name}({formatted_command_args})"
     elif prompt_type == "Prompt":
-        available_prompts = CustomPrompt().get_prompts()
+        available_prompts = Prompts().get_prompts()
         prompt_name = st.selectbox(
             "Select Custom Prompt",
             [""] + available_prompts,
             key="add_step_prompt_name",
         )
 
         if prompt_name:
-            prompt_args = CustomPrompt().get_prompt_args(prompt_name)
+            prompt_args = Prompts().get_prompt_args(prompt_name)
             formatted_prompt_args = ", ".join(
                 [
                     f"{arg}: {st.text_input(arg, key=f'add_step_{arg}')} "
                     for arg in prompt_args
                     if arg != "context" and arg != "command_list" and arg != "COMMANDS"
                 ]
             )
```

### Comparing `agixt-1.1.74b0/agixt/pages/6-Custom_Prompts.py` & `agixt-1.1.75b0/agixt/pages/2-Prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import streamlit as st
-from CustomPrompt import CustomPrompt
+from Prompts import Prompts
 from auth_libs.Users import check_auth_status
 
 check_auth_status()
 
-st.header("Manage Custom Prompts")
+st.header("Manage Prompts")
 st.markdown("### Usage Instructions")
 st.markdown(
     """
 To create dynamic prompts that can have user inputs, you can use curly braces `{}` in your prompt content. 
 Anything between the curly braces will be considered as an input field. For example:
 
 ```python
@@ -25,15 +25,15 @@
 - `{date}` will cause the current date and timestamp to be injected.
 - `{COMMANDS}` will cause the available commands list to be injected and for automatic commands execution from the agent based on its suggestions.
 - `{command_list}` will cause the available commands list to be injected, but will not execute any commands the AI chooses. Useful on validation steps.
 - `{STEPx}` will cause the step `x` response from a chain to be injected. For example, `{STEP1}` will inject the first step's response in a chain.
 """
 )
 
-custom_prompt = CustomPrompt()
+custom_prompt = Prompts()
 prompt_list = custom_prompt.get_prompts()
 
 if st.checkbox("Add New Prompt"):
     action = "Add Prompt"
     prompt_name = st.text_input("Prompt Name")
     prompt_content = st.text_area("Prompt Content", height=300)
 else:
```

### Comparing `agixt-1.1.74b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.75b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/prompts/Instruction.txt` & `agixt-1.1.75b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 You have the following resources:
 1. Internet access for searches and information gathering.
 2. Long Term memory management.
 3. GPT-3.5 powered Agents for delegation of simple tasks.
 4. File output.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
-
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
     "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 
 Your task: {task}
```

### Comparing `agixt-1.1.74b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.75b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.75b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.75b0/agixt/prompts/ValidationFailed.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 {command_args}
 
 We received the following output:
 {command_output}
 
 The validation for running the command has failed.  The goal of this validation is to assist in completing the task.  Review the command output and correct the issue. Respond with the corrected command to usage to get the proper intended output.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
+If there are no commands, respond only with empty Json like {}. If there are commands to use from the Task Response, format them as follows in your response:
 
+```
 {
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
-}
+}
+```
```

### Comparing `agixt-1.1.74b0/agixt/prompts/instruct.txt` & `agixt-1.1.75b0/agixt/prompts/Execution.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-{COMMANDS}
-You have the following constraints:
-~500 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
-If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
-No user assistance.
+{context}
+
+You are an AI who performs one task based on the following objective: {objective}.
+Your role is to do anything asked of you with precision. You have the following constraints:
+1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
+2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
+3. No user assistance.
+
+Take into account these previously completed tasks from context.
 
-RESPOND IN THE FOLLOWING JSON FORMAT ONLY! THERE ARE SERIOUS CONSEQUENCES FOR BREAKING THIS RULE!
+Your task: {task}
+
+{COMMANDS}
 
+RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
+```JSON
 {
-    "response": "Your response to the task",
+    "response": "Your response to the task.",
     "commands": {
         "command_name": {
             "arg1": "val1",
             "arg2": "val2"
         },
         "command_name2": {
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
+```
 
-Your task: {task}
+Response:
```

### Comparing `agixt-1.1.74b0/agixt/provider/__init__.py` & `agixt-1.1.75b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/azure.py` & `agixt-1.1.75b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/bing.py` & `agixt-1.1.75b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/chatgpt.py` & `agixt-1.1.75b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/claude.py` & `agixt-1.1.75b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/fastchat.py` & `agixt-1.1.75b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/gpt4all.py` & `agixt-1.1.75b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/gpt4free.py` & `agixt-1.1.75b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.75b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/huggingchat.py` & `agixt-1.1.75b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/huggingface.py` & `agixt-1.1.75b0/agixt/provider/huggingface.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,18 @@
             "inputs": prompt,
             "max_tokens": int(self.MAX_TOKENS),
             "temperature": float(self.AI_TEMPERATURE),
         }
         for _ in range(num_retries):
             try:
                 response = requests.post(
-                    f"{self.HUGGINGFACE_API_URL}/models/{self.AI_MODEL}",
+                    self.HUGGINGFACE_API_URL,
                     headers=headers,
                     json=payload,
                 )
                 response.raise_for_status()
                 return response.json()[0]["generated_text"]
-            except:
+            except requests.exceptions.RequestException as e:
+                logging.error(e)
                 logging.info("Rate limit exceeded. Retrying after 20 seconds.")
                 time.sleep(20)
                 continue
```

### Comparing `agixt-1.1.74b0/agixt/provider/kobold.py` & `agixt-1.1.75b0/agixt/provider/kobold.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 
     def instruct(self, prompt, tokens: int = 0):
         try:
             max_tokens = int(self.MAX_TOKENS - tokens)
         except:
             max_tokens = 2000
         response = requests.post(
-            f"{self.AI_PROVIDER_URI}/generate",
+            f"{self.AI_PROVIDER_URI}/api/v1/generate",
             json={
                 "prompt": prompt,
-                "max_length": max_tokens,
+                "max_context_length": max_tokens,
+                "max_length": 200,
                 "temperature": float(self.AI_TEMPERATURE),
             },
         )
         try:
             return response.json()["results"][0]["text"].replace("\n", "\n")
         except:
             return response.json()["detail"][0]["msg"].replace("\n", "\n")
```

### Comparing `agixt-1.1.74b0/agixt/provider/llamacpp.py` & `agixt-1.1.75b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/llamacppapi.py` & `agixt-1.1.75b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/oobabooga.py` & `agixt-1.1.75b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/openai.py` & `agixt-1.1.75b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/palm.py` & `agixt-1.1.75b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/provider/transformer.py` & `agixt-1.1.75b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/agixt/starchat.sh` & `agixt-1.1.75b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.74b0/docs/README.md` & `agixt-1.1.75b0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,34 +63,34 @@
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart with Docker
 Clone the repository and run the AGiXT Streamlit Web App.
 ```
-git clone https://github.com/Josh-XT/AGiXT
-docker compose --profile streamlit up
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+docker compose streamlit up
 ```
 
 - Web Interface http://localhost:8501
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
 
 ### Alternative Docker Compose Profiles
 
 Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
 ```
-docker compose --profile all up
+docker compose all up
 ```
 
 ### Development using docker
 ```
-git clone https://github.com/Josh-XT/AGiXT
-docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
```

### Comparing `agixt-1.1.74b0/pyproject.toml` & `agixt-1.1.75b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.74-beta"
+version = "v1.1.75-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.74b0/PKG-INFO` & `agixt-1.1.75b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.74b0
+Version: 1.1.75b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
@@ -125,34 +125,34 @@
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart with Docker
 Clone the repository and run the AGiXT Streamlit Web App.
 ```
-git clone https://github.com/Josh-XT/AGiXT
-docker compose --profile streamlit up
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+docker compose streamlit up
 ```
 
 - Web Interface http://localhost:8501
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
 
 ### Alternative Docker Compose Profiles
 
 Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
 ```
-docker compose --profile all up
+docker compose all up
 ```
 
 ### Development using docker
 ```
-git clone https://github.com/Josh-XT/AGiXT
-docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
```


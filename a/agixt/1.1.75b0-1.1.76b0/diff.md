# Comparing `tmp/agixt-1.1.75b0.tar.gz` & `tmp/agixt-1.1.76b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.75b0.tar", max compression
+gzip compressed data, was "agixt-1.1.76b0.tar", max compression
```

## Comparing `agixt-1.1.75b0.tar` & `agixt-1.1.76b0.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0     1087 2023-05-31 00:15:01.082069 agixt-1.1.75b0/LICENSE
--rw-r--r--   0        0        0    19540 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    14146 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Agent.py
--rw-r--r--   0        0        0     7187 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Config.py
--rw-r--r--   0        0        0     7045 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6462 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-05-31 00:15:01.082069 agixt-1.1.75b0/agixt/Main.py
--rw-r--r--   0        0        0     9750 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7128 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12677 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1566 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/example.ipynb
--rw-r--r--   0        0        0     5982 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      854 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1168 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1164 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6605 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1829 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2036 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      533 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2451 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      616 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4198 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1887 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0      995 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      309 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1163 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2275 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     1970 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13354 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2779 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     2887 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1571 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      424 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      308 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3100 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-05-31 00:15:01.086069 agixt-1.1.75b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0    13585 2023-05-31 00:15:01.090069 agixt-1.1.75b0/docs/README.md
--rw-r--r--   0        0        0     2806 2023-05-31 00:15:01.098069 agixt-1.1.75b0/pyproject.toml
--rw-r--r--   0        0        0    16387 1970-01-01 00:00:00.000000 agixt-1.1.75b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-31 23:06:10.137556 agixt-1.1.76b0/LICENSE
+-rw-r--r--   0        0        0    19819 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    14146 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Agent.py
+-rw-r--r--   0        0        0     7187 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Config.py
+-rw-r--r--   0        0        0     5904 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6462 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Main.py
+-rw-r--r--   0        0        0     9680 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7128 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12677 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1566 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     5982 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      854 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1168 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1164 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6605 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1829 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2036 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      533 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2451 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      616 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4198 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1887 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0      995 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      309 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1163 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2275 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2011 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13354 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2779 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     2887 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1571 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      424 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      308 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0     8553 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/test-memory.ipynb
+-rw-r--r--   0        0        0    13585 2023-05-31 23:06:10.145556 agixt-1.1.76b0/docs/README.md
+-rw-r--r--   0        0        0     2838 2023-05-31 23:06:10.157557 agixt-1.1.76b0/pyproject.toml
+-rw-r--r--   0        0        0    16440 1970-01-01 00:00:00.000000 agixt-1.1.76b0/PKG-INFO
```

### Comparing `agixt-1.1.75b0/LICENSE` & `agixt-1.1.76b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/AGiXT.py` & `agixt-1.1.76b0/agixt/AGiXT.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import spacy
 from datetime import datetime
 from Agent import Agent
 from Prompts import Prompts
 from extensions.searxng import searxng
 from urllib.parse import urlparse
 import logging
+from concurrent.futures import Future
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
         self.agent_commands = self.agent.get_commands_string()
@@ -140,15 +141,21 @@
                 asyncio.set_event_loop(loop)
                 loop.run_until_complete(
                     self.websearch_agent(task=task, depth=websearch_depth)
                 )
             else:
                 self.websearch_agent(task=task, depth=websearch_depth)
         try:
-            self.response = self.agent.instruct(formatted_prompt, tokens=tokens)
+            # Workaround for non-threaded providers
+            run_response = self.agent.instruct(formatted_prompt, tokens=tokens)
+            self.response = (
+                run_response.result()
+                if isinstance(run_response, Future)
+                else run_response
+            )
         except Exception as e:
             logging.info(f"Error: {e}")
             logging.info(f"PROMPT CONTENT: {formatted_prompt}")
             logging.info(f"TOKENS: {tokens}")
             self.failures += 1
             if self.failures == 5:
                 self.failures == 0
@@ -191,15 +198,15 @@
                     )
             except:
                 return_response = self.response
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
-                self.agent.memories.store_result(task, self.response)
+                asyncio.run(self.agent.memories.store_result(task, self.response))
             except:
                 pass
             self.agent.log_interaction("USER", task)
             self.agent.log_interaction(self.agent_name, self.response)
         return self.response
 
     def smart_instruct(
@@ -392,15 +399,15 @@
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
                         if command_name in [
                             available_command["friendly_name"],
                             available_command["name"],
                         ]:
-                            command_name = available_command["name"]
+                            command_name = available_command["friendly_name"]
                             try:
                                 # Check if the command is a valid command in the self.avent.available_commands list
                                 command_output = self.agent.execute(
                                     command_name, command_args
                                 )
                                 logging.info("Running Command Execution Validation...")
                                 validate_command = self.run(
```

### Comparing `agixt-1.1.75b0/agixt/Agent.py` & `agixt-1.1.76b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Chain.py` & `agixt-1.1.76b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Config.py` & `agixt-1.1.76b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Embedding.py` & `agixt-1.1.76b0/agixt/Embedding.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import requests
 import inspect
-import openai
 from chromadb.utils import embedding_functions
 from chromadb.api.types import Documents, EmbeddingFunction, Embeddings
+from semantic_kernel.connectors.ai.hugging_face import HuggingFaceTextEmbedding
+from semantic_kernel.connectors.ai.open_ai import (
+    AzureTextEmbedding,
+    OpenAITextEmbedding,
+)
 import logging
 
 
 class GooglePalmEmbeddingFunction(EmbeddingFunction):
     """To use this EmbeddingFunction, you must have the google.generativeai Python package installed and have a PaLM API key."""
 
     def __init__(self, api_key: str, model_name: str = "models/embedding-gecko-001"):
@@ -73,124 +77,89 @@
         ).json()
         if "data" in response:
             if "embedding" in response["data"]:
                 return response["data"]["embedding"]
         return {}
 
 
-class AzureEmbeddingFunction(EmbeddingFunction):
-    def __init__(
-        self,
-        api_key: str,
-        model_name: str = "text-embedding-ada-002",
-        deployment_id: str = "",
-        AZURE_OPENAI_ENDPOINT: str = "https://api.openai.com",
-    ):
-        openai.api_type = "azure"
-        openai.api_type = "azure"
-        openai.api_base = AZURE_OPENAI_ENDPOINT
-        openai.api_version = "2023-05-15"
-        openai.api_key = api_key
-        if api_key is not None:
-            self.api_key = api_key
-        else:
-            raise ValueError("Please update your Agent settings with an AZURE_API_KEY.")
-        if deployment_id is not None:
-            self.deployment_id = deployment_id
-        else:
-            raise ValueError("Please update your Agent settings with an AZURE_API_KEY.")
-        self._client = openai.Embedding(engine=model_name)
-        self._model_name = model_name
-
-    def __call__(self, texts: Documents) -> Embeddings:
-        # replace newlines, which can negatively affect performance.
-        texts = [t.replace("\n", " ") for t in texts]
-
-        # Call the OpenAI Embedding API
-        embeddings = self._client.create(
-            input=texts,
-            engine=self._model_name,
-        )["data"]
-
-        # Sort resulting embeddings by index
-        sorted_embeddings = sorted(embeddings, key=lambda e: e["index"])
-
-        # Return just the embeddings
-        return [result["embedding"] for result in sorted_embeddings]
-
-
 class Embedding:
     def __init__(self, AGENT_CONFIG=None):
-        # We need to take the embedder string and then return the correct embedder
-        # We also need to return the correct chunk size
         self.AGENT_CONFIG = AGENT_CONFIG
+
+    async def get_embedder(self):
         try:
             embedder = self.AGENT_CONFIG["settings"]["embedder"]
-            self.embed, self.chunk_size = self.__getattribute__(embedder)()
+            embed, chunk_size = await self.__getattribute__(embedder)()
         except:
-            self.embed, self.chunk_size = self.default()
+            embed, chunk_size = await self.default()
             logging.info("Embedder not found, using default embedder")
+        return embed, chunk_size
+
+    async def embed_text(self, text):
+        embed, chunk_size = await self.get_embedder()
+        return await embed(text)
 
-    def default(self):
+    async def default(self):
         chunk_size = 128
-        embed = embedding_functions.SentenceTransformerEmbeddingFunction(
-            model_name="all-mpnet-base-v2"
-        )
+        embed = HuggingFaceTextEmbedding(
+            model_name="all-mpnet-base-v2", log=logging
+        ).generate_embeddings_async
         return embed, chunk_size
 
-    def large_local(self):
+    async def large_local(self):
         chunk_size = 500
-        embed = embedding_functions.SentenceTransformerEmbeddingFunction(
-            model_name="gtr-t5-large"
-        )
+        embed = HuggingFaceTextEmbedding(
+            model_name="gtr-t5-large", log=logging
+        ).generate_embeddings_async
         return embed, chunk_size
 
-    def azure(self):
+    async def azure(self):
         chunk_size = 1000
-        embed = AzureEmbeddingFunction(
+        embed = AzureTextEmbedding(
+            deployment_name=self.AGENT_CONFIG["settings"]["AZURE_DEPLOYMENT_NAME"],
+            endpoint=self.AGENT_CONFIG["settings"]["AZURE_OPENAI_ENDPOINT"],
             api_key=self.AGENT_CONFIG["settings"]["AZURE_API_KEY"],
-            deployment_id=self.AGENT_CONFIG["settings"]["AZURE_EMBEDDER_DEPLOYMENT_ID"],
-            AZURE_OPENAI_ENDPOINT=self.AGENT_CONFIG["settings"][
-                "AZURE_OPENAI_ENDPOINT"
-            ],
-        )
+            logger=logging,
+        ).generate_embeddings_async
         return embed, chunk_size
 
-    def openai(self):
+    async def openai(self):
         chunk_size = 1000
-        embed = embedding_functions.OpenAIEmbeddingFunction(
+        embed = OpenAITextEmbedding(
+            model_id="text-embedding-ada-002",
             api_key=self.AGENT_CONFIG["settings"]["OPENAI_API_KEY"],
-        )
+            log=logging,
+        ).generate_embeddings_async
         return embed, chunk_size
 
-    def google_palm(self):
+    async def google_palm(self):
         chunk_size = 1000
         embed = GooglePalmEmbeddingFunction(
             api_key=self.AGENT_CONFIG["settings"]["GOOGLE_API_KEY"],
         )
         return embed, chunk_size
 
-    def google_vertex(self):
+    async def google_vertex(self):
         chunk_size = 1000
         embed = GoogleVertexEmbeddingFunction(
             api_key=self.AGENT_CONFIG["settings"]["GOOGLE_API_KEY"],
             project_id=self.AGENT_CONFIG["settings"]["GOOGLE_PROJECT_ID"],
         )
         return embed, chunk_size
 
-    def cohere(self):
+    async def cohere(self):
         chunk_size = 500
         embed = embedding_functions.CohereEmbeddingFunction(
             api_key=self.AGENT_CONFIG["settings"]["COHERE_API_KEY"],
         )
         return embed, chunk_size
 
-    def llamacpp(self):
+    async def llamacpp(self):
         chunk_size = 250
-        embed = embedding_functions.LlamaCppEmbeddingFunction(
+        embed = LlamacppEmbeddingFunction(
             model_name=self.AGENT_CONFIG["settings"]["EMBEDDING_URI"],
         )
         return embed, chunk_size
 
 
 def get_embedding_providers():
     return [
```

### Comparing `agixt-1.1.75b0/agixt/Extensions.py` & `agixt-1.1.76b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Main.py` & `agixt-1.1.76b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Memories.py` & `agixt-1.1.76b0/agixt/Memories.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import chromadb
 from typing import List
 import spacy
 import os
 from hashlib import sha256
 from Embedding import Embedding
 from datetime import datetime
 from collections import Counter
 import pandas as pd
 import docx2txt
 import pdfplumber
 from playwright.async_api import async_playwright
+from semantic_kernel.connectors.memory.chroma import ChromaMemoryStore
+from semantic_kernel.memory.memory_record import MemoryRecord
+from chromadb.config import Settings
 from bs4 import BeautifulSoup
 import logging
 import asyncio
 import sys
 
 if sys.platform == "win32":
     asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
@@ -22,131 +24,132 @@
 class Memories:
     def __init__(self, agent_name: str = "AGiXT", agent_config=None):
         self.agent_name = agent_name
         self.agent_config = agent_config
         self.chroma_client = None
         self.collection = None
         self.nlp = None
-        self.chroma_persist_dir = f"agents/{self.agent_name}/memories"
-        if not os.path.exists(self.chroma_persist_dir):
-            os.makedirs(self.chroma_persist_dir)
+        self.chunk_size = 128
+        memories_dir = os.path.join(os.getcwd(), "agents", self.agent_name, "memories")
+        self.chroma_client = ChromaMemoryStore(
+            persist_directory=memories_dir,
+            client_settings=Settings(
+                chroma_db_impl="chromadb.db.duckdb.PersistentDuckDB",
+                persist_directory=memories_dir,
+                anonymized_telemetry=False,
+            ),
+        )
 
     def load_spacy_model(self):
         if not self.nlp:
             try:
                 self.nlp = spacy.load("en_core_web_sm")
             except:
                 spacy.cli.download("en_core_web_sm")
                 self.nlp = spacy.load("en_core_web_sm")
         self.nlp.max_length = 99999999999999999999999
 
-    def initialize_chroma_client(self):
+    async def get_embedder(self):
+        embedder, chunk_size = await Embedding(
+            AGENT_CONFIG=self.agent_config
+        ).get_embedder()
+        return embedder, chunk_size
+
+    async def get_collection(self):
         try:
-            return chromadb.Client(
-                settings=chromadb.config.Settings(
-                    chroma_db_impl="duckdb+parquet",
-                    persist_directory=self.chroma_persist_dir,
-                    anonymized_telemetry=False,
-                )
+            memories_exist = await self.chroma_client.does_collection_exist_async(
+                "memories"
             )
+            if not memories_exist:
+                await self.chroma_client.create_collection_async(
+                    collection_name="memories"
+                )
+                memories = await self.chroma_client.get_collection_async(
+                    collection_name="memories"
+                )
+            else:
+                memories = await self.chroma_client.get_collection_async(
+                    collection_name="memories"
+                )
+            return memories
         except Exception as e:
             raise RuntimeError(f"Unable to initialize chroma client: {e}")
 
-    def get_or_create_collection(self):
-        if not self.chroma_client:
-            self.chroma_client = self.initialize_chroma_client()
-        embedder = Embedding(self.agent_config)
-        self.embedding_function = embedder.embed
-        self.chunk_size = embedder.chunk_size
-        try:
-            return self.chroma_client.get_collection(
-                name="memories", embedding_function=self.embedding_function
-            )
-        except ValueError:
-            logging.info(f"Memories for {self.agent_name} do not exist. Creating...")
-            return self.chroma_client.create_collection(
-                name="memories", embedding_function=self.embedding_function
-            )
-
-    def generate_id(self, content: str, timestamp: str):
-        return sha256((content + timestamp).encode()).hexdigest()
+    async def store_memory(
+        self, content: str, description: str = None, external_source_name: str = None
+    ):
+        embedder, chunk_size = await self.get_embedder()
+        collection = await self.get_collection()
+        record = MemoryRecord(
+            is_reference=False,
+            id=sha256((content + datetime.now().isoformat()).encode()).hexdigest(),
+            text=content,
+            timestamp=datetime.now().isoformat(),
+            description=description,
+            external_source_name=external_source_name,  # URL or File path
+            embedding=await embedder(content),
+        )
 
-    def store_memory(self, id: str, content: str, metadatas: dict):
-        if not self.chroma_client:
-            self.chroma_client = self.initialize_chroma_client()
-            self.collection = self.get_or_create_collection()
         try:
-            self.collection.add(
-                ids=id,
-                documents=content,
-                metadatas=metadatas,
+            await self.chroma_client.upsert_async(
+                collection_name="memories",
+                record=record,
             )
+            self.chroma_client._client.persist()
         except Exception as e:
             logging.info(f"Failed to store memory: {e}")
 
-    def store_result(self, task_name: str, result: str):
-        if not self.chroma_client:
-            self.chroma_client = self.initialize_chroma_client()
-            self.collection = self.get_or_create_collection()
+    async def store_result(
+        self, task_name: str, result: str, external_source_name: str = None
+    ):
         if result:
-            timestamp = datetime.now()  # current time as datetime object
             if not isinstance(result, str):
                 result = str(result)
-            chunks = self.chunk_content(result, task_name)
+            chunks = await self.chunk_content(result, task_name)
             for chunk in chunks:
-                result_id = self.generate_id(chunk, timestamp.isoformat())
-                self.store_memory(
-                    result_id,
-                    chunk,
-                    {
-                        "task": task_name,
-                        "result": chunk,
-                        "timestamp": timestamp.isoformat(),
-                    },
+                await self.store_memory(
+                    content=chunk,
+                    description=task_name,
+                    external_source_name=external_source_name,
                 )
 
-    def context_agent(self, query: str, top_results_num: int) -> List[str]:
-        if not self.chroma_client:
-            self.chroma_client = self.initialize_chroma_client()
-            self.collection = self.get_or_create_collection()
-        count = self.collection.count()
-        if count == 0:
+    async def context_agent(self, query: str, top_results_num: int) -> List[str]:
+        embedder, chunk_size = await self.get_embedder()
+        collection = await self.get_collection()
+        if collection == None:
             return []
-        results = self.collection.query(
-            query_texts=query,
-            n_results=min(top_results_num, count),
-            include=["metadatas"],
-        )
-        sorted_results = sorted(
-            results["metadatas"][0],
-            key=lambda item: datetime.strptime(
-                item.get("timestamp") or "1970-01-01T00:00:00.000",
-                "%Y-%m-%dT%H:%M:%S.%f",
-            ),
-            reverse=True,
-        )
-        # TODO: Before sending results, ask AI if each chunk it is relevant to the task-
-        #   so that we're only injecting relevant memories into the context.
-        # This will ensure we aren't injecting memories that aren't relevant.
-        # Need to research to find out how to do this locally instead of sending more shots to the AI.
-        context = [item["result"] for item in sorted_results]
-        trimmed_context = self.trim_context(context)
+        try:
+            results = await self.chroma_client.get_nearest_matches_async(
+                collection_name="memories",
+                embedding=await embedder(query),
+                limit=top_results_num,
+                min_relevance_score=0.1,
+            )
+        except Exception as e:
+            logging.info(f"Failed to get context: {e}")
+            return []
+        # Each result is as results._text
+        context = []
+        for memory, score in results:
+            context.append(memory._text)
+        trimmed_context = await self.trim_context(context)
         logging.info(f"CONTEXT: {trimmed_context}")
         context_str = "\n".join(trimmed_context)
         response = f"Context: {context_str}\n\n"
         return response
 
-    def trim_context(self, context: List[str]) -> List[str]:
+    async def trim_context(self, context: List[str]) -> List[str]:
+        embedder, chunk_size = await self.get_embedder()
         if not self.nlp:
             self.load_spacy_model()
         trimmed_context = []
         total_tokens = 0
         for item in context:
             item_tokens = len(self.nlp(item))
-            if total_tokens + item_tokens <= self.chunk_size:
+            if total_tokens + item_tokens <= chunk_size:
                 trimmed_context.append(item)
                 total_tokens += item_tokens
             else:
                 break
         return trimmed_context
 
     def get_keywords(self, query: str):
@@ -161,27 +164,30 @@
 
     def score_chunk(self, chunk: str, keywords: set):
         """Score a chunk based on the number of query keywords it contains."""
         chunk_counter = Counter(chunk.split())
         score = sum(chunk_counter[keyword] for keyword in keywords)
         return score
 
-    def chunk_content(self, content: str, query: str, overlap: int = 2) -> List[str]:
+    async def chunk_content(
+        self, content: str, query: str, overlap: int = 2
+    ) -> List[str]:
+        embedder, chunk_size = await self.get_embedder()
         if not self.nlp:
             self.load_spacy_model()
         doc = self.nlp(content)
         sentences = list(doc.sents)
         content_chunks = []
         chunk = []
         chunk_len = 0
         keywords = self.get_keywords(query)
 
         for i, sentence in enumerate(sentences):
             sentence_tokens = len(sentence)
-            if chunk_len + sentence_tokens > self.chunk_size and chunk:
+            if chunk_len + sentence_tokens > chunk_size and chunk:
                 chunk_text = " ".join(token.text for token in chunk)
                 content_chunks.append(
                     (self.score_chunk(chunk_text, keywords), chunk_text)
                 )
                 chunk = list(sentences[i - overlap : i]) if i - overlap >= 0 else []
                 chunk_len = sum(len(s) for s in chunk)
             chunk.extend(sentence)
@@ -191,15 +197,15 @@
             chunk_text = " ".join(token.text for token in chunk)
             content_chunks.append((self.score_chunk(chunk_text, keywords), chunk_text))
 
         # Sort the chunks by their score in descending order before returning them
         content_chunks.sort(key=lambda x: x[0], reverse=True)
         return [chunk_text for score, chunk_text in content_chunks]
 
-    def mem_read_file(self, file_path: str):
+    async def mem_read_file(self, file_path: str):
         try:
             # If file extension is pdf, convert to text
             if file_path.endswith(".pdf"):
                 with pdfplumber.open(file_path) as pdf:
                     content = "\n".join([page.extract_text() for page in pdf.pages])
             # If file extension is xls, convert to csv
             elif file_path.endswith(".xls") or file_path.endswith(".xlsx"):
@@ -208,15 +214,15 @@
             elif file_path.endswith(".doc") or file_path.endswith(".docx"):
                 content = docx2txt.process(file_path)
             # TODO: If file is an image, classify it in text.
             # Otherwise just read the file
             else:
                 with open(file_path, "r") as f:
                     content = f.read()
-            self.store_result(task_name=file_path, result=content)
+            await self.store_result(task_name=file_path, result=content)
             return True
         except:
             return False
 
     async def read_website(self, url):
         try:
             async with async_playwright() as p:
@@ -235,11 +241,11 @@
                     link_list.append((title, href))
 
                 await browser.close()
                 soup = BeautifulSoup(content, "html.parser")
                 text_content = soup.get_text()
                 text_content = " ".join(text_content.split())
                 if text_content:
-                    self.store_result(url, text_content)
+                    await self.store_result(url, text_content)
                 return text_content, link_list
         except:
             return None, None
```

### Comparing `agixt-1.1.75b0/agixt/Prompts.py` & `agixt-1.1.76b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/Tasks.py` & `agixt-1.1.76b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/app.py` & `agixt-1.1.76b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.76b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.76b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/auth_libs/Users.py` & `agixt-1.1.76b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/chains/Smart Chat.json` & `agixt-1.1.76b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/chains/Test_Commands.json` & `agixt-1.1.76b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/components/agent_selector.py` & `agixt-1.1.76b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/example.ipynb` & `agixt-1.1.76b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.76b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/briantts.py` & `agixt-1.1.76b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/dalle.py` & `agixt-1.1.76b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/discord.py` & `agixt-1.1.76b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.76b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/file_system.py` & `agixt-1.1.76b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/github.py` & `agixt-1.1.76b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/google.py` & `agixt-1.1.76b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/gtts.py` & `agixt-1.1.76b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/huggingface.py` & `agixt-1.1.76b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/macostts.py` & `agixt-1.1.76b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.76b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/searxng.py` & `agixt-1.1.76b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.76b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/twitter.py` & `agixt-1.1.76b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/extensions/web_playwright.py` & `agixt-1.1.76b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.76b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/1-Learning.py` & `agixt-1.1.76b0/agixt/pages/1-Learning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import streamlit as st
 import os
+import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 
 agent_name, agent = agent_selector()
 
@@ -23,27 +24,27 @@
             learn_file_path = os.path.join(
                 "data", "uploaded_files", learn_file_upload.name
             )
             if not os.path.exists(os.path.dirname(learn_file_path)):
                 os.makedirs(os.path.dirname(learn_file_path))
             with open(learn_file_path, "wb") as f:
                 f.write(learn_file_upload.getbuffer())
-            agent.memories.mem_read_file(learn_file_path)
+            asyncio.run(agent.memories.mem_read_file(learn_file_path))
             st.success(
                 "Agent '"
                 + agent_name
                 + "' has learned from file: "
                 + learn_file_upload.name
             )
 
     st.markdown("## Learn from a URL")
     learn_url = st.text_input("Enter a URL for the agent to learn from..")
     if st.button("Learn from URL"):
         if learn_url:
-            _, _ = agent.memories.read_website(learn_url)
+            _, _ = asyncio.run(agent.memories.read_website(learn_url))
             st.success(f"Agent '{agent_name}' has learned from the URL.")
     st.markdown("## Wipe Agent Memory")
     st.markdown(
         "The agent can simply learn too much undesired information at times. If you're having an issue with the context being injected from memory with your agent, try wiping the memory."
     )
     if st.button("Wipe agent memory"):
         agent.wipe_agent_memories(agent_name)
```

### Comparing `agixt-1.1.75b0/agixt/pages/2-Prompts.py` & `agixt-1.1.76b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/3-Chains.py` & `agixt-1.1.76b0/agixt/pages/3-Chains.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/4-Chat.py` & `agixt-1.1.76b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/5-Instructions.py` & `agixt-1.1.76b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/6-Tasks.py` & `agixt-1.1.76b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/Login.py` & `agixt-1.1.76b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/Profile.py` & `agixt-1.1.76b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/pages/Register.py` & `agixt-1.1.76b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.76b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/Execution.txt` & `agixt-1.1.76b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/Instruction.txt` & `agixt-1.1.76b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.76b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.76b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.76b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.76b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.76b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/instruct.txt` & `agixt-1.1.76b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.76b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.76b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/__init__.py` & `agixt-1.1.76b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/azure.py` & `agixt-1.1.76b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/bing.py` & `agixt-1.1.76b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/chatgpt.py` & `agixt-1.1.76b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/claude.py` & `agixt-1.1.76b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/fastchat.py` & `agixt-1.1.76b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/gpt4all.py` & `agixt-1.1.76b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/gpt4free.py` & `agixt-1.1.76b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.76b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/huggingchat.py` & `agixt-1.1.76b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/huggingface.py` & `agixt-1.1.76b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/kobold.py` & `agixt-1.1.76b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/llamacpp.py` & `agixt-1.1.76b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/llamacppapi.py` & `agixt-1.1.76b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/oobabooga.py` & `agixt-1.1.76b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/openai.py` & `agixt-1.1.76b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/palm.py` & `agixt-1.1.76b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/provider/transformer.py` & `agixt-1.1.76b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/starchat.sh` & `agixt-1.1.76b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/agixt/test-commands.ipynb` & `agixt-1.1.76b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/docs/README.md` & `agixt-1.1.76b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.75b0/pyproject.toml` & `agixt-1.1.76b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.75-beta"
+version = "v1.1.76-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
@@ -83,14 +83,15 @@
   { markers = "platform_machine == 'x86_64' and sys_platform == 'linux'", version = "^2.0.1", source = "pytorch.org"},
   { markers = "platform_machine == 'aarch64' or sys_platform == 'win32'", version = "^2.0.1", source = "PyPI"}
 ]
 transformers = { version = "^4.29.2", extras = ["accelerate"] }
 sentence-transformers = "^2.2.2"
 llama-cpp-python = "^0.1.55"
 nomic = "^1.1.6"
+semantic-kernel = "^0.2.9.dev0"
 
 [tool.poetry.group.gpt4free]
 optional = true
 
 [tool.poetry.group.gpt4free.dependencies]
 gpt4free = { git = "https://github.com/xtekky/gpt4free.git", rev = "6598265e2bf46ce1054736cd64db9ff42a358331" }
```

### Comparing `agixt-1.1.75b0/PKG-INFO` & `agixt-1.1.76b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.75b0
+Version: 1.1.76b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
@@ -43,14 +43,15 @@
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: playwright (>=1.33.0,<2.0.0)
 Requires-Dist: protobuf (==3.20.*)
 Requires-Dist: random-password-generator (>=2.2.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: revChatGPT (>=5.2.0,<6.0.0)
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
+Requires-Dist: semantic-kernel (>=0.2.9.dev0,<0.3.0)
 Requires-Dist: sendgrid (>=6.10.0,<7.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: streamlit (>=1.22.0,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; platform_machine == "aarch64" or sys_platform == "win32"
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; platform_machine == "x86_64" and sys_platform == "linux"
 Requires-Dist: transformers[accelerate] (>=4.29.2,<5.0.0)
```


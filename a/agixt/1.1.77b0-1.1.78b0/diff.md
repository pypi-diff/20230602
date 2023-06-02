# Comparing `tmp/agixt-1.1.77b0.tar.gz` & `tmp/agixt-1.1.78b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.77b0.tar", max compression
+gzip compressed data, was "agixt-1.1.78b0.tar", max compression
```

## Comparing `agixt-1.1.77b0.tar` & `agixt-1.1.78b0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     1087 2023-06-02 09:44:01.759448 agixt-1.1.77b0/LICENSE
--rw-r--r--   0        0        0    19641 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    24299 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Agent.py
--rw-r--r--   0        0        0     7330 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Config.py
--rw-r--r--   0        0        0     5904 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6474 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Main.py
--rw-r--r--   0        0        0     9471 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7099 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12707 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0      410 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0     1566 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1893 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2035 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13398 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2909 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     3006 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1616 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0     8553 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/test-memory.ipynb
--rw-r--r--   0        0        0    13215 2023-06-02 09:44:01.767448 agixt-1.1.77b0/docs/README.md
--rw-r--r--   0        0        0     2838 2023-06-02 09:44:01.779448 agixt-1.1.77b0/pyproject.toml
--rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.77b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-02 13:25:13.010806 agixt-1.1.78b0/LICENSE
+-rw-r--r--   0        0        0    19685 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    24299 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Agent.py
+-rw-r--r--   0        0        0     7330 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Config.py
+-rw-r--r--   0        0        0     5904 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6474 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Main.py
+-rw-r--r--   0        0        0     9471 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7099 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12707 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0      410 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0     1566 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-02 13:25:13.010806 agixt-1.1.78b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2035 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13398 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2909 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     3006 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1616 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0     8553 2023-06-02 13:25:13.014806 agixt-1.1.78b0/agixt/test-memory.ipynb
+-rw-r--r--   0        0        0    13215 2023-06-02 13:25:13.018806 agixt-1.1.78b0/docs/README.md
+-rw-r--r--   0        0        0     2838 2023-06-02 13:25:13.026806 agixt-1.1.78b0/pyproject.toml
+-rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.78b0/PKG-INFO
```

### Comparing `agixt-1.1.77b0/LICENSE` & `agixt-1.1.78b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/AGiXT.py` & `agixt-1.1.78b0/agixt/AGiXT.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,14 +501,16 @@
         for result in results:
             search_string = result.lstrip("0123456789. ")
             try:
                 searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
             except:
                 searx_server = ""
             try:
-                links = searxng(SEARXNG_INSTANCE_URL=searx_server).search(search_string)
+                links = await searxng(SEARXNG_INSTANCE_URL=searx_server).search(
+                    search_string
+                )
                 if len(links) > depth:
                     links = links[:depth]
             except:
                 links = None
             if links is not None:
                 await resursive_browsing(task, links)
```

### Comparing `agixt-1.1.77b0/agixt/Agent.py` & `agixt-1.1.78b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Chain.py` & `agixt-1.1.78b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Config.py` & `agixt-1.1.78b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Embedding.py` & `agixt-1.1.78b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Extensions.py` & `agixt-1.1.78b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Main.py` & `agixt-1.1.78b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Memories.py` & `agixt-1.1.78b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Prompts.py` & `agixt-1.1.78b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/Tasks.py` & `agixt-1.1.78b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/app.py` & `agixt-1.1.78b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.78b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.78b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/auth_libs/Users.py` & `agixt-1.1.78b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/chains/Smart Chat.json` & `agixt-1.1.78b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/chains/Test_Commands.json` & `agixt-1.1.78b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/components/agent_selector.py` & `agixt-1.1.78b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/example.ipynb` & `agixt-1.1.78b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.78b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/briantts.py` & `agixt-1.1.78b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/dalle.py` & `agixt-1.1.78b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/discord.py` & `agixt-1.1.78b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.78b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/file_system.py` & `agixt-1.1.78b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/github.py` & `agixt-1.1.78b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/google.py` & `agixt-1.1.78b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/gtts.py` & `agixt-1.1.78b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/huggingface.py` & `agixt-1.1.78b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/macostts.py` & `agixt-1.1.78b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.78b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/searxng.py` & `agixt-1.1.78b0/agixt/extensions/searxng.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
             summaries = [
                 result["title"] + " - " + result["url"] for result in results["results"]
             ]
             return summaries
         except:
             # The SearXNG server is down or refusing connection, so we will use the default one.
             self.SEARXNG_ENDPOINT = "https://search.us.projectsegfau.lt/search"
-            return self.search(query)
+            return await self.search(query)
```

### Comparing `agixt-1.1.77b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.78b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/twitter.py` & `agixt-1.1.78b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/extensions/web_playwright.py` & `agixt-1.1.78b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.78b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/1-Learning.py` & `agixt-1.1.78b0/agixt/pages/1-Learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/2-Prompts.py` & `agixt-1.1.78b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/3-Chains.py` & `agixt-1.1.78b0/agixt/pages/3-Chains.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/4-Chat.py` & `agixt-1.1.78b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/5-Instructions.py` & `agixt-1.1.78b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/6-Tasks.py` & `agixt-1.1.78b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/Login.py` & `agixt-1.1.78b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/Profile.py` & `agixt-1.1.78b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/pages/Register.py` & `agixt-1.1.78b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.78b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/Execution.txt` & `agixt-1.1.78b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/Instruction.txt` & `agixt-1.1.78b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.78b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.78b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.78b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.78b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.78b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/instruct.txt` & `agixt-1.1.78b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.78b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.78b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/__init__.py` & `agixt-1.1.78b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/azure.py` & `agixt-1.1.78b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/bing.py` & `agixt-1.1.78b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/chatgpt.py` & `agixt-1.1.78b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/claude.py` & `agixt-1.1.78b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/fastchat.py` & `agixt-1.1.78b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/gpt4all.py` & `agixt-1.1.78b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/gpt4free.py` & `agixt-1.1.78b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.78b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/huggingchat.py` & `agixt-1.1.78b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/huggingface.py` & `agixt-1.1.78b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/kobold.py` & `agixt-1.1.78b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/llamacpp.py` & `agixt-1.1.78b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/llamacppapi.py` & `agixt-1.1.78b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/oobabooga.py` & `agixt-1.1.78b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/openai.py` & `agixt-1.1.78b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/palm.py` & `agixt-1.1.78b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/runpod.py` & `agixt-1.1.78b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/provider/transformer.py` & `agixt-1.1.78b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/starchat.sh` & `agixt-1.1.78b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/test-commands.ipynb` & `agixt-1.1.78b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/agixt/test-memory.ipynb` & `agixt-1.1.78b0/agixt/test-memory.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/docs/README.md` & `agixt-1.1.78b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.77b0/pyproject.toml` & `agixt-1.1.78b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.77-beta"
+version = "v1.1.78-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.77b0/PKG-INFO` & `agixt-1.1.78b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.77b0
+Version: 1.1.78b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
```


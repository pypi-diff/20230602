# Comparing `tmp/agixt-1.1.76b0.tar.gz` & `tmp/agixt-1.1.77b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.76b0.tar", max compression
+gzip compressed data, was "agixt-1.1.77b0.tar", max compression
```

## Comparing `agixt-1.1.76b0.tar` & `agixt-1.1.77b0.tar`

### file list

```diff
@@ -1,107 +1,111 @@
--rw-r--r--   0        0        0     1087 2023-05-31 23:06:10.137556 agixt-1.1.76b0/LICENSE
--rw-r--r--   0        0        0    19819 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    14146 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Agent.py
--rw-r--r--   0        0        0     7187 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Config.py
--rw-r--r--   0        0        0     5904 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6462 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Main.py
--rw-r--r--   0        0        0     9680 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7128 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12677 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1566 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/example.ipynb
--rw-r--r--   0        0        0     5982 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      854 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1168 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-05-31 23:06:10.137556 agixt-1.1.76b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1164 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6605 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1829 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2036 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      533 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2451 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      616 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4198 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1887 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0      995 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      309 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1163 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2275 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2011 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13354 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2779 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     2887 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1571 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      424 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      308 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0     8553 2023-05-31 23:06:10.141556 agixt-1.1.76b0/agixt/test-memory.ipynb
--rw-r--r--   0        0        0    13585 2023-05-31 23:06:10.145556 agixt-1.1.76b0/docs/README.md
--rw-r--r--   0        0        0     2838 2023-05-31 23:06:10.157557 agixt-1.1.76b0/pyproject.toml
--rw-r--r--   0        0        0    16440 1970-01-01 00:00:00.000000 agixt-1.1.76b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-02 09:44:01.759448 agixt-1.1.77b0/LICENSE
+-rw-r--r--   0        0        0    19641 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    24299 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Agent.py
+-rw-r--r--   0        0        0     7330 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Config.py
+-rw-r--r--   0        0        0     5904 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6474 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Main.py
+-rw-r--r--   0        0        0     9471 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7099 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12707 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0      410 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0     1566 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1893 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2035 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13398 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2909 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     3006 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1616 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-06-02 09:44:01.763448 agixt-1.1.77b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0     8553 2023-06-02 09:44:01.767448 agixt-1.1.77b0/agixt/test-memory.ipynb
+-rw-r--r--   0        0        0    13215 2023-06-02 09:44:01.767448 agixt-1.1.77b0/docs/README.md
+-rw-r--r--   0        0        0     2838 2023-06-02 09:44:01.779448 agixt-1.1.77b0/pyproject.toml
+-rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.77b0/PKG-INFO
```

### Comparing `agixt-1.1.76b0/LICENSE` & `agixt-1.1.77b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/AGiXT.py` & `agixt-1.1.77b0/agixt/AGiXT.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 import os
-import asyncio
 import regex
 import json
 import time
 import spacy
 from datetime import datetime
 from Agent import Agent
 from Prompts import Prompts
@@ -53,36 +52,37 @@
         try:
             with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
                 responses = json.load(f)
             return responses.get(str(step_number))
         except:
             return ""
 
-    def format_prompt(
+    async def format_prompt(
         self,
         task: str = "",
         top_results: int = 5,
         prompt="",
         chain_name="",
         step_number=0,
+        memories=None,
         **kwargs,
     ):
         cp = Prompts()
         if prompt == "":
             prompt = task
         else:
             try:
                 prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
             except:
                 prompt = prompt
         if top_results == 0:
             context = "None"
         else:
             try:
-                context = self.agent.memories.context_agent(
+                context = await memories.context_agent(
                     query=task, top_results_num=top_results
                 )
             except:
                 context = "None."
         command_list = self.agent.get_commands_string()
         formatted_prompt = self.custom_format(
             prompt,
@@ -105,49 +105,43 @@
             )
         if not self.nlp:
             self.load_spacy_model()
         tokens = len(self.nlp(formatted_prompt))
         logging.info(f"FORMATTED PROMPT: {formatted_prompt}")
         return formatted_prompt, prompt, tokens
 
-    def run(
+    async def run(
         self,
         task: str = "",
         prompt: str = "",
         context_results: int = 5,
         websearch: bool = False,
         websearch_depth: int = 3,
-        async_exec: bool = False,
         learn_file: str = "",
         chain_name: str = "",
         step_number: int = 0,
         **kwargs,
     ):
         logging.info(f"KWARGS: {kwargs}")
+        memories = self.agent.get_memories()
         if learn_file != "":
-            learning_file = self.agent.memories.mem_read_file(file_path=learn_file)
+            learning_file = await memories.mem_read_file(file_path=learn_file)
             if learning_file == False:
                 return "Failed to read file."
-        formatted_prompt, unformatted_prompt, tokens = self.format_prompt(
+        formatted_prompt, unformatted_prompt, tokens = await self.format_prompt(
             task=task,
             top_results=context_results,
             prompt=prompt,
             chain_name=chain_name,
             step_number=step_number,
+            memories=memories,
             **kwargs,
         )
         if websearch:
-            if async_exec:
-                loop = asyncio.new_event_loop()
-                asyncio.set_event_loop(loop)
-                loop.run_until_complete(
-                    self.websearch_agent(task=task, depth=websearch_depth)
-                )
-            else:
-                self.websearch_agent(task=task, depth=websearch_depth)
+            await self.websearch_agent(task=task, depth=websearch_depth)
         try:
             # Workaround for non-threaded providers
             run_response = self.agent.instruct(formatted_prompt, tokens=tokens)
             self.response = (
                 run_response.result()
                 if isinstance(run_response, Future)
                 else run_response
@@ -161,26 +155,25 @@
                 self.failures == 0
                 logging.info("Failed to get a response 5 times in a row.")
                 return None
             logging.info(f"Retrying in 10 seconds...")
             time.sleep(10)
             if context_results > 0:
                 context_results = context_results - 1
-            self.response = self.run(
+            self.response = await self.run(
                 task=task,
                 prompt=prompt,
                 context_results=context_results,
-                async_exec=async_exec,
                 **kwargs,
             )
 
         # Handle commands if the prompt contains the {COMMANDS} placeholder
         # We handle command injection that DOESN'T allow command execution by using {command_list} in the prompt
         if "{COMMANDS}" in unformatted_prompt:
-            execution_response = self.execution_agent(
+            execution_response = await self.execution_agent(
                 execution_response=self.response,
                 task=task,
                 context_results=context_results,
                 **kwargs,
             )
             return_response = ""
             try:
@@ -198,156 +191,154 @@
                     )
             except:
                 return_response = self.response
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
-                asyncio.run(self.agent.memories.store_result(task, self.response))
+                await memories.store_result(task, self.response)
             except:
                 pass
             self.agent.log_interaction("USER", task)
             self.agent.log_interaction(self.agent_name, self.response)
         return self.response
 
-    def smart_instruct(
+    async def smart_instruct(
         self,
         task: str = "Write a tweet about AI.",
         shots: int = 3,
-        async_exec: bool = False,
         learn_file: str = "",
         objective: str = None,
         **kwargs,
     ):
         answers = []
         # Do multi shots of prompt to get N different answers to be validated
         answers.append(
-            self.run(
+            await self.run(
                 task=task,
                 prompt="SmartInstruct-StepByStep"
                 if objective == None
                 else "SmartTask-StepByStep",
                 context_results=6,
                 websearch=True,
                 websearch_depth=3,
                 shots=shots,
-                async_exec=async_exec,
                 learn_file=learn_file,
                 objective=objective,
                 **kwargs,
             )
         )
         if shots > 1:
             for i in range(shots - 1):
                 answers.append(
-                    self.run(
+                    await self.run(
                         task=task,
                         prompt="SmartInstruct-StepByStep"
                         if objective == None
                         else "SmartTask-StepByStep",
                         context_results=6,
                         shots=shots,
                         objective=objective,
                         **kwargs,
                     )
                 )
         answer_str = ""
         for i, answer in enumerate(answers):
             answer_str += f"Answer {i + 1}:\n{answer}\n\n"
-        researcher = self.run(
+        researcher = await self.run(
             task=answer_str,
             prompt="SmartInstruct-Researcher",
             shots=shots,
             **kwargs,
         )
-        resolver = self.run(
+        resolver = await self.run(
             task=researcher,
             prompt="SmartInstruct-Resolver",
             shots=shots,
             **kwargs,
         )
-        execution_response = self.run(
+        execution_response = await self.run(
             task=task,
             prompt="SmartInstruct-Execution",
             previous_response=resolver,
             **kwargs,
         )
-        clean_response_agent = self.run(
+        clean_response_agent = await self.run(
             task=task,
             prompt="SmartInstruct-CleanResponse"
             if objective == None
             else "SmartTask-CleanResponse",
             resolver_response=resolver,
             execution_response=execution_response,
             objective=objective,
             **kwargs,
         )
         return clean_response_agent
 
-    def smart_chat(
+    async def smart_chat(
         self,
         task: str = "Write a tweet about AI.",
         shots: int = 3,
-        async_exec: bool = False,
         learn_file: str = "",
         **kwargs,
     ):
         answers = []
         answers.append(
-            self.run(
+            await self.run(
                 task=task,
                 prompt="SmartChat-StepByStep",
                 context_results=6,
                 websearch=True,
                 websearch_depth=3,
                 shots=shots,
-                async_exec=async_exec,
                 learn_file=learn_file,
                 **kwargs,
             )
         )
         # Do multi shots of prompt to get N different answers to be validated
         if shots > 1:
             for i in range(shots - 1):
                 answers.append(
-                    self.run(
+                    await self.run(
                         task=task,
                         prompt="SmartChat-StepByStep",
                         context_results=6,
                         shots=shots,
                         **kwargs,
                     )
                 )
         answer_str = ""
         for i, answer in enumerate(answers):
             answer_str += f"Answer {i + 1}:\n{answer}\n\n"
-        researcher = self.run(
+        researcher = await self.run(
             task=answer_str,
             prompt="SmartChat-Researcher",
             context_results=6,
             shots=shots,
             **kwargs,
         )
-        resolver = self.run(
+        resolver = await self.run(
             task=researcher,
             prompt="SmartChat-Resolver",
             context_results=6,
             shots=shots,
             **kwargs,
         )
-        clean_response_agent = self.run(
+        clean_response_agent = await self.run(
             task=task,
             prompt="SmartChat-CleanResponse",
             resolver_response=resolver,
             **kwargs,
         )
         return clean_response_agent
 
     # Worker Sub-Agents
-    def validation_agent(self, task, execution_response, context_results, **kwargs):
+    async def validation_agent(
+        self, task, execution_response, context_results, **kwargs
+    ):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
             cleaned_json = pattern.findall(execution_response)
             if len(cleaned_json) == 0:
                 return False
             if isinstance(cleaned_json, list):
                 cleaned_json = cleaned_json[0]
@@ -357,74 +348,76 @@
             logging.info("INVALID JSON RESPONSE")
             logging.info(execution_response)
             logging.info("... Trying again.")
             if context_results != 0:
                 context_results = context_results - 1
             else:
                 context_results = 0
-            execution_response = self.run(
+            execution_response = await self.run(
                 task=task, context_results=context_results, **kwargs
             )
-            return self.validation_agent(
+            return await self.validation_agent(
                 task, execution_response, context_results, **kwargs
             )
 
-    def revalidation_agent(
+    async def revalidation_agent(
         self,
         task,
         command_name,
         command_args,
         command_output,
         context_results,
         **kwargs,
     ):
         logging.info(
             f"Command {command_name} did not execute as expected with args {command_args}. Trying again.."
         )
-        revalidate = self.run(
+        revalidate = await self.run(
             task=task,
             prompt="ValidationFailed",
             command_name=command_name,
             command_args=command_args,
             command_output=command_output,
             **kwargs,
         )
-        return self.execution_agent(revalidate, task, context_results, **kwargs)
+        return await self.execution_agent(revalidate, task, context_results, **kwargs)
 
-    def execution_agent(self, execution_response, task, context_results, **kwargs):
-        validated_response = self.validation_agent(
+    async def execution_agent(
+        self, execution_response, task, context_results, **kwargs
+    ):
+        validated_response = await self.validation_agent(
             task, execution_response, context_results, **kwargs
         )
         try:
             for command_name, command_args in validated_response["commands"].items():
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
                         if command_name in [
                             available_command["friendly_name"],
                             available_command["name"],
                         ]:
                             command_name = available_command["friendly_name"]
                             try:
                                 # Check if the command is a valid command in the self.avent.available_commands list
-                                command_output = self.agent.execute(
+                                command_output = await self.agent.execute(
                                     command_name, command_args
                                 )
                                 logging.info("Running Command Execution Validation...")
-                                validate_command = self.run(
+                                validate_command = await self.run(
                                     task=task,
                                     prompt="Validation",
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=command_output,
                                     **kwargs,
                                 )
                                 if validate_command.startswith("Yes"):
                                     # Failed command execution
-                                    return self.revalidation_agent(
+                                    return await self.revalidation_agent(
                                         task=task,
                                         command_name=command_name,
                                         command_args=command_args,
                                         command_output=command_output,
                                         context_results=context_results,
                                         **kwargs,
                                     )
@@ -432,15 +425,15 @@
                                     # Successful command execution
                                     logging.info(
                                         f"Command {command_name} executed successfully with args {command_args}. Command Output: {command_output}"
                                     )
                                     response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
                                     return response
                             except:
-                                return self.revalidation_agent(
+                                return await self.revalidation_agent(
                                     task=task,
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=command_output,
                                     context_results=context_results,
                                     **kwargs,
                                 )
@@ -453,14 +446,16 @@
             logging.info("\nERROR IN EXECUTION_AGENT, validated_response:\n")
             logging.info(validated_response)
             return "\nNo commands were executed.\n"
 
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
+        memories = self.agent.get_memories()
+
         async def resursive_browsing(task, links):
             try:
                 words = links.split()
                 links = [
                     word for word in words if urlparse(word).scheme in ["http", "https"]
                 ]
             except:
@@ -479,33 +474,33 @@
                     if url.startswith("http"):
                         logging.info(f"Scraping: {url}")
                         if url not in self.browsed_links:
                             self.browsed_links.append(url)
                             (
                                 collected_data,
                                 link_list,
-                            ) = await self.agent.memories.read_website(url)
+                            ) = await memories.read_website(url)
                             if link_list is not None:
                                 if len(link_list) > 0:
                                     if len(link_list) > 5:
                                         link_list = link_list[:3]
                                     try:
-                                        pick_a_link = self.run(
+                                        pick_a_link = await self.run(
                                             task=task,
                                             prompt="Pick-a-Link",
                                             links=link_list,
                                         )
                                         if not pick_a_link.startswith("None"):
                                             await resursive_browsing(task, pick_a_link)
                                     except:
                                         logging.info(
                                             f"Issues reading {url}. Moving on..."
                                         )
 
-        results = self.run(task=task, prompt="WebSearch")
+        results = await self.run(task=task, prompt="WebSearch")
         results = results.split("\n")
         for result in results:
             search_string = result.lstrip("0123456789. ")
             try:
                 searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
             except:
                 searx_server = ""
```

### Comparing `agixt-1.1.76b0/agixt/Chain.py` & `agixt-1.1.77b0/agixt/Chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,22 +72,22 @@
                 return step
         return None
 
     def get_steps(self, chain_name):
         chain_data = self.get_chain(chain_name=chain_name)
         return chain_data["steps"]
 
-    def run_chain(self, chain_name):
+    async def run_chain(self, chain_name):
         chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
-                step_response = self.run_chain_step(
+                step_response = await self.run_chain_step(
                     step=step_data, chain_name=chain_name
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
                 logging.info(f"Response: {step_response}")
         # Write the responses to the json file.
         with open(os.path.join("chains", f"{chain_name}_responses.json"), "w") as f:
             json.dump(responses, f)
@@ -118,65 +118,69 @@
             )
             # replace the {STEPx} with the response
             prompt_content = prompt_content.replace(
                 f"{{STEP{step_number}}}", step_response
             )
         return prompt_content
 
-    def run_chain_step(self, step: dict = {}, chain_name=""):
+    async def run_chain_step(self, step: dict = {}, chain_name=""):
         logging.info(step)
         if step:
             if "prompt_type" in step:
                 prompt_type = step["prompt_type"]
                 prompt = step["prompt"]
                 agent_name = step["agent_name"]
+                agent = AGiXT(agent_name)
                 step_number = step["step"]
                 try:
                     command_name = prompt["command_name"]
                 except:
                     command_name = ""
                 if prompt_type == "Command":
                     commands_args = prompt.copy()
                     for arg in commands_args:
                         commands_args[arg] = self.get_step_content(
                             chain_name, step_number, commands_args[arg]
                         )
-                    return Extensions(agent_config=agent_name).execute_command(
+                    return await Extensions(
+                        agent_config=agent.agent.agent_config
+                    ).execute_command(
                         command_name=command_name, command_args=commands_args
                     )
                 try:
                     prompt_content = Prompts().get_prompt(
                         prompt_name=prompt["prompt_name"]
                     )
                     prompt_content = self.get_step_content(
                         chain_name, step_number, prompt_content
                     )
-                    agent = AGiXT(agent_name)
                 except:
                     return None
                 if prompt_type == "Prompt":
-                    result = agent.run(
+                    result = await agent.run(
                         prompt=prompt["prompt_name"],
                         chain_name=chain_name,
                         step_number=step_number,
                         **prompt,
                     )
                 elif prompt_type == "Chain":
-                    result = self.run_chain(prompt["chain_name"])
+                    result = await self.run_chain(prompt["chain_name"])
                 elif prompt_type == "Smart Instruct":
-                    result = agent.smart_instruct(task=prompt_content, **prompt)
+                    result = await agent.smart_instruct(task=prompt_content, **prompt)
                 elif prompt_type == "Smart Chat":
-                    result = agent.smart_chat(task=prompt_content, **prompt)
+                    result = await agent.smart_chat(task=prompt_content, **prompt)
                 elif prompt_type == "Task":
-                    result = agent.run_task(objective=prompt_content, **prompt)
+                    result = await agent.run_task(objective=prompt_content, **prompt)
         if result:
             return result
         else:
             return None
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--chain", type=str, default="")
     args = parser.parse_args()
     chain_name = args.chain
-    Chain().run_chain(chain_name=chain_name)
+    import asyncio
+
+    asyncio.run(Chain().run_chain(chain_name=chain_name))
```

### Comparing `agixt-1.1.76b0/agixt/Config.py` & `agixt-1.1.77b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/Embedding.py` & `agixt-1.1.77b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/Extensions.py` & `agixt-1.1.77b0/agixt/Extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         return None, None, None  # Updated return statement
 
     def get_commands_list(self):
         self.commands = self.load_commands(agent_name=self.agent_name)
         commands_list = [command_name for command_name, _, _ in self.commands]
         return commands_list
 
-    def execute_command(self, command_name: str, command_args: dict = None):
+    async def execute_command(self, command_name: str, command_args: dict = None):
         command_function, module, params = self.find_command(command_name=command_name)
         logging.info(
             f"Executing command: {command_name} with args: {command_args}. Command Function: {command_function}"
         )
         if command_function is None:
             logging.error(f"Command {command_name} not found")
             return False
@@ -146,12 +146,12 @@
                 if param != "self" and param != "kwargs":
                     command_args[param] = None
         args = command_args.copy()
         for param in command_args:
             if param not in params:
                 del args[param]
         try:
-            output = getattr(module(), command_function.__name__)(**args)
+            output = await getattr(module(), command_function.__name__)(**args)
         except Exception as e:
             output = f"Error: {str(e)}"
         logging.info(f"Command Output: {output}")
         return output
```

### Comparing `agixt-1.1.76b0/agixt/Main.py` & `agixt-1.1.77b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/Memories.py` & `agixt-1.1.77b0/agixt/Memories.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.collection = None
         self.nlp = None
         self.chunk_size = 128
         memories_dir = os.path.join(os.getcwd(), "agents", self.agent_name, "memories")
         self.chroma_client = ChromaMemoryStore(
             persist_directory=memories_dir,
             client_settings=Settings(
-                chroma_db_impl="chromadb.db.duckdb.PersistentDuckDB",
+                chroma_db_impl="duckdb+parquet",
                 persist_directory=memories_dir,
                 anonymized_telemetry=False,
             ),
         )
 
     def load_spacy_model(self):
         if not self.nlp:
@@ -113,25 +113,20 @@
                 )
 
     async def context_agent(self, query: str, top_results_num: int) -> List[str]:
         embedder, chunk_size = await self.get_embedder()
         collection = await self.get_collection()
         if collection == None:
             return []
-        try:
-            results = await self.chroma_client.get_nearest_matches_async(
-                collection_name="memories",
-                embedding=await embedder(query),
-                limit=top_results_num,
-                min_relevance_score=0.1,
-            )
-        except Exception as e:
-            logging.info(f"Failed to get context: {e}")
-            return []
-        # Each result is as results._text
+        results = await self.chroma_client.get_nearest_matches_async(
+            collection_name="memories",
+            embedding=await embedder(query),
+            limit=top_results_num,
+            min_relevance_score=0.1,
+        )
         context = []
         for memory, score in results:
             context.append(memory._text)
         trimmed_context = await self.trim_context(context)
         logging.info(f"CONTEXT: {trimmed_context}")
         context_str = "\n".join(trimmed_context)
         response = f"Context: {context_str}\n\n"
```

### Comparing `agixt-1.1.76b0/agixt/Prompts.py` & `agixt-1.1.77b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/Tasks.py` & `agixt-1.1.77b0/agixt/Tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,46 +97,46 @@
         return files
 
     def stop_tasks(self):
         if self.stop_running_event is not None:
             self.stop_running_event = True
         self.task_list.clear()
 
-    def instruction_agent(self, task, **kwargs):
+    async def instruction_agent(self, task, **kwargs):
         if "task_name" in task:
             task = task["task_name"]
 
-        resolver = self.ai.run(
+        resolver = await self.ai.run(
             task=task,
             prompt="SmartInstruct-StepByStep"
             if self.primary_objective is None
             else "SmartTask-StepByStep",
             context_results=6,
             objective=self.primary_objective,
             **kwargs,
         )
         # Check if agent has commands before trying to run execution agent
-        if Agent(self.agent_name).get_commands_string() != None:
-            execution_response = self.ai.run(
+
+        if Agent(agent_name=self.agent_name).get_commands_string() != None:
+            execution_response = await self.ai.run(
                 task=task,
                 prompt="SmartInstruct-Execution"
                 if self.primary_objective is None
                 else "SmartTask-Execution",
                 previous_response=resolver,
                 objective=self.primary_objective,
                 **kwargs,
             )
             return f"RESPONSE:\n{resolver}\n\nCommand Execution Response{execution_response}"
         else:
             return f"RESPONSE:\n{resolver}"
 
-    def run_task(
+    async def run_task(
         self,
         objective: str = "",
-        async_exec: bool = False,
         smart: bool = False,
         load_task: str = "",
         **kwargs,
     ):
         initial_task = "Break down the objective into a list of small achievable tasks in the form of instructions that lead up to achieving the ultimate goal of the objective."
         if load_task != "":
             self.load_task(load_task)
@@ -156,20 +156,19 @@
         while not self.stop_running_event and self.task_list != deque([]):
             task = self.task_list.popleft()
             if task["task_name"] in ["None", "None.", ""]:
                 self.stop_tasks()
                 continue
             logging.info(f"\nExecuting task {task['task_id']}: {task['task_name']}\n")
             if smart != True:
-                result = self.instruction_agent(task=task["task_name"], **kwargs)
+                result = await self.instruction_agent(task=task["task_name"], **kwargs)
             else:
-                result = self.ai.smart_instruct(
+                result = await self.ai.smart_instruct(
                     task=task["task_name"],
                     shots=3,
-                    async_exec=async_exec,
                     objective=self.primary_objective,
                     **kwargs,
                 )
             self.update_task(task["task_id"], task["task_name"], result)
             logging.info(f"\nTask Result:\n\n{result}\n")
             if task["task_name"] == initial_task:
                 lines = result.split("\n") if "\n" in result else [result]
```

### Comparing `agixt-1.1.76b0/agixt/app.py` & `agixt-1.1.77b0/agixt/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,39 +180,39 @@
     Agent(agent_name).wipe_agent_memories(agent_name)
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
 @app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
 async def instruct(agent_name: str, prompt: Prompt):
     agent = AGiXT(agent_name)
-    response = agent.run(
+    response = await agent.run(
         task=prompt.prompt,
         prompt="instruct",
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartinstruct/{shots}", tags=["Agent"])
 async def smartinstruct(agent_name: str, shots: int, prompt: Prompt):
     agent = AGiXT(agent_name)
-    response = agent.smart_instruct(task=prompt.prompt, shots=int(shots))
+    response = await agent.smart_instruct(task=prompt.prompt, shots=int(shots))
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/chat", tags=["Agent"])
 async def chat(agent_name: str, prompt: Prompt):
     agent = AGiXT(agent_name)
-    response = agent.run(prompt.prompt, prompt="Chat", context_results=6)
+    response = await agent.run(prompt.prompt, prompt="Chat", context_results=6)
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartchat/{shots}", tags=["Agent"])
 async def smartchat(agent_name: str, shots: int, prompt: Prompt):
     agent = AGiXT(agent_name)
-    response = agent.smart_chat(prompt.prompt, shots=shots)
+    response = await agent.smart_chat(prompt.prompt, shots=shots)
     return {"response": str(response)}
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
     agent = Agent(agent_name)
     return {"commands": agent.agent_config["commands"]}
@@ -290,15 +290,15 @@
 async def get_chain(chain_name: str):
     chain_data = Chain().get_chain(chain_name)
     return {"chain": chain_data}
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
 async def run_chain(chain_name: str) -> ResponseMessage:
-    Chain().run_chain(chain_name)
+    await Chain().run_chain(chain_name)
     return {"message": f"Chain '{chain_name}' started."}
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
     Chain().add_chain(chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
```

### Comparing `agixt-1.1.76b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.77b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.77b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/auth_libs/Users.py` & `agixt-1.1.77b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/chains/Smart Chat.json` & `agixt-1.1.77b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/chains/Test_Commands.json` & `agixt-1.1.77b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/components/agent_selector.py` & `agixt-1.1.77b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/example.ipynb` & `agixt-1.1.77b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.77b0/agixt/extensions/agixt_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,94 +33,96 @@
                     self.commands.update(
                         {f"Run Chain: {chain['name']}": self.run_chain}
                     )
 
     def command_exists(self, file_name: str) -> bool:
         return os.path.exists(f"commands/{file_name}.py")
 
-    def create_command(
-        self, function_description: str, agent_name: str = "AGiXT"
+    async def create_command(
+        self, function_description: str, agent: str = "AGiXT"
     ) -> List[str]:
         with open(f"prompts/Create New Command.txt", "r") as f:
             prompt = f.read()
         prompt = prompt.replace("{{NEW_FUNCTION_DESCRIPTION}}", function_description)
-        response = AGiXT(agent_name).run(prompt)
+        response = await AGiXT(agent).run(prompt)
         file_name = response.split("class ")[1].split("(")[0]
         code = code.replace("```", "")
 
         if not self.command_exists(file_name):
             with open(f"commands/{file_name}.py", "w") as f:
                 f.write(code)
             return f"Created new command: {file_name}."
         else:
             return f"Command {file_name} already exists. No changes were made."
 
-    def evaluate_code(self, code: str, agent_name: str = "AGiXT") -> List[str]:
+    async def evaluate_code(self, code: str, agent: str = "AGiXT") -> List[str]:
         args = [code]
         function_string = "def analyze_code(code: str) -> List[str]:"
         description_string = "Analyzes the given code and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def analyze_pull_request(self, pr_url: str, agent_name: str = "AGiXT") -> List[str]:
+    async def analyze_pull_request(
+        self, pr_url: str, agent: str = "AGiXT"
+    ) -> List[str]:
         args = [pr_url]
         function_string = "def analyze_pr(pr_url: str) -> List[str]:"
         description_string = "Analyzes the given pull request and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def perform_automated_testing(
-        self, test_url: str, agent_name: str = "AGiXT"
+    async def perform_automated_testing(
+        self, test_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [test_url]
         function_string = "def perform_testing(test_url: str) -> List[str]:"
         description_string = "Performs automated testing using AI-driven tools and returns a list of test results."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def improve_code(
-        self, suggestions: List[str], code: str, agent_name: str = "AGiXT"
+    async def improve_code(
+        self, suggestions: List[str], code: str, agent: str = "AGiXT"
     ) -> str:
         args = [json.dumps(suggestions), code]
         function_string = (
             "def generate_improved_code(suggestions: List[str], code: str) -> str:"
         )
         description_string = "Improves the provided code based on the suggestions provided, making no other changes."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def write_tests(
+    async def write_tests(
         self,
         code: str,
         focus: Optional[List[str]] = None,
-        agent_name: str = "AGiXT",
+        agent: str = "AGiXT",
     ) -> str:
         args = [code, json.dumps(focus) if focus else "None"]
         function_string = "def create_test_cases(code: str, focus: Optional[List[str]] = None) -> str:"
         description_string = "Generates test cases for the existing code, focusing on specific areas if required."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def run_ci_cd_pipeline(self, repo_url: str, agent_name: str = "AGiXT") -> str:
+    async def run_ci_cd_pipeline(self, repo_url: str, agent: str = "AGiXT") -> str:
         args = [repo_url]
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return AGiXT(agent_name).run(prompt)
+        return await AGiXT(agent).run(prompt)
 
-    def run_chain(self, chain_name):
-        Chain().run_chain(chain_name)
+    async def run_chain(self, chain_name):
+        await Chain().run_chain(chain_name)
         return "Chain started successfully."
 
-    def ask(self, prompt: str, agent_name: str = "AGiXT") -> str:
-        response = AGiXT(agent_name).run(
+    async def ask(self, prompt: str, agent: str = "AGiXT") -> str:
+        response = await AGiXT(agent).run(
             prompt, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
-    def instruct(self, prompt: str, agent_name: str = "AGiXT") -> str:
-        response = AGiXT(agent_name).run(
+    async def instruct(self, prompt: str, agent: str = "AGiXT") -> str:
+        response = await AGiXT(agent).run(
             task=prompt, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
```

### Comparing `agixt-1.1.76b0/agixt/extensions/briantts.py` & `agixt-1.1.77b0/agixt/extensions/briantts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         USE_BRIAN_TTS: bool = True,
         **kwargs,
     ):
         self.USE_BRIAN_TTS = USE_BRIAN_TTS
         if self.USE_BRIAN_TTS:
             self.commands = {"Speak with TTS with BrianTTS": self.speak_with_briantts}
 
-    def speak_with_briantts(self, text: str) -> bool:
+    async def speak_with_briantts(self, text: str) -> bool:
         tts_url = (
             f"https://api.streamelements.com/kappa/v2/speech?voice=Brian&text={text}"
         )
         response = requests.get(tts_url)
 
         if response.status_code == 200:
             with open("speech.mp3", "wb") as f:
```

### Comparing `agixt-1.1.76b0/agixt/extensions/dalle.py` & `agixt-1.1.77b0/agixt/extensions/dalle.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.OPENAI_API_KEY = OPENAI_API_KEY
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
         if self.OPENAI_API_KEY:
             self.commands = {
                 "Generate Image with DALLE": self.generate_image_with_dalle
             }
 
-    def generate_image_with_dalle(self, prompt: str, filename: str) -> str:
+    async def generate_image_with_dalle(self, prompt: str, filename: str) -> str:
         openai.api_key = self.OPENAI_API_KEY
 
         response = openai.Image.create(
             prompt=prompt,
             n=1,
             size="256x256",
             response_format="b64_json",
```

### Comparing `agixt-1.1.76b0/agixt/extensions/discord.py` & `agixt-1.1.77b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.77b0/agixt/extensions/elevenlabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         ELEVENLABS_VOICE: str = "Josh",
         **kwargs,
     ):
         self.ELEVENLABS_API_KEY = ELEVENLABS_API_KEY
         self.ELEVENLABS_VOICE = ELEVENLABS_VOICE
         self.commands = {"Speak with TTS Using Elevenlabs": self.speak_with_elevenlabs}
 
-    def speak_with_elevenlabs(self, text: str, voice_index: int = 0) -> bool:
+    async def speak_with_elevenlabs(self, text: str, voice_index: int = 0) -> bool:
         voices = ["ErXwobaYiN019PkySvjV", "EXAVITQu4vr4xnSDxMaL"]
         headers = {
             "Content-Type": "application/json",
             "xi-api-key": self.ELEVENLABS_VOICE,
         }
 
         tts_url = f"https://api.elevenlabs.io/v1/text-to-speech/{voices[voice_index]}"
```

### Comparing `agixt-1.1.76b0/agixt/extensions/file_system.py` & `agixt-1.1.77b0/agixt/extensions/file_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "Delete File": self.delete_file,
             "Search Files": self.search_files,
             "Execute Python File": self.execute_python_file,
             "Execute Shell": self.execute_shell,
         }
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
 
-    def execute_python_file(self, file: str):
+    async def execute_python_file(self, file: str):
         logging.info(f"Executing file '{file}' in workspace '{self.WORKING_DIRECTORY}'")
 
         if not file.endswith(".py"):
             return "Error: Invalid file type. Only .py files are allowed."
 
         file_path = os.path.join(self.WORKING_DIRECTORY, file)
 
@@ -91,15 +91,15 @@
             container.remove()
 
             return logs
 
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def execute_shell(self, command_line: str) -> str:
+    async def execute_shell(self, command_line: str) -> str:
         current_dir = os.getcwd()
         os.chdir(current_dir)
         logging.info(
             f"Executing command '{command_line}' in working directory '{os.getcwd()}'"
         )
         result = subprocess.run(command_line, capture_output=True, shell=True)
         output = f"STDOUT:\n{result.stdout}\nSTDERR:\n{result.stderr}"
@@ -122,53 +122,53 @@
                     os.makedirs(new_path)
         else:
             new_path = os.path.normpath(os.path.join("/", *paths))
             if not os.path.exists(new_path):
                 os.makedirs(new_path)
         return new_path
 
-    def read_file(self, filename: str) -> str:
+    async def read_file(self, filename: str) -> str:
         try:
             filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             with open(filepath, "r", encoding="utf-8") as f:
                 content = f.read()
             return content
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def write_to_file(self, filename: str, text: str) -> str:
+    async def write_to_file(self, filename: str, text: str) -> str:
         try:
             filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             directory = os.path.dirname(filepath)
             if not os.path.exists(directory):
                 os.makedirs(directory)
             with open(filepath, "w", encoding="utf-8") as f:
                 f.write(text)
             return "File written to successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def append_to_file(self, filename: str, text: str) -> str:
+    async def append_to_file(self, filename: str, text: str) -> str:
         try:
             filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             with open(filepath, "a") as f:
                 f.write(text)
             return "Text appended successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def delete_file(self, filename: str) -> str:
+    async def delete_file(self, filename: str) -> str:
         try:
             filepath = self.safe_join(base=self.WORKING_DIRECTORY, paths=filename)
             os.remove(filepath)
             return "File deleted successfully."
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def search_files(self, directory: str) -> List[str]:
+    async def search_files(self, directory: str) -> List[str]:
         found_files = []
 
         if directory in {"", "/"}:
             search_directory = self.WORKING_DIRECTORY
         else:
             search_directory = self.safe_join(
                 base=self.WORKING_DIRECTORY, paths=directory
```

### Comparing `agixt-1.1.76b0/agixt/extensions/github.py` & `agixt-1.1.77b0/agixt/extensions/github.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,29 +14,29 @@
         self.GITHUB_USERNAME = GITHUB_USERNAME
         self.GITHUB_API_KEY = GITHUB_API_KEY
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
         self.commands = {"Clone Github Repository": self.clone_repo}
         if self.GITHUB_USERNAME and self.GITHUB_API_KEY:
             self.commands["Create Github Repository"] = self.create_repo
 
-    def clone_repo(self, repo_url: str, clone_path: str) -> str:
+    async def clone_repo(self, repo_url: str, clone_path: str) -> str:
         split_url = repo_url.split("//")
         if self.GITHUB_USERNAME is not None and self.GITHUB_API_KEY is not None:
             auth_repo_url = f"//{self.GITHUB_USERNAME}:{self.GITHUB_API_KEY}@".join(
                 split_url
             )
         else:
             auth_repo_url = "//".join(split_url)
         try:
             git.Repo.clone_from(auth_repo_url, self.WORKING_DIRECTORY + clone_path)
             return f"""Cloned {repo_url} to {self.WORKING_DIRECTORY + clone_path}"""
         except Exception as e:
             return f"Error: {str(e)}"
 
-    def create_repo(self, repo_name: str, readme: str) -> str:
+    async def create_repo(self, repo_name: str, readme: str) -> str:
         g = Github(self.GITHUB_API_KEY)
         user = g.get_user(self.GITHUB_USERNAME)
         repo = user.create_repo(repo_name, private=True)
         repo_url = repo.clone_url
         repo_dir = f"./{repo_name}"
         repo = git.Repo.init(repo_dir)
         with open(f"{repo_dir}/README.md", "w") as f:
```

### Comparing `agixt-1.1.76b0/agixt/extensions/google.py` & `agixt-1.1.77b0/agixt/extensions/google.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, GOOGLE_API_KEY: str = "", **kwargs):
         self.GOOGLE_API_KEY = GOOGLE_API_KEY
         if self.GOOGLE_API_KEY:
             self.commands = {
                 "Google Search": self.google_official_search,
             }
 
-    def google_official_search(
+    async def google_official_search(
         self, query: str, num_results: int = 8
     ) -> Union[str, List[str]]:
         from googleapiclient.discovery import build
         from googleapiclient.errors import HttpError
 
         try:
             # Get the Google API key and Custom Search Engine ID from the config file
```

### Comparing `agixt-1.1.76b0/agixt/extensions/gtts.py` & `agixt-1.1.77b0/agixt/extensions/gtts.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,13 +10,13 @@
         USE_GTTS: bool = False,
         **kwargs,
     ):
         self.USE_GTTS = USE_GTTS
         if USE_GTTS:
             self.commands = {"Speak with GTTS": self.speak_with_gtts}
 
-    def speak_with_gtts(self, text: str) -> bool:
+    async def speak_with_gtts(self, text: str) -> bool:
         tts = ts.gTTS(text)
         tts.save("speech.mp3")
         playsound("speech.mp3", True)
         os.remove("speech.mp3")
         return True
```

### Comparing `agixt-1.1.76b0/agixt/extensions/huggingface.py` & `agixt-1.1.77b0/agixt/extensions/huggingface.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if self.HUGGINGFACE_API_KEY is not None:
             self.commands = {
                 "Read Audio from File": self.read_audio_from_file,
                 "Read Audio": self.read_audio,
                 "Generate Image with Stable Diffusion": self.generate_image_with_hf,
             }
 
-    def generate_image_with_hf(self, prompt: str, filename: str) -> str:
+    async def generate_image_with_hf(self, prompt: str, filename: str) -> str:
         API_URL = (
             "https://api-inference.huggingface.co/models/CompVis/stable-diffusion-v1-4"
         )
         headers = {"Authorization": f"Bearer {self.HUGGINGFACE_API_TOKEN}"}
 
         response = requests.post(
             API_URL,
@@ -43,21 +43,21 @@
         image = Image.open(BytesIO(response.content))
         logging.info(f"Image Generated for prompt:{prompt}")
 
         image.save(os.path.join(self.WORKING_DIRECTORY, filename))
 
         return f"Saved to disk:{filename}"
 
-    def read_audio_from_file(self, audio_path: str):
+    async def read_audio_from_file(self, audio_path: str):
         audio_path = os.path.join(self.WORKING_DIRECTORY, audio_path)
         with open(audio_path, "rb") as audio_file:
             audio = audio_file.read()
-        return self.read_audio(audio)
+        return await self.read_audio(audio)
 
-    def read_audio(self, audio):
+    async def read_audio(self, audio):
         model = self.HUGGINGFACE_AUDIO_TO_TEXT_MODEL
         api_url = f"https://api-inference.huggingface.co/models/{model}"
         api_token = self.HUGGINGFACE_API_KEY
         headers = {"Authorization": f"Bearer {api_token}"}
 
         if api_token is None:
             raise ValueError(
```

### Comparing `agixt-1.1.76b0/agixt/extensions/macostts.py` & `agixt-1.1.77b0/agixt/extensions/macostts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self,
         USE_MAC_OS_TTS: bool = False,
         **kwargs,
     ):
         self.USE_MAC_OS_TTS = USE_MAC_OS_TTS
         self.commands = {"Speak with MacOS TTS": self.speak_with_macos_speech}
 
-    def speak_with_macos_speech(self, text: str, voice_index: int = 0) -> bool:
+    async def speak_with_macos_speech(self, text: str, voice_index: int = 0) -> bool:
         if voice_index == 0:
             os.system(f'say "{text}"')
         elif voice_index == 1:
             os.system(f'say -v "Ava (Premium)" "{text}"')
         else:
             os.system(f'say -v Samantha "{text}"')
         return True
```

### Comparing `agixt-1.1.76b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.77b0/agixt/extensions/microsoft_365.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     self.MICROSOFT_365_CLIENT_SECRET != "None"
                     and self.MICROSOFT_365_CLIENT_SECRET != ""
                 ):
                     self.credentials = self.get_credentials()
             except:
                 pass
 
-    def get_credentials(self) -> Credentials:
+    async def get_credentials(self) -> Credentials:
         flow = InstalledAppFlow.from_client_config(
             {
                 "installed": {
                     "client_id": self.MICROSOFT_365_CLIENT_ID,
                     "client_secret": self.MICROSOFT_365_CLIENT_SECRET,
                     "redirect_uris": [self.MICROSOFT_365_REDIRECT_URI],
                     "auth_uri": "https://login.microsoftonline.com/common/oauth2/v2.0/authorize",
@@ -48,15 +48,15 @@
                 }
             },
             ["https://graph.microsoft.com/Mail.ReadWrite"],
         )
 
         return flow.run_local_server(port=0)
 
-    def send_email(
+    async def send_email(
         self, from_email: str, to_email: str, subject: str, content: str
     ) -> List[str]:
         try:
             message = {
                 "message": {
                     "subject": subject,
                     "body": {"contentType": "HTML", "content": content},
@@ -71,30 +71,32 @@
                 service.users().messages().send(userId="me", body=message).execute()
             )
             return [f"Email sent successfully. Message ID: {response['id']}"]
 
         except HttpError as error:
             return [f"Error sending email: {error}"]
 
-    def check_email(self) -> List[str]:
+    async def check_email(self) -> List[str]:
         try:
             service = build("graph.microsoft.com", "v1.0", credentials=self.credentials)
             response = service.users().messages().list(userId="me").execute()
             emails = response.get("value", [])
 
             result = []
             for email in emails:
                 result.append(f"Email ID: {email['id']}, Subject: {email['subject']}")
 
             return result
 
         except HttpError as error:
             return [f"Error checking email: {error}"]
 
-    def move_email(self, message_id: str, destination_folder_id: str) -> List[str]:
+    async def move_email(
+        self, message_id: str, destination_folder_id: str
+    ) -> List[str]:
         try:
             service = build("graph.microsoft.com", "v1.0", credentials=self.credentials)
             response = (
                 service.users()
                 .messages()
                 .move(
                     userId="me",
```

### Comparing `agixt-1.1.76b0/agixt/extensions/searxng.py` & `agixt-1.1.77b0/agixt/extensions/searxng.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 self.SEARXNG_INSTANCE_URL = servers[random_index]
             except:  # Select default remote server that typically works if unable to get list.
                 self.SEARXNG_INSTANCE_URL = "https://search.us.projectsegfau.lt"
         server = self.SEARXNG_INSTANCE_URL.rstrip("/")
         endpoint = f"{server}/search"
         return endpoint
 
-    def search(self, query: str) -> List[str]:
+    async def search(self, query: str) -> List[str]:
         try:
             response = requests.get(
                 self.SEARXNG_ENDPOINT,
                 params={
                     "q": query,
                     "language": "en",
                     "safesearch": 1,
```

### Comparing `agixt-1.1.76b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.77b0/agixt/extensions/sendgrid_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class sendgrid_email(Extensions):
     def __init__(self, SENDGRID_API_KEY: str = "", SENDGRID_EMAIL: str = "", **kwargs):
         self.SENDGRID_API_KEY = SENDGRID_API_KEY
         self.SENDGRID_EMAIL = SENDGRID_EMAIL
         if self.SENDGRID_API_KEY:
             self.commands = {"Send Email with Sendgrid": self.send_email}
 
-    def send_email(self, to_email: str, subject: str, content: str) -> List[str]:
+    async def send_email(self, to_email: str, subject: str, content: str) -> List[str]:
         message = Mail(
             from_email=self.SENDGRID_EMAIL,
             to_emails=to_email,
             subject=subject,
             html_content=content,
         )
```

### Comparing `agixt-1.1.76b0/agixt/extensions/twitter.py` & `agixt-1.1.77b0/agixt/extensions/twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.TW_CONSUMER_KEY = TW_CONSUMER_KEY
         self.TW_CONSUMER_SECRET = TW_CONSUMER_SECRET
         self.TW_ACCESS_TOKEN = TW_ACCESS_TOKEN
         self.TW_ACCESS_TOKEN_SECRET = TW_ACCESS_TOKEN_SECRET
         if self.TW_CONSUMER_KEY and self.TW_ACCESS_TOKEN:
             self.commands = {"Send Tweet": self.send_tweet}
 
-    def send_tweet(self, tweet_text):
+    async def send_tweet(self, tweet_text):
         # Authenticate to Twitter
         auth = tweepy.OAuthHandler(self.TW_CONSUMER_KEY, self.TW_CONSUMER_SECRET)
         auth.set_access_token(self.TW_ACCESS_TOKEN, self.TW_ACCESS_TOKEN_SECRET)
 
         # Create API object
         api = tweepy.API(auth)
```

### Comparing `agixt-1.1.76b0/agixt/extensions/web_playwright.py` & `agixt-1.1.77b0/agixt/extensions/web_playwright.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class web_playwright(Extensions):
     def __init__(self, **kwargs):
         self.commands = {
             "Scrape Text with Playwright": self.scrape_text_with_playwright,
             "Scrape Links with Playwright": self.scrape_links_with_playwright,
         }
 
-    def scrape_text_with_playwright(self, url: str) -> str:
+    async def scrape_text_with_playwright(self, url: str) -> str:
         with sync_playwright() as p:
             browser = p.chromium.launch()
             page = browser.new_page()
 
             try:
                 page.goto(url)
                 html_content = page.content()
@@ -36,15 +36,15 @@
                 text = f"Error: {str(e)}"
 
             finally:
                 browser.close()
 
         return text
 
-    def scrape_links_with_playwright(self, url: str) -> Union[str, List[str]]:
+    async def scrape_links_with_playwright(self, url: str) -> Union[str, List[str]]:
         with sync_playwright() as p:
             browser = p.chromium.launch()
             page = browser.new_page()
 
             try:
                 page.goto(url)
                 html_content = page.content()
```

### Comparing `agixt-1.1.76b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.77b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/pages/1-Learning.py` & `agixt-1.1.77b0/agixt/pages/1-Learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 
 # Initialize session state for stop events and agent status if not exist
 if "agent_status" not in st.session_state:
     st.session_state.agent_status = {}
 
 if agent_name:
     st.markdown("## Learn from a file")
+    memories = agent.get_memories()
     learn_file_upload = st.file_uploader(
         "Upload a file for the agent to learn from.", accept_multiple_files=True
     )
     if learn_file_upload is not None:
         for learn_file_upload in learn_file_upload.copy():
             learn_file_path = os.path.join(
                 "data", "uploaded_files", learn_file_upload.name
             )
             if not os.path.exists(os.path.dirname(learn_file_path)):
                 os.makedirs(os.path.dirname(learn_file_path))
             with open(learn_file_path, "wb") as f:
                 f.write(learn_file_upload.getbuffer())
-            asyncio.run(agent.memories.mem_read_file(learn_file_path))
+            asyncio.run(memories.mem_read_file(learn_file_path))
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
-            _, _ = asyncio.run(agent.memories.read_website(learn_url))
+            _, _ = asyncio.run(memories.read_website(learn_url))
             st.success(f"Agent '{agent_name}' has learned from the URL.")
     st.markdown("## Wipe Agent Memory")
     st.markdown(
         "The agent can simply learn too much undesired information at times. If you're having an issue with the context being injected from memory with your agent, try wiping the memory."
     )
     if st.button("Wipe agent memory"):
         agent.wipe_agent_memories(agent_name)
```

### Comparing `agixt-1.1.76b0/agixt/pages/2-Prompts.py` & `agixt-1.1.77b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/pages/3-Chains.py` & `agixt-1.1.77b0/agixt/pages/3-Chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import auth_libs.Redirect as redir
 from Config import Config
 from Chain import Chain
 from Extensions import Extensions
 from Agent import Agent
 from Prompts import Prompts
 import logging
+import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 
-agent_name, agent = agent_selector()
 CFG = Config()
 
 st.header("Manage Chains")
 st.markdown("### Predefined Injection Variables")
 st.markdown(
     """
     Any of these variables can be used in command arguments or prompt arguments to inject data into the prompt. These can also be used inside of any Custom Prompt.
@@ -41,15 +41,15 @@
             st.success(f"Chain '{chain_name}' created.")
             st.experimental_rerun()
         elif chain_action == "Delete Chain":
             Chain().delete_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' deleted.")
             st.experimental_rerun()
         elif chain_action == "Run Chain":
-            Chain().run_chain(chain_name=chain_name)
+            asyncio.run(Chain().run_chain(chain_name=chain_name))
             st.success(f"Chain '{chain_name}' executed.")
     else:
         st.error("Chain name is required.")
 
 st.header("Manage Chain Steps & View Responses")
 
 chain_names = Chain().get_chains()
@@ -283,19 +283,19 @@
                             arg != "context"
                             and arg != "command_list"
                             and arg != "COMMANDS"
                         ):
                             prompt_data[arg] = st.session_state[f"add_step_{arg}"]
 
                 Chain().add_chain_step(
-                    selected_chain_name,
-                    step_number,
-                    agent_name,
-                    prompt_type,
-                    prompt_data,
+                    chain_name=selected_chain_name,
+                    step_number=step_number,
+                    agent_name=agent_name,
+                    prompt_type=prompt_type,
+                    prompt=prompt_data,
                 )
                 st.success(
                     f"Step {step_number} added to chain '{selected_chain_name}'."
                 )
                 st.experimental_rerun()
             elif step_action == "Update Step":
                 if prompt_type == "Command":
```

### Comparing `agixt-1.1.76b0/agixt/pages/4-Chat.py` & `agixt-1.1.77b0/agixt/pages/4-Chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     container,
     text_input,
     button,
     spinner,
     error,
     warning,
 )
-
+import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 agent_name, agent = agent_selector()
 
 
@@ -57,26 +57,29 @@
 
     chat_prompt = text_input("Enter your message", key="chat_prompt")
     send_button = button("Send Message")
 
     if send_button:
         if agent_name and chat_prompt:
             with spinner("Thinking, please wait..."):
-                agent = AGiXT(agent_name)
+                agent = AGiXT(agent_name=agent_name)
                 if smart_chat_toggle:
-                    response = agent.smart_chat(
-                        chat_prompt,
-                        shots=3,
-                        async_exec=True,
+                    response = asyncio.run(
+                        agent.smart_chat(
+                            chat_prompt,
+                            shots=3,
+                        )
                     )
                 else:
-                    response = agent.run(
-                        chat_prompt,
-                        prompt="Chat",
-                        context_results=6,
+                    response = asyncio.run(
+                        agent.run(
+                            chat_prompt,
+                            prompt="Chat",
+                            context_results=6,
+                        )
                     )
             chat_entry = [
                 {"sender": "User", "message": chat_prompt},
                 {"sender": "Agent", "message": response},
             ]
             st.session_state.chat_history[agent_name].extend(chat_entry)
             render_chat_history(
```

### Comparing `agixt-1.1.76b0/agixt/pages/5-Instructions.py` & `agixt-1.1.77b0/agixt/pages/5-Instructions.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     container,
     text_input,
     button,
     spinner,
     error,
     warning,
 )
-
+import asyncio
 from auth_libs.Users import check_auth_status
 from components.agent_selector import agent_selector
 
 check_auth_status()
 agent_name, agent = agent_selector()
 
 
@@ -59,24 +59,27 @@
     send_button = button("Send Message")
 
     if send_button:
         if agent_name and instruct_prompt:
             with spinner("Thinking, please wait..."):
                 agent = AGiXT(agent_name)
                 if smart_instruct_toggle:
-                    response = agent.smart_instruct(
-                        instruct_prompt,
-                        shots=3,
-                        async_exec=True,
+                    response = asyncio.run(
+                        agent.smart_instruct(
+                            instruct_prompt,
+                            shots=3,
+                        )
                     )
                 else:
-                    response = agent.run(
-                        instruct_prompt,
-                        prompt="instruct",
-                        context_results=6,
+                    response = asyncio.run(
+                        agent.run(
+                            instruct_prompt,
+                            prompt="instruct",
+                            context_results=6,
+                        )
                     )
             instruct_entry = [
                 {"sender": "User", "message": instruct_prompt},
                 {"sender": "Agent", "message": response},
             ]
             st.session_state.chat_history[agent_name].extend(instruct_entry)
             render_history(
```

### Comparing `agixt-1.1.76b0/agixt/pages/6-Tasks.py` & `agixt-1.1.77b0/agixt/pages/6-Tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import streamlit as st
 from Tasks import Tasks
 from auth_libs.Users import check_auth_status
 from pathlib import Path
 from components.agent_selector import agent_selector
+import asyncio
 
 check_auth_status()
 
 agent_name, agent = agent_selector()
 st.title("Manage Tasks")
 
 
@@ -26,19 +27,20 @@
     )
 
     col1, col2 = st.columns([3, 1])
     with col1:
         columns = st.columns([3, 2])
         if st.button("Start Task", key=f"start_{agent_name}"):
             if agent_name and (task_objective or load_task):
-                task_agent.run_task(
-                    objective=task_objective,
-                    async_exec=True,
-                    smart=smart_task_toggle,
-                    load_task=load_task,
+                asyncio.run(
+                    task_agent.run_task(
+                        objective=task_objective,
+                        smart=smart_task_toggle,
+                        load_task=load_task,
+                    )
                 )
                 st.experimental_rerun()
             else:
                 columns[0].error("Agent name and task objective are required.")
 
         if st.button("Stop Task", key=f"stop_{agent_name}"):
             task_agent.stop_tasks()
```

### Comparing `agixt-1.1.76b0/agixt/pages/Login.py` & `agixt-1.1.77b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/pages/Profile.py` & `agixt-1.1.77b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/pages/Register.py` & `agixt-1.1.77b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.77b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/Execution.txt` & `agixt-1.1.77b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/Instruction.txt` & `agixt-1.1.77b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.77b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.77b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.77b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.77b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.77b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/instruct.txt` & `agixt-1.1.77b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.77b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.77b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/__init__.py` & `agixt-1.1.77b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/azure.py` & `agixt-1.1.77b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/bing.py` & `agixt-1.1.77b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/chatgpt.py` & `agixt-1.1.77b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/claude.py` & `agixt-1.1.77b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/fastchat.py` & `agixt-1.1.77b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/gpt4all.py` & `agixt-1.1.77b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/gpt4free.py` & `agixt-1.1.77b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.77b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/huggingchat.py` & `agixt-1.1.77b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/huggingface.py` & `agixt-1.1.77b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/kobold.py` & `agixt-1.1.77b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/llamacpp.py` & `agixt-1.1.77b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/llamacppapi.py` & `agixt-1.1.77b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/oobabooga.py` & `agixt-1.1.77b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/openai.py` & `agixt-1.1.77b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/palm.py` & `agixt-1.1.77b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/runpod.py` & `agixt-1.1.77b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/provider/transformer.py` & `agixt-1.1.77b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/starchat.sh` & `agixt-1.1.77b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/test-commands.ipynb` & `agixt-1.1.77b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/agixt/test-memory.ipynb` & `agixt-1.1.77b0/agixt/test-memory.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.76b0/docs/README.md` & `agixt-1.1.77b0/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,59 +60,50 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Quickstart with Docker
-Clone the repository and run the AGiXT Streamlit Web App.
-```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
-docker compose streamlit up
-```
-
-- Web Interface http://localhost:8501
-### Windows Docker Desktop (streamlit only example)
-- Container Name: AGiXT
-- Host Port: 8501:8501/tcp
+## Quickstart using docker
 
-### Alternative Docker Compose Profiles
-
-Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
-```
-docker compose all up
-```
+see [Quick Start](https://github.com/Josh-XT/AGiXT/edit/main/docs/1-Getting%20started/Quick%20Start.md)
 
-### Development using docker
+## Development using docker
 ```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+git clone https://github.com/Josh-XT/AGiXT
+cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
-## Local Development
+## Development using poetry
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
 `pip install poetry==1.5.0`
+
 Check if poetry is available via
+
 `poetry --version`
+
 or
+
 `python3 -m poetry --version`
+
 Adapt the following commands accordingly.
 
 #### Setup AGiXT
 ```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.0
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
+cd AGiXT
 poetry install --with gpt4free
 playwright install
-cd agixt
 ```
 
 #### Run Streamlit 
 `poetry run streamlit run Main.py`
 
 #### Run REST
 `poetry run uvicorn app:app --port 7437`
```

### Comparing `agixt-1.1.76b0/pyproject.toml` & `agixt-1.1.77b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.76-beta"
+version = "v1.1.77-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.76b0/PKG-INFO` & `agixt-1.1.77b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.76b0
+Version: 1.1.77b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
@@ -123,59 +123,50 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Quickstart with Docker
-Clone the repository and run the AGiXT Streamlit Web App.
-```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
-docker compose streamlit up
-```
-
-- Web Interface http://localhost:8501
-### Windows Docker Desktop (streamlit only example)
-- Container Name: AGiXT
-- Host Port: 8501:8501/tcp
+## Quickstart using docker
 
-### Alternative Docker Compose Profiles
-
-Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
-```
-docker compose all up
-```
+see [Quick Start](https://github.com/Josh-XT/AGiXT/edit/main/docs/1-Getting%20started/Quick%20Start.md)
 
-### Development using docker
+## Development using docker
 ```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+git clone https://github.com/Josh-XT/AGiXT
+cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
-## Local Development
+## Development using poetry
 
 Clone the repository for the AGiXT back end and start it.
 
 #### Install poetry
 `pip install poetry==1.5.0`
+
 Check if poetry is available via
+
 `poetry --version`
+
 or
+
 `python3 -m poetry --version`
+
 Adapt the following commands accordingly.
 
 #### Setup AGiXT
 ```
-git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.0
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
+cd AGiXT
 poetry install --with gpt4free
 playwright install
-cd agixt
 ```
 
 #### Run Streamlit 
 `poetry run streamlit run Main.py`
 
 #### Run REST
 `poetry run uvicorn app:app --port 7437`
```


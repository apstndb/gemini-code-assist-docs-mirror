---
name: documents/developers.google.com/gemini-code-assist/docs/configure-local-codebase-awareness
uri: https://developers.google.com/gemini-code-assist/docs/configure-local-codebase-awareness
title: Configure local codebase awareness
description: Describes how to configure local codebase awareness settings for Gemini Code Assist.
data_source: developers.google.com
---

Local codebase awareness improves the relevance of Gemini Code Assist responses through indexing and supporting techniques. Gemini Code Assist uses the current open file as context. An [agent](https://developers.google.com/gemini-code-assist/docs/agent-mode) is able to use tools to find and read the files it needs. You can also [specify files and folders in your workspace context](https://developers.google.com/gemini-code-assist/docs/chat-gemini#specify-context) .

By default, local codebase awareness is enabled, but you can [exclude files from Gemini Code Assist use](https://developers.google.com/gemini-code-assist/docs/create-aiexclude-file) , and VS Code users can disable local codebase awareness entirely. To disable local codebase awareness entirely, perform the following steps:

### VS Code

1.  In your IDE, navigate to **Settings** \> **Extensions** \> **Gemini Code Assist** .

2.  Search for the **Local Codebase Awareness** setting.

3.  Unselect the checkbox to disable local codebase awareness.

4.  Reload your IDE.

### IntelliJ

Local codebase awareness configuration settings aren't supported in Gemini Code Assist for IntelliJ and other JetBrains IDEs.

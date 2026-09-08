---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/gemini-3
uri: https://docs.cloud.google.com/gemini/docs/codeassist/gemini-3
title: Gemini 3 in Gemini Code Assist
description: Gemini 3 considerations with Gemini Code Assist.
data_source: docs.cloud.google.com
---

> **Preview**
> 
> This feature is subject to the "Pre-GA Offerings Terms" in the General Service Terms section of the [Service Specific Terms](https://docs.cloud.google.com/terms/service-terms#1) . Pre-GA features are available "as is" and might have limited support. For more information, see the [launch stage descriptions](https://cloud.google.com/products/#product-launch-stages) .

Gemini 3.1 Pro is available as public preview and Gemini 3.5 Flash is generally available to Gemini Code Assist users in VS Code and IntelliJ. You can use these models for [agent mode](https://docs.cloud.google.com/gemini/docs/codeassist/agent-mode) , [chat](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini) , and [code generation](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#generate_code_with_prompts) . Responses generated with Gemini 3 include a label identifying the model.

## Gemini 3 availability

| License or subscription                                                                        | Gemini 3 availability                                                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Gemini Code Assist Enterprise](https://docs.cloud.google.com/gemini/docs/codeassist/overview) | Gemini 3.1 Pro is **available to users** in VS Code and IntelliJ whose administrator has configured the [Preview release channel](https://docs.cloud.google.com/gemini/docs/codeassist/configure-release-channels) . Gemini 3.5 Flash is **available to all users** . |
| [Gemini Code Assist Standard](https://docs.cloud.google.com/gemini/docs/codeassist/overview)   | Gemini 3.1 Pro **available to users** in VS Code and IntelliJ whose administrator has configured the [Preview release channel](https://docs.cloud.google.com/gemini/docs/codeassist/configure-release-channels) . Gemini 3.5 Flash is **available to all users** .    |

## Use Gemini 3 in VS Code

If Gemini 3 is available to you, it will automatically be selected for chat and code generation. You can use the model selector in chat to select a different model. You can't select a different model in agent mode, as Gemini CLI automatically selects the model.

## Use Gemini 3 in IntelliJ

If Gemini 3 is available to you, it will automatically be selected for agent mode, chat and code generation. You can use the model selector in chat to select a different model, including in agent mode.

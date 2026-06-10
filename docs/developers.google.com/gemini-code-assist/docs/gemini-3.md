---
name: documents/developers.google.com/gemini-code-assist/docs/gemini-3
uri: https://developers.google.com/gemini-code-assist/docs/gemini-3
title: Gemini 3 in Gemini Code Assist
description: Gemini 3 considerations with Gemini Code Assist.
data_source: developers.google.com
---

> **Preview**
> 
> This product or feature is in preview. Products and features that are in preview are available "as is".

Gemini 3.1 Pro is available as public preview and Gemini 3.5 Flash is generally available to Gemini Code Assist users in VS Code and IntelliJ. You can use these models for [agent mode](https://developers.google.com/gemini-code-assist/docs/agent-mode) , [chat](https://developers.google.com/gemini-code-assist/docs/chat-gemini) , and [code generation](https://developers.google.com/gemini-code-assist/docs/write-code-gemini#generate_code_with_prompts) . Responses generated with Gemini 3 include a label identifying the model.

## Gemini 3 availability

| License or subscription                                                                              | Gemini 3 availability                                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Google AI Ultra](https://one.google.com/about/google-ai-plans/)                                     | **Available to all users** in VS Code and IntelliJ                                                                                                                                                                                                                     |
| [Google AI Pro](https://one.google.com/about/google-ai-plans/)                                       | **Available to all users** in VS Code and IntelliJ                                                                                                                                                                                                                     |
| [Gemini Code Assist Enterprise](https://developers.google.com/gemini-code-assist/docs/overview)      | Gemini 3.1 Pro is **available to users** in VS Code and IntelliJ whose administrator has configured the [Preview release channel](https://developers.google.com/gemini-code-assist/docs/configure-release-channels) . Gemini 3.5 Flash is **available to all users** . |
| [Gemini Code Assist Standard](https://developers.google.com/gemini-code-assist/docs/overview)        | Gemini 3.1 Pro **available to users** in VS Code and IntelliJ whose administrator has configured the [Preview release channel](https://developers.google.com/gemini-code-assist/docs/configure-release-channels) . Gemini 3.5 Flash is **available to all users** .    |
| [Gemini Code Assist for individuals](https://developers.google.com/gemini-code-assist/docs/overview) | **Available to select users** from the waitlist in VS Code and IntelliJ.                                                                                                                                                                                               |

## Use Gemini 3 in VS Code

If Gemini 3 is available to you, it will automatically be selected for chat and code generation. You can use the model selector in chat to select a different model. You can't select a different model in agent mode, as Gemini CLI automatically selects the model.

## Use Gemini 3 in IntelliJ

If Gemini 3 is available to you, it will automatically be selected for agent mode, chat and code generation. You can use the model selector in chat to select a different model, including in agent mode.

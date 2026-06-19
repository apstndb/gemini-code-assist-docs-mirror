---
name: documents/developers.google.com/gemini-code-assist/docs/use-pre-release-features-gemini-code-assist
uri: https://developers.google.com/gemini-code-assist/docs/use-pre-release-features-gemini-code-assist
title: Use pre-release features in Gemini Code Assist for VS Code
description: Try out pre-release features of Gemini Code Assist with the insiders build.
data_source: developers.google.com
---

This page describes how to use pre-release features of Gemini Code Assist for VS Code on the insiders release channel.

Pre-release builds can include bug fixes and features still in development that might be removed in a future release.

## Before you begin

[Set up Gemini Code Assist Standard or Enterprise](https://developers.google.com/gemini-code-assist/docs/set-up-gemini-standard-enterprise) .

## Use the insiders build

To configure the update channel, follow these steps:

1.  In your IDE, open the **Command palette** ( `Cmd` + `Shift` + `P` ) and then select **Open User Settings JSON** .
2.  Add the following line to your user settings JSON: `"geminicodeassist.updateChannel": "Insiders",`
3.  Save your user settings.

You are prompted to reload your window to use the latest insiders build.

## Use the standard release channel

To use the standard release channel instead of the insiders build, follow these steps:

1.  In your IDE, open the **Command palette** ( `Cmd` + `Shift` + `P` ) and then select **Open User Settings JSON** .
2.  Comment out or remove the following line of your user settings JSON: `"geminicodeassist.updateChannel": "Insiders",`
3.  Save your user settings.

You are prompted to reload your window to use the standard release channel.

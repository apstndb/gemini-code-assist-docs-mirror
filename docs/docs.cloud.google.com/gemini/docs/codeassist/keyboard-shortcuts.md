---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/keyboard-shortcuts
uri: https://docs.cloud.google.com/gemini/docs/codeassist/keyboard-shortcuts
title: Keyboard shortcuts for Gemini Code Assist features
description: Outlines and describes the keyboard shortcuts for Gemini Code Assist in VS Code and JetBrains IDEs.
data_source: docs.cloud.google.com
---

Gemini Code Assist provides AI-powered assistance to help your development team build, deploy, and operate applications throughout the software development lifecycle.

This page provides an overview of the keyboard shortcuts you can use in VS Code, IntelliJ, and [other supported JetBrains IDEs](https://docs.cloud.google.com/gemini/docs/codeassist/supported-languages#supported_ides) , for Windows, Linux, and macOS users.

## Code generation shortcuts

### VS Code

| Action                                                                                                                                                     | Keyboard shortcut (Windows/Linux)        | Keyboard shortcut (macOS)                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------|------------------------------------------|
| Navigate to chat interface                                                                                                                                 | <span class="kbd"> Alt+G </span>         | <span class="kbd"> Option+G </span>      |
| [Add selected code snippet to Gemini Chat context](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini#add_selected_code_snippets_to_context) | <span class="kbd"> Control+Alt+X </span> | <span class="kbd"> Command+Alt+X </span> |
| [Finish code changes in a file](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#finish-changes)                                     | <span class="kbd"> Alt+F </span>         | <span class="kbd"> Option+F </span>      |

### IntelliJ

| Action                                                                                                                                                     | Keyboard shortcut (Windows/Linux)        | Keyboard shortcut (macOS)                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------|------------------------------------------|
| Generate code inline of a code file                                                                                                                        | <span class="kbd"> Control+G </span>     | <span class="kbd"> Option+G </span>      |
| Open In-Editor prompt                                                                                                                                      | <span class="kbd"> Control+\\ </span>    | <span class="kbd"> Command+\\ </span>    |
| [Add selected code snippet to Gemini Chat context](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini#add_selected_code_snippets_to_context) | <span class="kbd"> Control+Alt+X </span> | <span class="kbd"> Command+Alt+X </span> |
| [Finish code changes in a file](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#finish-changes)                                     | <span class="kbd"> Alt+F </span>         | <span class="kbd"> Option+F </span>      |

## Terminal shortcuts

### VS Code

| Action                                                                                                                                                                                      | Keyboard shortcut (Windows/Linux)        | Keyboard shortcut (macOS)                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------|------------------------------------------|
| [Add the current highlighted terminal content to the Gemini Chat context](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini#prompt_with_selected_terminal_output_using_chat) | <span class="kbd"> Control+Alt+X </span> | <span class="kbd"> Command+Alt+X </span> |

### IntelliJ

There aren't any default terminal shortcuts for Gemini Code Assist for IntelliJ and other supported JetBrains IDEs at this time.

## Chat shortcuts

### VS Code

| Action                                                                                          | Keyboard shortcut (Windows/Linux)         | Keyboard shortcut (macOS)                 |
|-------------------------------------------------------------------------------------------------|-------------------------------------------|-------------------------------------------|
| Cycle through prior chat prompts                                                                | <span class="kbd"> Up/down arrows </span> | <span class="kbd"> Up/down arrows </span> |
| [Generate an outline](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini#outline) | <span class="kbd"> Alt+O </span>          | <span class="kbd"> Option+O </span>       |

### IntelliJ

| Action                                                                                          | Keyboard shortcut (Windows/Linux)                 | Keyboard shortcut (macOS)                         |
|-------------------------------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------------------|
| Cycle through prior chat prompts                                                                | <span class="kbd"> Up/down arrows </span>         | <span class="kbd"> Up/down arrows </span>         |
| New chat                                                                                        | <span class="kbd"> Control+Alt+Windows+Up </span> | <span class="kbd"> Control+Alt+Command+Up </span> |
| [Generate an outline](https://docs.cloud.google.com/gemini/docs/codeassist/chat-gemini#outline) | <span class="kbd"> Alt+O </span>                  | <span class="kbd"> Option+O </span>               |

## Edit keyboard shortcuts

If you prefer to change any of the default Gemini Code Assist shortcuts, you can do so by following these steps:

### VS Code

1.  In your IDE, click **File** (for Windows and Linux) or **Code** (for macOS), and then navigate to **Settings** \> **Keyboard Shortcuts** .

2.  In the list of keyboard shortcuts, scroll until you find the shortcut that you want to change. For example: **Gemini Code Assist: Generate code** .

3.  Click the shortcut that you want to change (for example, **Gemini Code Assist: Generate Code** ), and then click edit **Change Keybinding** .

4.  In the dialog that appears, enter your own shortcut.

5.  Press <span class="kbd"> Enter </span> (for Windows and Linux) or <span class="kbd"> Return </span> (for macOS).

You can now use your newly assigned keyboard shortcut in your IDE.

To learn more about changing shortcuts in your IDE, see [Keybindings for Visual Studio Code](https://code.visualstudio.com/docs/getstarted/keybindings) .

### IntelliJ

1.  Navigate to settings **IDE and Project Settings** \> **Settings** \> **Keymap** \> **Plugins** \> **Gemini Code Assist** .

2.  Right-click the shortcut you want to change (for example, **Generate Code** ) and select **Add Keyboard Shortcut** .

3.  Enter your preferred keyboard shortcut and then click **OK** .

4.  Right-click the shortcut again and remove the shortcut. For example, right-click **Generate code** and select **Remove <span class="kbd"> Alt+G </span>** (for Windows and Linux), or **Remove <span class="kbd"> Option+G </span>** (for macOS).

You can now use your new keyboard shortcut in your IDE.

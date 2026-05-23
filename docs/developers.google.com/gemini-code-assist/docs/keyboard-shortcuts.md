---
name: documents/developers.google.com/gemini-code-assist/docs/keyboard-shortcuts
uri: https://developers.google.com/gemini-code-assist/docs/keyboard-shortcuts
title: Keyboard shortcuts for Gemini Code Assist features
description: Outlines and describes the keyboard shortcuts for Gemini Code Assist in VS Code and JetBrains IDEs.
data_source: developers.google.com
---

Gemini Code Assist provides AI-powered assistance to help your development team build, deploy, and operate applications throughout the software development lifecycle.

This page provides an overview of the keyboard shortcuts you can use in VS Code, IntelliJ, and [other supported JetBrains IDEs](https://developers.google.com/gemini-code-assist/docs/supported-languages#supported_ides) , for Windows, Linux, and macOS users.

## Code generation shortcuts

### VS Code

| Action                                                                                                                                                      | Keyboard shortcut (Windows/Linux) | Keyboard shortcut (macOS) |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- | ------------------------- |
| Navigate to chat interface                                                                                                                                  | Alt+G                             | Option+G                  |
| [Add selected code snippet to Gemini Chat context](https://developers.google.com/gemini-code-assist/docs/chat-gemini#add_selected_code_snippets_to_context) | Control+Alt+X                     | Command+Alt+X             |
| [Finish code changes in a file](https://developers.google.com/gemini-code-assist/docs/write-code-gemini#finish-changes)                                     | Alt+F                             | Option+F                  |

### IntelliJ

| Action                                                                                                                                                      | Keyboard shortcut (Windows/Linux) | Keyboard shortcut (macOS) |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- | ------------------------- |
| Generate code inline of a code file                                                                                                                         | Control+G                         | Option+G                  |
| Open In-Editor prompt                                                                                                                                       | Control+\\                        | Command+\\                |
| [Add selected code snippet to Gemini Chat context](https://developers.google.com/gemini-code-assist/docs/chat-gemini#add_selected_code_snippets_to_context) | Control+Alt+X                     | Command+Alt+X             |
| [Finish code changes in a file](https://developers.google.com/gemini-code-assist/docs/write-code-gemini#finish-changes)                                     | Alt+F                             | Option+F                  |

## Terminal shortcuts

### VS Code

| Action                                                                                                                                                                                       | Keyboard shortcut (Windows/Linux) | Keyboard shortcut (macOS) |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- | ------------------------- |
| [Add the current highlighted terminal content to the Gemini Chat context](https://developers.google.com/gemini-code-assist/docs/chat-gemini#prompt_with_selected_terminal_output_using_chat) | Control+Alt+X                     | Command+Alt+X             |

### IntelliJ

There aren't any default terminal shortcuts for Gemini Code Assist for IntelliJ and other supported JetBrains IDEs at this time.

## Chat shortcuts

### VS Code

| Action                                                                                           | Keyboard shortcut (Windows/Linux) | Keyboard shortcut (macOS) |
| ------------------------------------------------------------------------------------------------ | --------------------------------- | ------------------------- |
| Cycle through prior chat prompts                                                                 | Up/down arrows                    | Up/down arrows            |
| [Generate an outline](https://developers.google.com/gemini-code-assist/docs/chat-gemini#outline) | Alt+O                             | Option+O                  |

### IntelliJ

| Action                                                                                           | Keyboard shortcut (Windows/Linux) | Keyboard shortcut (macOS) |
| ------------------------------------------------------------------------------------------------ | --------------------------------- | ------------------------- |
| Cycle through prior chat prompts                                                                 | Up/down arrows                    | Up/down arrows            |
| New chat                                                                                         | Control+Alt+Windows+Up            | Control+Alt+Command+Up    |
| [Generate an outline](https://developers.google.com/gemini-code-assist/docs/chat-gemini#outline) | Alt+O                             | Option+O                  |

## Edit keyboard shortcuts

If you prefer to change any of the default Gemini Code Assist shortcuts, you can do so by following these steps:

### VS Code

1.  In your IDE, click **File** (for Windows and Linux) or **Code** (for macOS), and then navigate to **Settings** \> **Keyboard Shortcuts** .

2.  In the list of keyboard shortcuts, scroll until you find the shortcut that you want to change. For example: **Gemini Code Assist: Generate code** .

3.  Click the shortcut that you want to change (for example, **Gemini Code Assist: Generate Code** ), and then click edit **Change Keybinding** .

4.  In the dialog that appears, enter your own shortcut.

5.  Press Enter (for Windows and Linux) or Return (for macOS).
    
    You can now use your newly assigned keyboard shortcut in your IDE.

To learn more about changing shortcuts in your IDE, see [Keybindings for Visual Studio Code](https://code.visualstudio.com/docs/getstarted/keybindings) .

### IntelliJ

1.  Navigate to settings **IDE and Project Settings** \> **Settings** \> **Keymap** \> **Plugins** \> **Gemini Code Assist** .

2.  Right-click the shortcut you want to change (for example, **Generate Code** ) and select **Add Keyboard Shortcut** .

3.  Enter your preferred keyboard shortcut and then click **OK** .

4.  Right-click the shortcut again and remove the shortcut. For example, right-click **Generate code** and select **Remove Alt+G** (for Windows and Linux), or **Remove Option+G** (for macOS).

You can now use your new keyboard shortcut in your IDE.

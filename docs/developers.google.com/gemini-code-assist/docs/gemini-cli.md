---
name: documents/developers.google.com/gemini-code-assist/docs/gemini-cli
uri: https://developers.google.com/gemini-code-assist/docs/gemini-cli
title: Gemini CLI
description: Learn about the Gemini CLI
data_source: developers.google.com
---

The [Gemini command line interface (CLI)](https://geminicli.com/docs/) is an open source AI agent that provides access to Gemini directly in your terminal. The Gemini CLI uses a reason and act (ReAct) loop with your built-in tools and local or remote MCP servers to complete complex use cases like fixing bugs, creating new features, and improving test coverage. While the Gemini CLI excels at coding, it's also a versatile local utility that you can use for a wide range of tasks, from content generation and problem solving to deep research and task management.

Each [Gemini Code Assist edition](https://developers.google.com/gemini-code-assist/docs/overview) provides [quotas](https://geminicli.com/docs/quota-and-pricing/) for using the Gemini CLI. Note that these quotas are shared between Gemini CLI and [Gemini Code Assist agent mode](https://developers.google.com/gemini-code-assist/docs/agent-mode) . Gemini CLI also supports using a Gemini API key to [pay as you go](https://geminicli.com/docs/quota-and-pricing/#pay-as-you-go) .

The Gemini CLI is available without additional setup in [Cloud Shell](https://docs.cloud.google.com/shell/docs/use-cloud-shell-terminal) . To get started with Gemini CLI in other environments, see the [Gemini CLI documentation](https://geminicli.com/docs/) .

### Privacy

For users of Gemini Code Assist Standard and Enterprise, the data protection and privacy practices described in [Security, privacy, and compliance for Gemini Code Assist Standard and Enterprise](https://docs.cloud.google.com/gemini/docs/codeassist/security-privacy-compliance) also apply to Gemini CLI.

For users of Gemini Code Assist for individuals, the data protection and privacy practices described in the [Gemini Code Assist Privacy Notice for individuals](https://developers.google.com/gemini-code-assist/resources/privacy-notice-gemini-code-assist-individuals) also apply to Gemini CLI.

## Gemini Code Assist agent mode (Preview)

[Gemini Code Assist agent mode](https://developers.google.com/gemini-code-assist/docs/agent-mode) in VS Code is powered by Gemini CLI. A subset of Gemini CLI functionality is available directly in the Gemini Code Assist chat within VS Code.

The following Gemini CLI features are available in Gemini Code Assist for VS Code.

  - [Model Context Protocol (MCP) servers](https://developers.google.com/gemini-code-assist/docs/use-agentic-chat-pair-programmer#configure-mcp-servers)
  - Gemini CLI [commands](https://geminicli.com/docs/cli/commands/) : `/memory` , `/stats` , `/tools` , `/mcp`
  - [Yolo mode](https://developers.google.com/gemini-code-assist/docs/use-agentic-chat-pair-programmer#yolo-mode)
  - built-in tools like grep, terminal, file read or file write
  - Web search
  - Web fetch

## What's next

  - Read more about [Gemini CLI documentation](https://geminicli.com/docs/) .
  - Download and [install Gemini CLI](https://geminicli.com/docs/get-started/installation/) .

---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/overview
uri: https://docs.cloud.google.com/gemini/docs/codeassist/overview
title: Gemini Code Assist Standard and Enterprise overview
description: Get AI-powered assistance from Gemini to help your development team build, deploy, and operate applications.
data_source: docs.cloud.google.com
---

> **Note:** We have unified our tools into a single, multi-agent platform called Antigravity, with Antigravity CLI now available. Starting June 18, 2026, Gemini Code Assist IDE Extensions and Gemini CLI stopped serving requests for the Gemini Code Assist for individuals, Google AI Pro, and Google AI Ultra tiers. Affected users should migrate to Antigravity and Antigravity CLI. To learn more, see the [deprecation page](https://developers.google.com/gemini-code-assist/docs/deprecations/code-assist-individuals) .

Gemini Code Assist Standard and Enterprise offer AI-powered assistance to help your development team build, deploy, and operate applications throughout the software development lifecycle.

For information about Gemini Code Assist Standard and Enterprise pricing and quotas, see [Gemini Code Assist pricing](https://cloud.google.com/products/gemini/pricing) and [Gemini Code Assist quotas](https://docs.cloud.google.com/gemini/docs/quotas) .

You can use Gemini Code Assist in [supported IDEs](https://docs.cloud.google.com/gemini/docs/codeassist/supported-languages#supported_ides) , such as VS Code, JetBrains IDEs, or Android Studio, for AI-powered coding assistance in [many popular languages](https://docs.cloud.google.com/gemini/docs/codeassist/supported-languages) . You can get code completions as you write your code, generate full functions or code blocks from comments, generate unit tests, and get help with debugging, understanding, and documenting your code.

Gemini Code Assist provides contextualized responses to your prompts, including [source citations](https://docs.cloud.google.com/gemini/docs/discover/works#how-when-gemini-cites-sources) Gemini Code Assist used to generate its responses.

The Gemini large language models (LLMs) that are used by Gemini Code Assist are trained on datasets of publicly available code, Google Cloud-specific material, and other relevant technical information in addition to the datasets used to train the Gemini [foundation models](https://storage.googleapis.com/deepmind-media/gemini/gemini_1_report.pdf) . Models are trained so that Gemini Code Assist responses are as useful to Gemini Code Assist users as possible.

As an early-stage technology, Gemini Code Assist can generate output that seems plausible but is factually incorrect. We recommend that you validate all output from Gemini Code Assist before you use it. For more information, see [Gemini products in Google Cloud and responsible AI](https://docs.cloud.google.com/gemini/docs/discover/responsible-ai) .

Gemini Code Assist provides citation information when it directly quotes at length from another source, such as existing open source code. For more information, see [How and when Gemini cites sources](https://docs.cloud.google.com/gemini/docs/discover/works#how-when-gemini-cites-sources) .

## Gemini Code Assist Standard and Enterprise editions overview

The following section compares the Gemini Code Assist Standard and Enterprise editions.

The Standard edition offers AI coding assistance, with enterprise-grade security, for building and running applications. The Enterprise edition offers all of the [supported features](https://docs.cloud.google.com/gemini/docs/codeassist/overview#supported-features) in the Standard edition, but you can also customize it based on your private source code repositories, and it's integrated with additional Google Cloud services for building applications across a broader tech stack.

The following table helps you to decide which edition aligns best with your organization's development goals by highlighting the intended audience and the benefits for each edition:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th>Gemini Code Assist Standard</th>
<th>Gemini Code Assist Enterprise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Intended audience</td>
<td><ul>
<li>Customers with basic coding needs.</li>
<li>Organizations with strict data security and compliance requirements.</li>
</ul></td>
<td><ul>
<li>Large enterprises with complex software development processes.</li>
<li>Customers wanting to have AI response customized based on private source code repositories to accelerate development based on organizational best practices.</li>
<li>Customers needing AI-powered application development assistant across an expanding list of Google Cloud services.</li>
</ul></td>
</tr>
<tr class="even">
<td>Benefits</td>
<td><ul>
<li>Code completion and generation for popular programming languages, and available across some Google Cloud services.</li>
<li>AI-powered chat support.</li>
<li>Simplified user interface and integration with IDEs.</li>
<li>Local codebase awareness in your IDE: Use the power of Gemini's large context window for in-depth local codebase understanding.</li>
<li>Enterprise-grade security: Robust data governance, secure infrastructure, and indemnification for code suggestions.</li>
<li>Extended integrations: Gemini Code Assist Standard provides AI assistance in Firebase, Colab Enterprise, BigQuery data insights, Cloud Run, and Database Studio.</li>
</ul></td>
<td>All of the benefits mentioned for Gemini Code Assist Standard, with the addition of the following:
<ul>
<li><a href="https://docs.cloud.google.com/gemini/docs/codeassist/code-customization-overview">Code customization</a> : Your organization can augment the model with your private codebases for tailored suggestions.</li>
<li>Extended integrations: Gemini Code Assist Enterprise provides AI assistance across Google Cloud like Apigee, Application Integration, and Gemini Cloud Assist, empowering cloud teams to build, design and operate, and optimize their applications and infrastructure more effectively on Google Cloud.</li>
</ul></td>
</tr>
</tbody>
</table>

For a comparison of each edition's features, see [Supported features](https://docs.cloud.google.com/gemini/docs/codeassist/overview#supported-features) .

## Supported features for Gemini Code Assist Standard and Enterprise

The following sections show the types of generative AI assistance that are available in Gemini Code Assist Standard and Enterprise.

### Code assistance and chat

The following table shows the types of generative AI assistance that are available in [supported IDEs](https://docs.cloud.google.com/gemini/docs/codeassist/supported-languages#supported_ides) :

AI coding assistance

Gemini Code Assist Standard

Gemini Code Assist Enterprise

Code completion and generation in your IDE project in the following IDEs:

  - [Cloud Shell Editor](https://docs.cloud.google.com/code/docs/shell/write-code-gemini#get_inline_suggestions_while_you_code)
  - [Cloud Workstations](https://docs.cloud.google.com/workstations/docs/write-code-gemini#get_inline_suggestions_while_you_code)
  - [JetBrains IDEs (such as IntelliJ and PyCharm)](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#get_code_completions)
  - [VS Code](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#get_code_completions)
  - [Android Studio](https://developer.android.com/studio/gemini/overview)

Conversational assistant in your IDE [using your opened files' context](https://docs.cloud.google.com/gemini/docs/discover/works#gemini-code-assist)

Multi-IDE support (VS Code, [JetBrains IDEs such as IntelliJ and PyCharm](https://docs.cloud.google.com/gemini/docs/codeassist/supported-languages#supported_ides) , Cloud Workstations)

Agentic chat

Prompt Gemini to complete complex, multi-step tasks that use system tools and Model Context Protocol (MCP) servers. For more information, see [Use the Gemini Code Assist agent mode](https://docs.cloud.google.com/gemini/docs/codeassist/use-agentic-chat-pair-programmer) .

Gemini CLI quota

[Quota](https://docs.cloud.google.com/gemini/docs/quotas) for using [Gemini CLI](https://docs.cloud.google.com/gemini/docs/codeassist/gemini-cli) .

Smart actions and commands

Initiate smart actions by right-clicking selected code ( [VS Code](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#use_smart_actions) , [JetBrains IDEs such as IntelliJ and PyCharm](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#use_smart_actions) , [Cloud Shell Editor](https://docs.cloud.google.com/code/docs/shell/write-code-gemini#use_smart_actions) , [Cloud Workstations](https://docs.cloud.google.com/workstations/docs/write-code-gemini#use_smart_actions) , and [Android Studio](https://developer.android.com/studio/gemini/overview) ). Initiate smart commands with the slash `/` on the quick pick bar either with or without selected code ( [VS Code](https://docs.cloud.google.com/gemini/docs/codeassist/write-code-gemini#generate_code_with_prompts) , [Cloud Shell Editor](https://docs.cloud.google.com/code/docs/shell/write-code-gemini#use_smart_commands) , and [Cloud Workstations](https://docs.cloud.google.com/workstations/docs/write-code-gemini#use_smart_commands) ).

Intellectual property and compliance

[Source citations in your IDE and the Google Cloud console](https://docs.cloud.google.com/gemini/docs/discover/works)

[IP indemnification](https://docs.cloud.google.com/gemini/docs/discover/works#how-gemini-protects)

[VPC-SC and Private Google Access](https://docs.cloud.google.com/gemini/docs/configure-vpc-service-controls)

Enterprise knowledge

[Customized code suggestions from your code bases in GitHub, GitLab, and Bitbucket in your IDE](https://docs.cloud.google.com/gemini/docs/codeassist/code-customization-overview)

### Additional features outside the IDE

The following sections detail additional features available with the Gemini Code Assist Standard and Enterprise editions that go beyond assistance in your IDE.

#### Gemini Cloud Assist

The following table shows the types of generative AI assistance in [Gemini Cloud Assist](https://docs.cloud.google.com/cloud-assist/overview) in the Google Cloud console:

| Gemini Cloud Assist assistance                                                                                                                                                                            | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- | ----------------------------- |
| [Gemini Cloud Assist features](https://docs.cloud.google.com/cloud-assist/overview#ai-assistance) (including features available to all Google users and available to Gemini Code Assist Enterprise users) |                             |                               |

#### Gemini in Apigee

The following table shows the types of generative AI assistance with API development in [Apigee](https://docs.cloud.google.com/apigee/docs) (IDE and the Google Cloud console):

| Gemini Code Assist for API management                                                                                                                                                                                                                                                     | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- | ----------------------------- |
| [Create or edit OpenAPI specification](https://docs.cloud.google.com/apigee/docs/api-platform/local-development/vscode/develop-design-edit-apis#designing-apis-with-gemini-code-assist) using natural language prompts.                                                                   |                             |                               |
| [Enterprise context](https://docs.cloud.google.com/apigee/docs/api-platform/local-development/vscode/develop-design-edit-apis#designing-apis-with-gemini-code-assist) used when creating or updating API specifications.                                                                  |                             |                               |
| [Gemini Code Assist code explained for Apigee policies.](https://docs.cloud.google.com/apigee/docs/api-platform/develop/attaching-and-configuring-policies-management-ui#use-gemini-code-assist-code-explain) ( [Preview](https://docs.cloud.google.com/products#product-launch-stages) ) |                             |                               |

#### Gemini in Application Integration

The following table shows the types of generative AI assistance in [Application Integration](https://docs.cloud.google.com/application-integration/docs/overview) in the Google Cloud console:

| Integration creation assist                                                                                                                                                                    | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- | ----------------------------- |
| [AI-assisted visual editor for automation flow generation](https://docs.cloud.google.com/application-integration/docs/build-integrations-gemini#create-an-integration)                         |                             |                               |
| [Enterprise context embedded AI-assisted automation authoring](https://docs.cloud.google.com/application-integration/docs/build-integrations-gemini#contextual-recommendations)                |                             |                               |
| [Generative AI Automation flow documentation generation and refinement](https://docs.cloud.google.com/application-integration/docs/build-integrations-gemini#generate-integration-description) |                             |                               |

#### Gemini in BigQuery features with Gemini Code Assist

The following table shows the types of generative AI assistance for BigQuery in [BigQuery Studio](https://docs.cloud.google.com/bigquery/docs/query-overview#bigquery-studio) :

| Data insights                                                                                                                                                                            | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- | ----------------------------- |
| [Data insights](https://docs.cloud.google.com/bigquery/docs/data-insights#insights-bigquery-table) provides an insightful library of queries generated from the metadata of your tables. |                             |                               |

#### Gemini in Colab Enterprise

The following table shows the types of generative AI assistance for code in [Colab Enterprise](https://docs.cloud.google.com/colab/docs/introduction) :

| Notebook code assist                                                                                              | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| ----------------------------------------------------------------------------------------------------------------- | --------------------------- | ----------------------------- |
| [Python code generation and completion in notebook](https://docs.cloud.google.com/colab/docs/use-code-completion) |                             |                               |

#### Gemini in databases

The following table shows the types of generative AI assistance for coding in databases:

| Generate SQL queries                                  | Gemini Code Assist Standard | Gemini Code Assist Enterprise |
| ----------------------------------------------------- | --------------------------- | ----------------------------- |
| Write in natural language to generate SQL statements. |                             |                               |
| Get contextual code that works with your schema.      |                             |                               |
| Optimize and explain existing queries.                |                             |                               |

#### Gemini in Firebase

The following table shows the types of generative AI assistance for application development provided by [Gemini in Firebase](https://firebase.google.com/docs/gemini-in-firebase) :

Chat AI assistance in the Firebase console

Gemini Code Assist Standard

Gemini Code Assist Enterprise

Use deep knowledge, best practices, and troubleshooting expertise for Firebase products and services.

Generate, refactor, and debug sample code for Firebase with natural language in chat.

Use natural language prompts to explain, generate, and transform code.

App quality analysis

Summarize app crashes and provide insights and troubleshooting steps to help developers investigate and resolve app quality issues.

Analyze existing code, identify potential issues, and suggest improvements.

Firebase Cloud Messaging and In-App Messaging campaign summarization and insights

Summarize and analyze your messaging campaigns, providing actionable recommendations to improve performance.

Firebase Data Connect schema generation and data exploration

Generate database schemas with natural language.

Generate GraphQL queries and mutations with natural language.

Contextual awareness

Use project and application context to guide conversational assistance, troubleshooting, and app quality analysis.

## Set up Gemini Code Assist

For detailed setup steps, see [Set up Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini) .

## Interact with Gemini Code Assist in your IDE

After you [set up Gemini Code Assist Standard or Enterprise for a Google Cloud project](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini) , and install the Gemini Code Assist extension in your IDE ( [VS Code](https://marketplace.visualstudio.com/items?itemName=GoogleCloudTools.cloudcode) or [supported JetBrains IDE](https://plugins.jetbrains.com/plugin/24198-gemini-code-assist) ), you can ask for assistance in the following ways:

  - Receive code completions or generate code directly in the code editor.

  - Click spark **Gemini** in the IDE to display the conversational assistant. You can ask questions or select code in your editor and enter prompts such as the following:
    
      - `Write unit tests for my code.`
      - `Help me debug my code.`
      - `Make my code more readable.`

For more information, see [Use Gemini Code Assist in your IDE](https://docs.cloud.google.com/gemini/docs/codeassist/use-in-ide) .

## What's next

  - Learn how to [use Gemini Code Assist in your IDE](https://docs.cloud.google.com/gemini/docs/codeassist/use-in-ide) .
  - Learn [how Gemini Code Assist uses your data](https://docs.cloud.google.com/gemini/docs/discover/data-governance) .
  - Learn about [Gemini Code Assist pricing](https://cloud.google.com/products/gemini/pricing) .
  - Learn about the [security, privacy, and compliance of Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/security-privacy-compliance) .

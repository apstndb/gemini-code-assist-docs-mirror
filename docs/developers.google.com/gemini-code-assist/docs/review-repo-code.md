---
name: documents/developers.google.com/gemini-code-assist/docs/review-repo-code
uri: https://developers.google.com/gemini-code-assist/docs/review-repo-code
title: Review GitHub code using Gemini Code Assist
description: Review pull requests using Gemini Code Assist.
data_source: developers.google.com
---

Gemini Code Assist on GitHub brings the power of Gemini to the pull request process by acting as a code reviewer. Gemini Code Assist on GitHub uses a Gemini-powered agent that automatically summarizes pull requests and provides in-depth code reviews, speeding up reviews and increasing the quality of code.

Once you've [set up Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) , you can [invoke Gemini Code Assist](https://developers.google.com/gemini-code-assist/docs/use-code-assist-github) at any stage of the pull request to review the code. You can interact with Gemini Code Assist in the pull request comments directly by:

  - Asking clarifying questions on the review that Gemini Code Assist creates.
  - Prompting Gemini Code Assist by adding the `/gemini` tag to your comments to ask questions in the context of the pull request.

Gemini Code Assist will automatically retrieve helpful information from the repository and pull request to perform its tasks.

This document is intended for developers of all skill levels. It assumes that you have a working knowledge of GitHub.

## Consumer version and enterprise version

> **Important:** The enterprise version of Gemini Code Assist on GitHub is a separate and distinct product from [Gemini Code Assist Enterprise](https://developers.google.com/gemini-code-assist/docs/overview#supported-features) .

Gemini Code Assist on GitHub is available in an enterprise version, which you [install](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) through Google Cloud. A consumer version also exists; however, serving requests to the consumer version is being discontinued, and you shouldn't install this version.

The following table summarizes the differences between the consumer version and enterprise version:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th style="text-align: center;">Consumer version</th>
<th style="text-align: center;">Enterprise version <a href="https://cloud.google.com/products#product-launch-stages">(Preview)</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Terms of service</td>
<td style="text-align: center;"><a href="https://policies.google.com/terms">Google terms of service</a></td>
<td style="text-align: center;"><a href="https://cloud.google.com/terms/">Google Cloud terms of service</a></td>
</tr>
<tr class="even">
<td><a href="https://developers.google.com/gemini-code-assist/resources/quotas#github">Quotas</a></td>
<td style="text-align: center;">33 pull requests per day</td>
<td style="text-align: center;">100+ pull requests per day</td>
</tr>
<tr class="odd">
<td><a href="https://developers.google.com/gemini-code-assist/docs/customize-repo-review">Managing configurations</a></td>
<td style="text-align: center;"><p>Per-repository within GitHub</p>
<p>All repositories associated with an account using the <a href="https://codeassist.google/code-review">settings page</a></p></td>
<td style="text-align: center;"><p>Per-repository within GitHub</p>
<p>Across multiple repositories using <a href="https://console.cloud.google.com/gemini-code-assist/agents-tools">Google Cloud</a></p></td>
</tr>
<tr class="even">
<td><a href="https://developers.google.com/gemini-code-assist/docs/code-review-style-guide">Adding a style guide</a></td>
<td style="text-align: center;">Per-repository within GitHub</td>
<td style="text-align: center;"><p>Per-repository within GitHub</p>
<p>Across multiple repositories using <a href="https://console.cloud.google.com/gemini-code-assist/agents-tools">Google Cloud</a></p></td>
</tr>
<tr class="odd">
<td>GitHub support</td>
<td style="text-align: center;"><p>GitHub</p></td>
<td style="text-align: center;"><p>GitHub</p>
<p><a href="https://docs.github.com/en/enterprise-server/admin/overview/about-github-enterprise-server">GitHub Enterprise Server</a></p>
<p><a href="https://docs.github.com/en/enterprise-cloud@latest/admin/data-residency/about-github-enterprise-cloud-with-data-residency">GitHub Enterprise Cloud</a></p></td>
</tr>
</tbody>
</table>

## Considerations

  - Gemini Code Assist on GitHub does not generate summaries or code suggestions for any files located within the `.github/workflows` directory. This exclusion helps prevent the introduction of potentially insecure configurations to the repository.

  - The [enterprise version](https://developers.google.com/gemini-code-assist/docs/review-repo-code#versions) uses a [Developer Connect connection](https://docs.cloud.google.com/developer-connect/docs/git-repo-connections) to connect your GitHub repositories to Google Cloud.
    
      - This Developer Connect connection is always created in the region `us-east1` .
    
      - This Developer Connect connection must be created using the **Code Assist Source Code Management** section found in Gemini Code Assist **Agents & Tools** . For instructions, see [Set up Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) .

## What's next

  - [Set up Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) .
  - [Use Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/use-code-assist-github) .
  - Learn how to [customize Gemini Code Assist on GitHub behavior](https://developers.google.com/gemini-code-assist/docs/customize-repo-review) .

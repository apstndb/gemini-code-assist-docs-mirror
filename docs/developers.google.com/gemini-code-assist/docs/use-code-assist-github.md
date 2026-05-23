---
name: documents/developers.google.com/gemini-code-assist/docs/use-code-assist-github
uri: https://developers.google.com/gemini-code-assist/docs/use-code-assist-github
title: Use Gemini Code Assist on GitHub
description: Review pull requests using Gemini Code Assist.
data_source: developers.google.com
---

This page shows you how to use [Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/review-repo-code) . This page applies to both [consumer and enterprise versions](https://developers.google.com/gemini-code-assist/docs/review-repo-code#versions) of Gemini Code Assist on GitHub.

## Before you begin

To complete the tasks in this page, make sure you have [set up Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) .

## Get pull request summary and feedback

To get an initial review for a pull request from Gemini Code Assist, create a new pull request.

When you open the new pull request, Gemini Code Assist provides an initial review. After the review is ready, `gemini-code-assist[bot]` is automatically added as a reviewer to the pull request. Gemini Code Assist adds an issue comment in the **Conversation** tab of the pull request with its feedback and proceeds to add comments about modified portions of the code.

Review comments contain the following information:

  - Severity of the issue, given as Critical, High, Medium, and Low
  - Feedback on the issue
  - Code suggestion that can be committed directly from GitHub
  - References to a [user-provided style guide](https://developers.google.com/gemini-code-assist/docs/code-review-style-guide)

Gemini Code Assist does not add comments that have a *severity* less than the minimum severity threshold that is [set for the repository](https://developers.google.com/gemini-code-assist/docs/customize-repo-review) .

## Manually invoke Gemini Code Assist

Gemini Code Assist listens to comments from any pull request contributor, and decides whether it should respond.

To manually invoke Gemini Code Assist, you can use the following commands in the main comments page on the pull request as an issue comment.

| Command           | Description                                            |
| ----------------- | ------------------------------------------------------ |
| `/gemini summary` | Posts a summary of the changes in the pull request     |
| `/gemini review`  | Posts a code review of the changes in the pull request |
| `/gemini`         | Manually invokes Gemini Code Assist in comments        |
| `/gemini help`    | Overview of the available commands                     |

## Manage the Gemini Code Assist settings

Anyone with permissions to modify GitHub App settings for the organization can manage the Gemini Code Assist app settings. You can review the permissions provided to the Gemini Code Assist app, manage repository access, and uninstall the Gemini Code Assist app.

To modify the settings, follow these steps:

1.  On GitHub, click your profile photo and then click **Settings** .
2.  In the **Integrations** section, click **Applications** . A list of GitHub Apps is displayed.
3.  Beside Gemini Code Assist, click **Configure** .

## Troubleshooting

If you're using the [enterprise version](https://developers.google.com/gemini-code-assist/docs/review-repo-code#versions) of Gemini Code Assist on GitHub and you're not receiving responses from Gemini Code Assist, it might be because the Google Cloud project that you used during setup isn't connected to a valid billing account. You should [verify the billing status of your project](https://developers.google.com/billing/docs/how-to/verify-billing-enabled) and, if necessary, connect your project to a valid billing account.

Note that Developer Connect has a large [free tier](https://cloud.google.com/developer-connect/pricing) , and there are no charges for using the enterprise version of Gemini Code Assist on GitHub during Preview. While a valid billing account is required, it only accrues charges when usage goes over the free tier limits.

## What's next

  - Learn more about [Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/review-repo-code) .
  - [Set up Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) .
  - Learn how to [customize Gemini Code Assist on GitHub behavior](https://developers.google.com/gemini-code-assist/docs/customize-repo-review) .

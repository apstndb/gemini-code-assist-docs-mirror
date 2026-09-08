---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/cross-org-license-usage
uri: https://docs.cloud.google.com/gemini/docs/codeassist/cross-org-license-usage
title: Help prevent cross-organization license usage
description: Describes scenarios to consider and help prevent using Gemini Code Assist licenses across organizations.
data_source: docs.cloud.google.com
---

This document describes methods to help prevent usage of Gemini Code Assist licenses across an organization, and scenarios where you might want to limit that usage.

By design, Gemini Code Assist licenses are assigned to individual users, not organizations or projects. This design lets individual users use Gemini Code Assist across multiple organizations.

However, some large organizations, such as global system integrators (GSIs), might want to [prevent cross-organization usage](https://docs.cloud.google.com/gemini/docs/codeassist/cross-org-license-usage#methods_to_help_prevent_cross-organization_usage) . For example:

  - **Developers working on projects that have different billing accounts.** For instance, you might let a developer work on one project but limit access to other projects because they have different billing accounts, even if they are in the same organization.
  - **Developers working on multiple projects from different customers.** For instance, a developer might work on projects for delivery organizations that have different tenancies and tools.

## Methods to help prevent cross-organization usage

To help prevent cross-organization usage of Gemini Code Assist in a project, you can do one of the following:

  - [Disable the Gemini for Google Cloud API on a project](https://docs.cloud.google.com/gemini/docs/turn-off-gemini#companion-api) .
  - Use Identity and Access Management (IAM) [denial policies](https://docs.cloud.google.com/iam/docs/deny-overview) to deny user access to the project.

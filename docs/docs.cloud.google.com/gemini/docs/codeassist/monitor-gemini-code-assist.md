---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/monitor-gemini-code-assist
uri: https://docs.cloud.google.com/gemini/docs/codeassist/monitor-gemini-code-assist
title: Monitor Gemini Code Assist usage
description: Visualize and analyze Gemini Code Assist usage metrics for your organization by using built-in Cloud Monitoring tools.
data_source: docs.cloud.google.com
---

This document describes how to monitor [Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/overview) usage in your organization.

Gemini Code Assist automatically collects and stores [metrics](https://docs.cloud.google.com/monitoring/docs/collect-metrics-overview#gc-metrics) in [Cloud Monitoring](https://docs.cloud.google.com/monitoring/docs) . You can use the data visualization and analysis tools in Cloud Monitoring to help you answer important questions, such as how many daily active users in your organization are using Gemini Code Assist. This dashboard is automatically available when you enable and use Gemini Code Assist, and includes some of the most important metrics, which lets you quickly view aggregated usage data.

## Limitations

Gemini Code Assist metrics data recording is limited to user interactions with Gemini Code Assist within the IDE.

## Before you begin

To get the permissions that you need to view metric data by using the Google Cloud console, ask your administrator to grant you the [Monitoring Viewer](https://docs.cloud.google.com/iam/docs/roles-permissions/monitoring#monitoring.viewer) ( `roles/monitoring.viewer` ) IAM role on your project. For more information about granting roles, see [Manage access to projects, folders, and organizations](https://docs.cloud.google.com/iam/docs/granting-changing-revoking-access) .

You might also be able to get the required permissions through [custom roles](https://docs.cloud.google.com/iam/docs/creating-custom-roles) or other [predefined roles](https://docs.cloud.google.com/iam/docs/roles-overview#predefined) .

Additionally, users must have the [Gemini Cloud Assist User](https://docs.cloud.google.com/iam/docs/roles-permissions/geminicloudassist#geminicloudassist.userrole) ( `roles/geminicloudassist.user` ) role on your project to collect their usage metrics and send the data to the dashboard.

## Available metrics

The following tables list metrics available for Gemini Code Assist. All metrics are reported under the `cloudaicompanion.googleapis.com/Instance` resource type.

### General active user metrics

These metrics track the number of users shown a response from a Gemini Code Assist service over different time frames.

| Metric                                      | Name                     |
| ------------------------------------------- | ------------------------ |
| `code_assist/hourly_active_user_count`      | Hourly active user count |
| `code_assist/daily_active_users`            | Daily active users       |
| `code_assist/weekly_active_user_count`      | Weekly active user count |
| `code_assist/twenty_eight_day_active_users` | 28-day active users      |

### Code suggestion and interaction metrics

These metrics count the number of Gemini Code Assist code responses shown to and accepted by users in the IDE or with the Gemini CLI.

| Metric                                        | Name                            |
| --------------------------------------------- | ------------------------------- |
| `code_assist/code_suggestions_count`          | Code suggestions count          |
| `code_assist/code_suggestions_accepted_count` | Code suggestions accepted count |
| `code_assist/code_lines_accepted_count`       | Code lines accepted count       |
| `code_assist/chat_conversation_count`         | Chat conversations              |
| `code_assist/chat_responses_count`            | Chat response count             |
| `code_assist/chat_responses_accepted_count`   | Chat responses accepted count   |

### Platform and usage metrics

These metrics track usage at the platform level, including API calls and tokens used.

| Metric                          | Name              |
| ------------------------------- | ----------------- |
| `code_assist/used_tokens_count` | Used tokens count |
| `code_assist/api_calls_count`   | API calls count   |

### Token and quota metrics

These metrics track model token consumption and overage usage for your organization:

| Metric              | Name                                     |
| ------------------- | ---------------------------------------- |
| `usage/token_count` | Total tokens (Input, Output, and Cached) |

## View Gemini Code Assist metrics in your project

To view aggregated metrics for Gemini Code Assist, do the following:

1.  Go to the **Gemini Code Assist Overview** page.

2.  Click **Metrics** in the left navigation menu.

## What's next

  - Learn how to view [Gemini Code Assist logs](https://docs.cloud.google.com/gemini/docs/log-gemini) .
  - Learn how to [monitor services and resources on Google Cloud](https://docs.cloud.google.com/monitoring/docs/monitoring-overview) .

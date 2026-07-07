---
name: documents/developers.google.com/gemini-code-assist/resources/quotas
uri: https://developers.google.com/gemini-code-assist/resources/quotas
title: Quotas and limits
description: Review quotas and limits for Gemini Code Assist.
data_source: developers.google.com
---

> **Note:** We have unified our tools into a single, multi-agent platform called Antigravity, with Antigravity CLI now available. Starting June 18, 2026, Gemini Code Assist IDE Extensions and Gemini CLI stopped serving requests for the Gemini Code Assist for individuals, Google AI Pro, and Google AI Ultra tiers. Affected users should migrate to Antigravity and Antigravity CLI. To learn more, see the [deprecation page](https://developers.google.com/gemini-code-assist/docs/deprecations/code-assist-individuals) .

This document lists the quotas and system limits that apply to your combined use of Gemini Code Assist and Gemini CLI.

  - *Quotas* specify the amount of a countable, shared resource that you can use.
  - *System limits* are fixed values that cannot be changed.

## Quotas for Gemini Code Assist

Gemini Code Assist enforces quotas for certain features.

| Quota                           | Value                          |
| ------------------------------- | ------------------------------ |
| Local codebase awareness        | 1,000,000 token context window |
| Code customization repositories | 20,000                         |

### Quotas for agent mode and Gemini CLI

Quotas for requests from Gemini Code Assist agent mode and Gemini CLI are combined. When in agent mode or when using the Gemini CLI, one prompt might result in multiple model requests. Requests are limited per user per minute and are subject to the availability of the service in times of high demand. These daily request limits are aggregated across all interactions with any model version or family (for example, Pro, Flash) used with the Gemini CLI or agent mode. Once the maximum number of requests per day is reached, no further requests can be made through these interfaces to any model until the quota resets.

Quota

Gemini Code Assist edition or license type

Way(s) to purchase

Value

Maximum requests per user per day

Standard

[Google Cloud console](https://developers.google.com/gemini-code-assist/docs/set-up-gemini-standard-enterprise)

1500

Enterprise

[Google Cloud console](https://developers.google.com/gemini-code-assist/docs/set-up-gemini-standard-enterprise)

2000

### Quotas for Gemini Code Assist on GitHub

Usage of [Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/review-repo-code) is not counted as part of the general quotas for Gemini Code Assist.

  - An installation of the consumer version of the Gemini Code Assist on GitHub app has a quota of 33 pull request reviews per day.

  - An [installation](https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github) of the enterprise version of the Gemini Code Assist on GitHub app [(Preview)](https://cloud.google.com/products#product-launch-stages) has a quota of at least 100 pull request reviews per day.
    
      - The exact number of pull request reviews depends on the codebase and how many model calls are required to complete each code review. Because of this, in some cases the quota can be significantly greater than 100.

Gemini Code Assist on GitHub quotas reset in alignment with resets for [Google Cloud quotas](https://docs.cloud.google.com/docs/quotas/overview#running_out) .

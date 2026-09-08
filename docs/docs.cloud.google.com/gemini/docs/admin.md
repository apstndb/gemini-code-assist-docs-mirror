---
name: documents/docs.cloud.google.com/gemini/docs/admin
uri: https://docs.cloud.google.com/gemini/docs/admin
title: Modify Gemini Code Assist subscriptions
description: Manage subscriptions, licenses, and more in the Gemini Code Assist admin controls.
data_source: docs.cloud.google.com
---

This document describes how to access and use the Gemini Code Assist administrator controls.

Gemini Code Assist subscriptions are subject to Google Cloud [Service Specific Terms](https://cloud.google.com/terms/service-terms) regarding Pricing and Billing for Committed Units.

## Grant IAM permissions

In order to get the required permissions for editing Gemini Code Assist subscriptions, ask your administrator to grant you the [`roles/billing.admin` IAM role](https://docs.cloud.google.com/billing/docs/how-to/billing-access#billing.admin) on the billing account.

Alternatively, ask your administrator to grant you the [`roles/consumerprocurement.orderAdmin` role](https://docs.cloud.google.com/marketplace/docs/access-control#consumerprocurement.orderAdmin) *and* the [`roles/billing.viewer` role](https://docs.cloud.google.com/billing/docs/how-to/billing-access#billing.viewer) .

These roles contain the permissions required to modify Gemini Code Assist subscriptions. To see the exact permissions that are required, expand the **Required permissions** section.

#### Required permissions

  - `consumerprocurement.orders.place`
  - `billing.billingAccountPrices.list`

## Access Gemini Code Assist administrator controls in the Google Cloud console

To access Gemini Code Assist administrator controls in the Google Cloud console, select **Admin for Gemini** in the navigation menu.

### Pick a billing account

To edit or purchase a Gemini Code Assist subscription, you must pick a billing account. Your Gemini Code Assist subscription is tied to a billing account and can be used with any project. You can only have one Gemini Code Assist subscription per billing account.

The following list shows possible ways to pick a billing account:

  - **Manage subscriptions with project access** .
    
      - If you don't have a subscription yet, click **Get Gemini Code Assist** to purchase one. Note that you must [set up a billing account](https://docs.cloud.google.com/billing/docs/how-to/create-billing-account) first.
    
      - If you have a subscription already but it's not associated with this billing account, click **Manage subscriptions** and then select a different billing account where you want to manage the subscription.
    
      - If you already have a subscription associated with your current billing account, click **Manage Gemini Code Assist** to navigate to the settings page. Then, click **Manage Subscriptions** to select and manage existing subscriptions.

  - **Manage subscriptions without project access** . If you have permission to manage subscriptions, select the product you want to edit or purchase. Then, select **Manage Subscription** and select a billing account.

  - **Manage subscriptions for projects in a folder** . If you start from a folder, you must select a billing account before you purchase a subscription, since billing accounts can't be directly associated with a folder.

## Edit a Gemini Code Assist subscription

> **Important:** Changes to a subscription that decrease the number of licenses, downgrade the edition, or reduce the subscription period don't take effect immediately; instead, they take effect at the end of the current subscription term. Similarly, you can't cancel a subscription during its term. If you want to end your subscription, make sure that you have auto-renewal disabled. For more information, see [Turn off Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/turn-off) .

1.  In the Google Cloud console, go to the **Admin for Gemini** page.
    
    The **Admin for Gemini** page loads.

2.  Use the project picker at the top of the page to ensure you are scoped to the project or folder that has an existing Gemini Code Assist subscription.

3.  Locate the **Gemini Code Assist** product tile, and then click **Manage Gemini Code Assist** .

4.  Select **Manage subscription** .
    
    The **Manage subscription** page appears.

5.  Select **Manage subscription** to edit the subscription, including:
    
      - **Manage edition** - If you're editing your Gemini Code Assist subscription, then you can upgrade from Standard edition to Enterprise edition, which takes effect immediately. Alternatively, you can downgrade from Enterprise edition to Standard edition, which takes effect at end of the current subscription term. To see a list of features available in each edition, see [Supported features](https://docs.cloud.google.com/gemini/docs/codeassist/overview#supported-features) .
        
        > **Note:** Gemini Code Assist Standard licenses obtained using the Gemini Enterprise bundle cannot be upgraded in the Google Cloud console because they are licenses, not a standalone subscription. To obtain Enterprise features in this scenario, you must purchase a separate Gemini Code Assist Enterprise subscription.
    
      - **Increase or decrease the number of licenses in the subscription** - Adding licenses makes them available to you almost immediately. However, if you reduce the number of licenses, then the changes won't take effect until the end of the subscription term. Additionally, the original license count is still reflected in your bill until the changes are applied.
    
      - **Change the subscription period** - You can set the subscription to bill monthly or annually. With an annual subscription, you are given a discounted rate that is charged on a monthly basis rather than a one-time payment. If you change from an annual subscription to a monthly subscription, then the change won't take effect until the end of the annual term. Additionally, you cannot change the subscription period unless you have enabled subscription auto-renewal.
    
      - **Enable or disable auto-renewal** - If you disable auto-renewal, the subscription expires at the end of the subscription term and all the licenses in the subscription become invalid. You cannot re-enable a subscription after it expires. Instead, you'll need to [purchase a new subscription](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini#purchase-subscription) to re-assign those licenses. Additionally, if auto-renewal is disabled, then you can't make the following changes:
        
          - Reduce number of licenses
          - Change from annual to monthly subscription period
          - Change from Enterprise edition to Standard edition

6.  Select **Continue** , and then select **Confirm changes** .

## What's next

  - Learn more about [Gemini Code Assist billing](https://docs.cloud.google.com/gemini/docs/billing-questions) .
  - [Manage your Gemini Code Assist licenses](https://docs.cloud.google.com/gemini/docs/codeassist/manage-licenses) .
  - [Turn off Gemini Code Assist](https://docs.cloud.google.com/gemini/docs/codeassist/turn-off) .

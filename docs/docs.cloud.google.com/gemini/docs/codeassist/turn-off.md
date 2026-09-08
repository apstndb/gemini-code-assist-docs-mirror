---
name: documents/docs.cloud.google.com/gemini/docs/codeassist/turn-off
uri: https://docs.cloud.google.com/gemini/docs/codeassist/turn-off
title: Turn off Gemini Code Assist
description: Describes how to turn off Gemini Code Assist.
data_source: docs.cloud.google.com
---

This document explains how to turn off Gemini Code Assist.

## Before you begin

  - To update a Gemini Code Assist subscription, make sure you have the `billing.subscriptions.update` Identity and Access Management (IAM) permission. The `billing.subscriptions.update` permission is included in the [`roles/billing.admin`](https://docs.cloud.google.com/billing/docs/how-to/billing-access#billing.admin) IAM role, or you can add the permission to a custom role.

## Turn off Gemini Code Assist

To turn off Gemini Code Assist, do the following:

1.  In the Google Cloud console, go to the **Gemini Products** page.

2.  From the **Gemini Products** page, navigate to the **Manage Subscription** page for the billing account associated with your project:
    
      - If you are prompted to select a billing account, select it and click **Continue to Admin for Gemini page** . Then, from the navigation menu, click **Manage Subscription** .
      - If you are not prompted to select a billing account, you are taken to the **Admin for Gemini** page. From the navigation menu, click **Manage Subscription** .

3.  Click the Gemini Code Assist subscription. The name of the subscription depends on the name given when Gemini Code Assist was set up.

4.  Review the subscription details and check the **Auto renew** setting.
    
      - If **Auto renew** is set to **Off** , then your subscription is already set to end on the subscription end date. No further action is needed.
    
      - If **Auto renew** is set to **On** , follow these step to disable it:
        
        1.  Click **Manage subscription** .
        2.  To proceed to renewal settings, click **Continue** .
        3.  For **Automatic subscription renewal** , select **No, don't automatically renew** , and then click **Continue** .
        4.  If you agree to the terms of purchase, select **I agree to the terms of this purchase** , and then click **Save changes** .

5.  Optional: If you are disabling all Gemini products in Google Cloud, then turn off the [Gemini for Google Cloud API](https://docs.cloud.google.com/gemini/docs/turn-off-gemini#companion-api) .

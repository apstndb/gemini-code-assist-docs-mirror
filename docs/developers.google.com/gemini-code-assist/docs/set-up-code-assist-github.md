---
name: documents/developers.google.com/gemini-code-assist/docs/set-up-code-assist-github
uri: https://developers.google.com/gemini-code-assist/docs/set-up-code-assist-github
title: Set up Gemini Code Assist on GitHub
description: Review pull requests using Gemini Code Assist.
data_source: developers.google.com
---

This page shows you how to set up the enterprise version of [Gemini Code Assist on GitHub](https://developers.google.com/gemini-code-assist/docs/review-repo-code) , a Gemini-powered agent that automatically summarizes pull requests and provides in-depth code reviews.

> **Important:** Serving requests to the [consumer version](https://developers.google.com/gemini-code-assist/docs/review-repo-code#versions) of Gemini Code Assist on GitHub is being discontinued, and you shouldn't install this version.

## Before you begin

To set up the enterprise version of Gemini Code Assist on GitHub, make sure you do the following:

1.  Have a GitHub organization or personal account.

2.  Have one or more GitHub repositories that you want to enable Gemini Code Assist on GitHub on.
    
    If you don't have such a repository, you can create a fork of [our sample repository](https://github.com/GoogleCloudPlatform/microservices-demo) to use.

3.  Ask your administrator to [grant](https://cloud.google.com/iam/docs/granting-changing-revoking-access) you the [**Service Usage Admin** role](https://cloud.google.com/iam/docs/roles-permissions/serviceusage#serviceusage.serviceUsageAdmin) and the `geminicodeassistmanagement.scmConnectionAdmin` role.
    
    > **Important:** The `geminicodeassistmanagement.scmConnectionAdmin` role can't be granted using the Google Cloud console. Use the Google Cloud CLI instead.
    
      - Alternatively, if you have the [**Admin** or **Owner** basic roles](https://cloud.google.com/iam/docs/roles-overview#basic) , you have the necessary IAM permissions to complete the setup for the enterprise version.

4.  Ensure that the Google Cloud project you use during setup is connected to a valid billing account.

## Install Gemini Code Assist on GitHub

The following steps show you how to set up the enterprise version of Gemini Code Assist on GitHub.

> **Preview**
> 
> This feature is subject to the "Pre-GA Offerings Terms" in the General Service Terms section of the [Service Specific Terms for Google Cloud](https://cloud.google.com/terms/service-terms#1) . Pre-GA features are available "as is" and might have limited support. For more information, see the [Google Cloud launch stage descriptions](https://cloud.google.com/products/#product-launch-stages) .

1.  In the Google Cloud console, go to the Gemini Code Assist **Agents & Tools** page.
    
    1.  If you haven't previously enabled the Developer Connect API, you see a caution banner that prompts you to enable the API. If this happens, click the **Enable** button associated with the banner, and click the **Enable** button in the dialog window that appears.

2.  In the **Agents** section, locate the **Code Assist Source Code Management** card, and click **Enable** .
    
    The **Enable Code Assist Source Code Management** pane opens.

3.  In the **Gemini Code Assist Management API** section, click **Enable** .

4.  In the **Select a connection** section, click the **Connection** drop-down.

5.  In the drop-down, click **Create new connection** .
    
    The **Link Git repositories via Developer Connect** pane opens.
    
    > **Note:** Gemini Code Assist on GitHub creates the Developer Connect connection in `us-east1` and doesn't support using existing connections you might have for other features, such as [code customization](https://developers.google.com/gemini-code-assist/docs/code-customization-overview) .

6.  In the **Provider** drop-down, select the GitHub provider you are using.

7.  In the **Name** field, enter a name for your connection.

8.  Click **Continue** .
    
    The **Request GitHub OAuth token** dialog window open.

9.  After reading the disclaimer, click **I understand and continue** .

10. In the **Install Gemini Code Assist** page, click the account you want to install the app in.

11. Choose whether to install the app for **All repositories** or **Only select repositories** .

12. Click **Install** .

13. Follow the GitHub steps to authenticate to GitHub.
    
    Once access is confirmed, the dialog window closes and you return to the **Link Git repositories via Developer Connect** pane.

14. In the **Link repositories** section, click the **Repositories** drop-down, select the repositories you want to link, and click **Ok** .
    
    > **Note:** If you create a new GitHub repository in the future and want to add it to the linked repositories in your connection, you must [use Developer Connect](https://cloud.google.com/developer-connect/docs/connect-github-repo#link-repos) to do so.

15. Click **Link** .

16. In the **Select a connection** drop-down, select the connection you created.

17. Click **Done** .

Gemini Code Assist is now active for all the pull requests within your selected repositories.

## What's next

  - Learn more about [Gemini Code Assist in GitHub](https://developers.google.com/gemini-code-assist/docs/review-repo-code) .
  - [Use Gemini Code Assist in GitHub](https://developers.google.com/gemini-code-assist/docs/use-code-assist-github) .
  - Learn how to [customize Gemini Code Assist on GitHub behavior](https://developers.google.com/gemini-code-assist/docs/customize-repo-review) .

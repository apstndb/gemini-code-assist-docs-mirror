---
name: documents/developers.google.com/gemini-code-assist/docs/feedback
uri: https://developers.google.com/gemini-code-assist/docs/feedback
title: Provide Gemini Code Assist feedback
description: Provide feedback about Gemini
data_source: developers.google.com
---

> **Important:** This page is only about feedback options for Gemini Code Assist. If you want to send feedback about Gemini in your iPhone or Android phone, see [Send feedback or report a problem with Gemini Apps](https://support.google.com/gemini/answer/13275746) .

Google welcomes feedback about Gemini Code Assist to help make the product better. To provide feedback, do one of the following:

  - You can submit feedback about Gemini Code Assist (and other Gemini for Google Cloud products) by filling out the [Gemini for Google Cloud survey](https://google.qualtrics.com/jfe/form/SV_3Uhk1BDQCUeerEW) . This survey lets you submit feedback about the quality of the answers that you get from a prompt, and also about the prompt itself to help us improve the response. The survey takes about five minutes to complete.

  - If you're using the Gemini Code Assist in VS Code or IntelliJ plugins, you can submit feedback directly in your IDE using these steps:
    
    ### VS Code
    
    1.  You can leave feedback in either of the following ways:
        
          - In the status bar, click spark **Gemini Code Assist** , and then in the **Quick Pick** menu, select **Send feedback** .
          - Open the **Command Palette** ( `Ctrl` / `Command` + `Shift` + `P` ) and then select **Gemini Code Assist: Send Feedback** .
    
    2.  In the form, fill out the **Title** and **Comments** fields.
    
    3.  In the **Feedback for Gemini Code Assist** form, select an option from the **Feedback category** and **Type** drop-down menus.
    
    4.  Write a detailed description of your experience in the **Comment** field.
    
    5.  Make sure to include your Gemini Code Assist logs in your feedback report. By default, this option is selected.
    
    6.  Check or un-check any of the other options, as you prefer.
    
    7.  Click **Submit Feedback** .
    
    ### IntelliJ
    
    1.  In the status bar, click spark **Gemini Code Assist** .
    
    2.  After prompting Gemini Code Assist in the chat, and if you aren't satisfied with the response, click thumb\_down **Negative** and then select **Provide feedback** .
    
    3.  In the text field at the top of the form, enter your feedback.
    
    4.  If you want to share your Gemini Code Assist logs, make sure that you select the log files.
    
    5.  Click **Submit Feedback** .

## Download Gemini Code Assist logs for support

The following steps describe how to retrieve your Gemini Code Assist log files to share for support, which you can download directly from your IDE:

### VS Code

1.  Open the **Command Palette** (press `Ctrl` / `Command` + `Shift` + `P` on Windows and Linux, or `Cmd` / `Command` + `Shift` + `P` on macOS).

2.  Select **Gemini Code Assist: Download logs for support** .

3.  In the warning dialog that explains the logs might contain sensitive data from your session, click **Continue** .
    
    Note that clicking **Continue** only compiles your logs into a local ZIP file. The plugin does not automatically send this ZIP file to Google. You can open and review the files in the ZIP folder on your machine to remove any sensitive information before you share it with support.

4.  Select a location on your machine to save the ZIP file, and then click **Save** .

### IntelliJ

To locate the debug logs on your local file system:

1.  From the top menu of your JetBrains IDE, select **Help** \> **Show Log in Explorer** (on Windows and Linux) or **Help** \> **Show Log in Finder** (on macOS).

2.  In your file explorer, locate the active log files (such as `idea.log` ) to share for support.

The preceding feedback options are submitted anonymously and used only to improve Gemini Code Assist.

---
id: "section_N3393788"
type: "section"
title: "Sending Bundle Messages"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Sending Bundle Messages"
parent: "section_N3384420"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393788.html"
anchors: ["procedure_N3393831"]
sha256: "199c880aafcff5caaf2abe1e0fb332749d08386c00b130806e3c86a3b2c0695d"
---

You can send messages to your install base for any bundle you've created. You can create, send, and review messages on the **Messages** subtab of the Bundle Details page.

Bundle messages are displayed on the Bundle Details page in selected target accounts, and may also be sent as email to target account bundle administrators. If you are a target account bundle user, see [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html) for details.

Warning:

You cannot send bundle messages to or from Sandbox accounts.

#### To create and send a bundle message: {#procedure_N3393831}

1.  Go to Customization > SuiteBundler > Saved Bundles > List.
    
2.  Click a bundle name to display its Bundle Details page.
    
3.  On the **Messages** subtab of the Bundle Details page, click **New Message**.
    
4.  If desired, change the email address to be displayed in the **From** field of the message.
    
    -   The default email address in the **From** field for the first bundle message sent from a source account is the email address of the currently logged in user.
        
    -   After this email address has been modified, it is used for later bundle messages from that source account until it is reset again.
        
    -   The **Reply-To** value for each bundle message is set to the email address in the **From** field, and bounced messages are returned to this email address.
        
    
    Note:
    
    For messages created prior to Version 2012 Release 2, the **From** field is blank by default.
    
5.  Enter a subject and message text.
    
    You can enter HTML or text. Rich text editing also is available if your user preference is set to enable it. (See [Personal Preferences for Appearance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479574.html).)
    
6.  The **Recipients** subtab lists accounts where the bundle is installed. Check the box for each account that you want to receive this message.
    
    -   You can filter the target accounts displayed on the **Recipients** subtab, to help you find the accounts that should receive a message. **Region** and **Bundle Version** filters are available.
        
7.  After you have entered text and selected recipient accounts, do one of the following:
    
    -   If you are not ready to send the message, click **Save as Draft**.
        
    -   If you are ready to send the message, click **Save & Send**.
        

When you send the message:

-   It is listed on the Bundle Details page in your account, with the number of install base accounts to which it has been sent, the number of accounts to which it has not been sent, and the date and time when it was last sent.
    
-   It is listed on the Bundle Details page in the target accounts you selected.
    
-   Each administrator and each user with SuiteApp Marketplace permission who are subscribed to this bundle's messages in target accounts receive an email. See [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html).
    

Important:

After you have sent a bundle message, you can no longer edit its subject or text. You can select additional accounts to receive the identical text, but if you want to change the text, you need to create a new message. Also, you cannot resend a message to an account that has already received it.

If you deprecate a bundle, after a target account installs the replacement bundle, its Bundle Details page **Messages** subtab no longer lists any messages sent for the deprecated bundle. Only messages sent for the replacement bundle are displayed. You can continue to send messages from a deprecated bundle, but these are only sent to accounts that have not yet updated to the replacement bundle.

If you delete a bundle in the source account, any messages sent for that bundle are removed from the Bundle Details page **Messages** subtab in all install base accounts.

### Related Topics

-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)
-   [Reviewing the Saved Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385293.html)
-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html)
-   [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html)
-   [Pushing a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391992.html)
-   [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
-   [Deleting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4465929869.html)
-   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
-   [Subscribing to Bundle Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397668.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

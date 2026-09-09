---
id: "section_N514531"
type: "section"
title: "Customizing Email Signatures and From Fields"
branch: "working-with-email"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Email > Sending Email from NetSuite > Customizing Email Signatures and From Fields"
parent: "section_N512264"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514531.html"
anchors: ["procedure_N514568"]
sha256: "c0ed2fdb59221c9c6a16f237c7d6321f388c1795cee438f5ea77151ec2b927ec"
---

You can set up an email profile to determine the following for email you send through NetSuite:

-   the name that appears in the From field
    
-   the From email address
    
-   a custom signature
    

#### To set up your email profile: {#procedure_N514568}

1.  Go to Home > Set Preferences, in the User Profile area of the **General** subtab.
    
2.  In the **Nickname** field, enter the name you want to appear in the **From** field on the email you send.
    
3.  In the **Signature** field, enter an email signature using HTML markup.
    
    For information about how to create an HTML signature file, see [Adding Images and Links to an Email Signature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1511181787.html).
    
    Note:
    
    You can enter up to 4000 HTML characters in this field.
    
4.  In the **From** Email Address field, enter the email address you want to appear in the From field on email you send.
    
5.  Click **Save**.
    

To include your email signature, you must include the following FreeMarker syntax in the email: `${preferences.message_signature}` You can also place this marker in email templates. If you don't enter a nickname or a From address, your login email address appears in the From field.

### Additional Information

-   [Add Logo or Image to Signature](https://suiteanswers.custhelp.com/app/answers/detail/a_id/24639)

### Related Topics

-   [Sending Email from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512264.html)
-   [Sending Email from Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512629.html)
-   [Requesting Read Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3734502442.html)
-   [Sending Email Directly from Lists and Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N513078.html)
-   [Sending Search and Report Results by Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514156.html)
-   [Attaching Files to Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

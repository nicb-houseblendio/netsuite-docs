---
id: "bridgehead_N2434142"
type: "bridgehead"
title: "Setting Up Your Mail Server for Email Case Capture in NetSuite OneWorld"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Up Customer Support in NetSuite OneWorld > Setting Up Your Mail Server for Email Case Capture in NetSuite OneWorld"
parent: "section_N2433348"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434142.html"
anchors: []
sha256: "c7f5b718132c0e46a08fa2380aeec3bf49a486ac7d9496add13c30dae7fdc845"
---

If you use the Email Case Capture feature, you can set up an inbound email address for each subsidiary using case profiles. See [Creating Case Profiles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3914420072.html).

When you have a case profile for each subsidiary, use **NetSuite Inbound Email Address** from the General subtab of each subsidiary's case profile. This is the forwarding address you'll redirect your company's subsidiary support email address to.

For example, on your company mail server you'd forward `support.emea@example.com` to the NetSuite Inbound Email Address of the subsidiary. If the company's account ID was 123456, the email address would look something like `cases.375xxx.248xx@123456.email.netsuite.com`. This enables cases to be automatically captured to your NetSuite account.

If you want to restrict the visibility of the case profile to the selected subsidiary only, select the subsidiary from the Subsidiary Filter field in the case profile record. For more information about server-side setup requirements when using Email Case Capture, see [Prerequisites for Setting Up Email Case Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162306863443.html).

### Related Topics

-   [Setting Company-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433546.html)
-   [Setting Subsidiary-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433676.html)
-   [Setting Up Case Forms for NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433829.html)
-   [Setting Up Online Case Forms for NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433912.html)
-   [Customizing Support Rep Roles for NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434051.html)
-   [Creating Case Rules and Territories Based on Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434106.html)
-   [Setting Up Customer Support in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2433348.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

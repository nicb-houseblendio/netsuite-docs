---
id: "bridgehead_N2425131"
type: "bridgehead"
title: "Support Email Notification"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Up Support Checklist > Setting Customer Service Preferences > Support Email Notification"
parent: "section_N2423389"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2425131.html"
anchors: []
sha256: "2694d52aa1f85ead7448f02676ca1d9374f894144c75c9afff10ca7ab6e3214f"
---

You can set the following support email preferences on the Notification subtab of the Support Preferences page.

If you use NetSuite OneWorld, you can create separate notification templates for each subsidiary. For more information, see [Setting Subsidiary-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433676.html).

| Column & Preference | Description |
| --- | --- |
| **Creation** |  |
| Notify Filer On Support Rep Cases | Check this box to automatically send email notification to customers when support reps manually create cases in your account. Checking this box also enables notification to employees when they submit help desk cases. Note: All case creation emails use the template you select in the Customer Notification Template field. |
| Notify Filer On External Cases | Check this box to automatically send email notification to customers when cases are submitted using the external case form in the Customer Center. Note: This doesn't send notification to customers submitting cases using online case forms. To send notification to these customers, select an email template in the Send Auto-Reply Email field on the Set Up Workflow subtab of the online form record. |
| Notify Main Support Email On External Cases | Check this box to send notification email to the support profile entered on the General subtab. Email is sent when new cases are created with an external case form in the Customer Center. |
| **Inbound Email Case Capture** |  |
| Notify Customers | Check this box to automatically send email notification to customers when cases are submitted by email using the Email Case Capture feature. Email notification uses the template you select in the Customer Notification Template field. |
| Notify to List | Check this box to send notification that a case was created to each email address listed in the **To** line of the original email. This preference works like Reply To All for the 'To' line only. |
| Notify CC List | Check this box to include addresses in the **CC** line of the original email when replying to incoming cases with notification. |
| **Assignment** |  |
| Notify Assignees | Check this box to automatically send email notification to support reps when cases are assigned to them. |
| Send Notification Replies to Customer | Check this box to send the customer a copy of the support rep's reply when they're assigned to a case. The reply appears on the case record. |
| **Update** |  |
| Notify Assignees | Check this box to send a notification email to support reps when any changes are made to a case assigned to them. This includes when customers reply to the case creation notification. |
| Send Notification Replies to Customer | Check this box to send the customer a copy of the support rep's reply when the case is updated. The reply appears on the case record. |
| **Escalation** |  |
| Notify Escalatees Upon Update | Check this box to send a notification to the person the case is escalated to whenever the case is updated. |
| Send Notification Replies to Customer | Check this box to send the customer a copy of the support rep's reply when the case is escalated. The reply appears on the case record. |
| **Closure** |  |
| Notify Customer Upon Automatic Closure | Check this box to notify a customer when their case is automatically closed because all other cases linked to the case have been closed. This preference requires Automatically Close Linked Cases to be enabled. Go to _Setup > Issues > Preferences > Issue Preferences_. Note: The notification is not sent if a linked case is closed manually. |

Important:

Assignment notifications aren't sent when a user logs in and assigns a case to themselves. Additionally, update notifications aren't sent when a user updates a case they're assigned to. You can work around this limitation by creating a SuiteScript that sends a notification to the logged in user after a case is saved.

### Related Topics

-   [External Case Capture Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2425980.html)
-   [Inbound Support Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2426150.html)
-   [Ordering Support Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2426304.html)
-   [Setting Customer Service Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423389.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

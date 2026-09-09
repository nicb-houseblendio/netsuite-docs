---
id: "section_N2423389"
type: "section"
title: "Setting Customer Service Preferences"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Up Support Checklist > Setting Customer Service Preferences"
parent: "section_N2421296"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423389.html"
anchors: ["bridgehead_N2423431"]
sha256: "4d2d873412dc16e81e357bde0320ef3644cb581f5ba8bf8cda9191c03b7eb2fa"
---

The Support Preferences page is where you set your default preferences for your customer support team's workflow.

To set support preferences, go to _Setup > Support > Preferences > Support Preferences_.

## General Support Preferences {#bridgehead_N2423431}

You can set the following preferences on the General subtab on the Support Preferences page.

| Preference | Description |
| --- | --- |
| **Case Email Setup** |  |
| Default Case Form to Send to Customer | Check this box to have the email Reply box on case records checked by default. |
| Default Case Form to Internal Only | Check this box if you want replies to cases marked Internal Only by default. |
| Default Case Profile | Select the default profile for incoming support cases. See [Creating Case Profiles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3914420072.html) |
| **Preferences** |  |
| Escalate to Support Reps Only | Check this box to only allow cases to be escalated to support reps. If you clear this box, cases can be escalated to partners, vendors and non-support rep personnel. |
| Prevent Support Reps from Receiving Customer Replies by Email | Check this box if you don't want support reps to receive an email copy of a customer's reply to a case. If you clear this box, the customer's reply is sent to the support rep by email and stored in the case record. Any subsequent replies are also added to the case record. This preference only shows if you have the Capture Email Replies feature enabled. |
| Messages Reopen Closed Cases | Check this box to let closed cases to change status to Re-Opened when a message is added to the case. Clear this box to have the case remain closed when a customer replies and prompt to create a new case. If you check this box and also choose to lock closed cases, the locked cases preference isn't overridden. Cases will not be reopened with new messages. |
| Only Link Approved Solutions to Cases | Check this box to only allow solutions that have been approved to be attached to case records. All solutions set to display online are also available to attach to cases. |
| External Case Response Page | If you check this box, anyone with a link can access the External Case Response Page that contains information about a case. If you clear the box, users need to log in to NetSuite to access the page. This preference is available only when the Customer Support and Service feature is enabled. |
| External Link Validity Period (in Weeks) | Set the duration (in weeks) for external links to the External Case Response Page. Values can be between two and eight weeks. Administrators can manually expire any active link by clicking Disable Link on the case record in edit mode. If external users click an expired link, they're automatically prompted and guided through the UI to generate a new link. |
| **Defaults** |  |
| Status for New Cases | Select the status a new case is set to when it's first created. You can create new statuses at _Setup > Support > Case Statuses > New_. |
| Status for Grabbed Cases | Select the status a case is set to when a support rep grabs it. |
| Status for Reopened Cases | Select the status a closed case is set to after it's reopened. |
| Status for Escalated Cases | Select the status a case is set to when it's escalated to another employee. |
| Status for Closed Cases | Select the status a case is set to when it's closed. |
| Priority for New Cases | Select the case priority newly created cases are set to. You can create new case priorities at _Setup > Support > Case Priorities > New_. |
| **Case Lockout** |  |
| Lock Closed Cases After Lockout Period | Check this box to lock closed cases from being edited after the specified number of days in the Period (Days) field. Only account administrators can edit locked cases. |
| Period (Days) | Specify how many days you want closed cases to remain editable for after they're closed. Enter 0 to lock editing immediately after a case closure. |

### Related Topics

-   [Support Email Notification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2425131.html)
-   [External Case Capture Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2425980.html)
-   [Inbound Support Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2426150.html)
-   [Ordering Support Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2426304.html)
-   [Creating Case Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422185.html)
-   [Creating Case Origins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422364.html)
-   [Creating Case Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422557.html)
-   [Creating Case Priorities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422747.html)
-   [Creating Case Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422868.html)
-   [Offering Support for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423026.html)
-   [Setting Up Support Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423204.html)
-   [Marking Employees as Support Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2426343.html)
-   [Setting Up Support Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2421296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

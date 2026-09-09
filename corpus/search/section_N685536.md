---
id: "section_N685536"
type: "section"
title: "Sending Summarized vs. Single-Record Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Sending Summarized vs. Single-Record Results"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html"
anchors: []
sha256: "87853024f7f070e1636253d331dbf64f31af32eab38fb4a23cf880f4b8416fee"
---

The following options are available for scheduled email results:

-   When the **Summarize Scheduled Emails** option is enabled, the recipients listed on the **Specific Recipients** subtab of the saved search **Email** subtab will receive a single email that contains a summary of all results. However, each of the recipients listed on the **Recipients from Results** subtab will receive only a summary of results related to this particular recipient.
    
-   When the **Summarize Scheduled Emails** option is disabled, the recipients listed on both the **Specific Recipients** and **Recipients from Results** subtabs of the saved search **Email** subtab will receive a separate email for each of the records in the search results. In this case, each email message is a "single-record result". Recipients may receive multiple messages on each scheduled date. This option can be used for drip marketing.
    

Important:

If the **Results** subtab of your saved search contains even one summarized field, all recipients are sent a summary of the results. This happens even if the **Summarize Scheduled Emails** option is disabled. Recipients on the **Specific Recipients** subtab are sent a single email containing the summary of the results. Recipients on the **Recipients from Results** subtab are sent an email containing a summary of the results specific to their records. Additionally, sending email using the **Save & Email** button always sends summarized results, regardless of the **Summarize Scheduled Emails** setting.

These settings do not apply to alert email, because these messages are always single-record results. Note that you can customize an alert message for a search that returns multiple rows per record, such as a transaction search, to include multiple rows. For information, see [Enabling Multi-Row Results for Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685250.html).

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html)
-   [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html)
-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

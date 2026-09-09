---
id: "section_N684160"
type: "section"
title: "Defining the Sender for Saved Search Email"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Defining the Sender for Saved Search Email"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html"
anchors: ["bridgehead_N684272"]
sha256: "f30062d47ad99ff412752e4322fee72f699ace2aa38c1b31fddcff49da03bbd6"
---

The sender of emails for a saved search is determined as follows:

1.  If a custom email address has been provided in the **From** field on the saved search record's **Email** subtab's **Customize Message** subtab, emails are sent from this address.
    
    For required format details, see [Required Format for Saved Search Email Sender](#bridgehead_N684272). For other details, see [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html).
    
2.  If the **From** field is blank, email messages are sent from the email address defined in the search owner's employee record.
    
3.  If the **From** field is blank, and no email address is defined in the search owner's employee record, email messages are sent from the email address defined in the **Return Email Address** field at _Setup > Company > Company Information_.
    
    For details about default return email address settings, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).
    

## Required Format for Saved Search Email Sender {#bridgehead_N684272}

The required format of the email sender for the **From** field on the saved search record's **Email** subtab's **Customize Message** subtab is the following:

          `'name' <email address>` 
        

Note the following:

-   The name must be enclosed in double quotes.
    
-   The email address must be enclosed in carets.
    
-   There must be a space between the quoted name and the email address.
    

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html)
-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)
-   [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N684570"
type: "section"
title: "Defining Recipients for Saved Search Email"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Defining Recipients for Saved Search Email"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html"
anchors: ["procedure_N684646", "procedure_N684748", "procedure_N684802"]
sha256: "f7a7a3ce5bf8ab18f24ca107c067e5e13d91b4245774d1e35c9f4b26b3af2331"
---

On the Email subtab of the saved search page, you can enable saved search email alerts triggered by record adds or updates, as well as scheduled email of saved search results sent according to defined intervals.

You can define multiple recipients for both types of saved search email, alerts and scheduled. Recipient lists are shared for both types of saved search email, and you can enable both at the same time. If you have enabled both alerts and scheduled email, defined recipients receive both types of email.

-   You can define a list of recipients by selecting user or group names on the Specific Recipients subtab.
    
    -   For alerts, each specific recipient receives alerts for every record.
        
    -   For scheduled email, a single email message is sent to all specific recipients, with full search results embedded or attached.
        
-   You can derive recipients targeted to search results field values, so that users with matching values receive email. For example, for a Customer saved search, you could select the Sales Rep field.
    
    -   For alerts, each targeted recipient receives alerts only for matching records.
        
    -   For scheduled email, by default each targeted recipient receives an email with a summary of all matching record results. If the Summarize Scheduled Emails option is disabled, then each targeted recipient receives a separate email for each matching record result.
        
-   An alternate method for targeting recipients based on search results field values is to define a filter for search criteria, such as Sales Rep is Mine or Sales Rep is My Team, as well as selecting recipients on the Specific Recipients subtab. Email is sent only to users who match search criteria AND are listed as Specific Recipients. This option may allow more control than selecting fields on the Recipients from Results field.
    

#### To define specific saved search email recipients: {#procedure_N684646}

1.  Click the **Specific Recipients** subtab of a saved search **Email** subtab.
    
    For alerts, a separate alert email message is sent to each recipient for every record add and, if applicable, update. For groups: if a group defined as an alert recipient has an email address, the alert is sent to that address; otherwise alert emails are sent to individual addresses of group members.
    
    For scheduled email, on each scheduled date, a single email message is sent, with all specified recipients (except those marked Bcc) listed in the To field, and full search results included.
    
    Note:
    
    At least one recipient must not be flagged as Bcc so the emails would be received by the recipients.
    
    If a group defined as a scheduled search email recipient has an email address, that address is used in the To or Bcc fields of the message containing the results; otherwise individual email addresses for group members are used.
    
2.  Select a user or group in the **Recipient** field. Click the ![Recipient list icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/recipient1.png) button and select List to open the Choose Recipient dialog.
    
    ![Choose Recipient popup window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/recipient2.png)
    
    Notice that you can limit the list of possible recipients to a specific type: contacts, customers, employees, groups, partners, or vendors. By default all types are listed.
    
3.  (Alerts only) If you want this recipient to receive alerts for updates as well as adds, enable the Send on Update option.
    
4.  (Alerts only) If you have enabled the Send on Update option, and you want these alerts to include information about changes, enable the Show Recent Changes option.
    
5.  (Scheduled email only) If you do not want other users to see this recipient listed, enable the Bcc option.
    
6.  Click **Add**.
    
7.  Repeat these steps for other users and groups as necessary.
    

#### To derive saved search email recipients from search results: {#procedure_N684748}

1.  Click the **Recipients from Results** subtab of a saved search **Email** subtab.
    
2.  (Alerts only) If you want all recipients derived from results to receive alerts for updates as well as adds, enable the Send on Update option.
    
3.  (Alerts only) If you have enabled the Send on Update option, and you want these alerts to include information about changes, enable the Show Recent Changes option.
    
4.  Select a field from the Recipient Field dropdown list and click Add, repeating as necessary.
    
    Available options include entity and email type fields. For example, for a Customer saved search, you can select Sales Rep.
    
5.  (Scheduled email only) On each scheduled date, separate email messages are sent to all recipients who match search results values for the selected field(s). Each message includes only search results with values matching the recipient. By default, each recipient receives one message with a summary of all matching results.
    
    To send a separate email message for each matching result, rather than a summary of all matching results, to each recipient derived from results, disable the Summarize Scheduled Emails option.
    
    This option can be used for drip marketing.
    

#### To derive saved search email recipients from search filters: {#procedure_N684802}

1.  Click the **Standard** subtab of a saved search **Criteria** subtab.
    
2.  Select the field you want to use to target recipients, and in the popup that appears, select a field value.
    
    For example, for a Customer saved search, you can select the **Sales Rep** field and a value of Mine or My Team.
    
3.  Click the **Email** subtab and the **Specific Recipients** subtab.
    
4.  Select users from the Recipient dropdown list, clicking **Add** after each selection.
    
    Email is sent only to users who match search criteria AND are listed as Specific Recipients.
    

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html)
-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)
-   [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

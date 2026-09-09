---
id: "section_N681962"
type: "section"
title: "Enabling Saved Search Email Alerts"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Enabling Saved Search Email Alerts"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html"
anchors: ["procedure_N682121"]
sha256: "96580fddd6cd27456b4ebbc80f676077dbdd1e3d455a4d5f8260d008120daa8c"
---

Set up email alerts for a saved search so recipients and subscribers get email messages when search results are added or updated.

-   By default, alerts are triggered for new records that match criteria defined in the saved search. Enable the **Send on Update** option so that the alerts are triggered also when an existing record is updated to match criteria defined in the saved search. You can modify update alerts to add information about recent changes or send them only when certain fields or values change.
    
-   If a saved search is inactive, email alerts aren't triggered. The alerts still exist in the system, but no emails are sent.
    
-   You can't use alerts for all types of saved searches. For a full list, see [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html).
    
-   You can't use alerts for searches with summarized results. For more information, see [Summary Types for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659258.html).
    
-   Specify alert recipients by user or group name, or set up a search field to select recipients based on results, such as the Sales Rep field for a Customer search. For more information, see [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html).
    
-   To let more users receive email alerts, enable the **Public** and the **Allow Users to Subscribe** options. Users can then set their own alert preferences. For more information, see [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html).
    
-   You can customize much of the text for alert email messages. For information, see [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html).
    
-   You can specify the sender for saved search emails. See [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html).
    
-   Each record add or update sends a separate alert to each recipient. If a recipient group has an email address, the alert is sent there. Otherwise, alerts are sent to the individual addresses of the members.
    
-   Each alert usually shows one result, filtered by the record that triggered it. For searches with multiple results per record, you can include more. For information, see [Enabling Multi-Row Results for Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685250.html).
    
-   If a saved search that has an alert is in a bundle, the alert is not sent in target accounts where the bundle is installed. Enable the Enable Email Alerts for WS and CSV Imports preference for the alert to be sent. You can do that at _Setup > Company > Email > Email Preferences_.
    
-   Saved Search Email doesn't work with email capture features or plug-ins. Use an email address that isn't associated with a capture feature. For more information, see [Email Capture Plug-in Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4235218166.html).
    

Important:

By default, email alerts aren't sent for CSV imports updates or SOAP web services integrations updates. To enable them, an account administrator or a user with the Set Up Company permission can set the **Enable Email Alerts for WS and CSV Imports** preference at _Setup > Company > Email > Email Preferences_. See [Setting Printing and Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253916.html).

#### To enable email alerts for a saved search: {#procedure_N682121}

1.  On a saved search page's **Email** subtab, enable the **Send Email Alerts When Records are Created/Updated** option.
    
    If this option is not available, it means alerts aren't available for this type of search. For more information, see [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html).
    
2.  To allow other users to receive this search's alerts, enable the **Public** and **Allow Users to Subscribe** options.
    
    The **Public** option is available near the top of the page, only for administrators and other users with the Publish Search permission. The **Allow Users to Subscribe** option is on the **Specific Recipients** subtab. Users can subscribe to a search's alerts by setting a preference. For information, see [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html).
    
3.  To specify recipients by user name, group name, or both, click the **Specific Recipients** subtab.
    
    1.  Select a user or group in the **Recipient** field. Click the ![Expand recipient list icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/recipient1.png) button and select **List**. Notice that you can limit the list of possible recipients to a specific type: contacts, customers, employees, groups, partners, or vendors. By default all types are listed.
        
    2.  If you want this recipient to receive alerts for updates as well as adds, enable the **Send on Update** option.
        
    3.  If you have enabled the **Send on Update** option, and you want these alerts to include information about changes, enable the **Show Recent Changes** option.
        
    4.  Click **Add**.
        
    5.  Repeat these steps for other users and groups as necessary.
        
4.  To target recipients based on values of search results fields, click the **Recipients from Results** subtab.
    
    1.  If you want all recipients derived from results to receive alerts for updates as well as adds, enable the **Send on Update** option.
        
    2.  If you have enabled the **Send on Update** option, and you want these alerts to include information about changes, enable the **Show Recent Changes** option.
        
    3.  Select a field from the **Recipient Field** dropdown list and click **Add**, repeating as necessary.
        
        Available options include entity and email type fields. For example, for a Customer saved search, you can select Sales Rep.
        
5.  To filter update alerts to occur only for a subset of updates, click the **Updated Fields** subtab:
    
    1.  If you want alerts to be sent only when a particular field is updated, select the field from the dropdown list.
        
    2.  If you want alerts to be sent only when a particular old value (value before update) occurs for the selected updated field, enter that value.
        
    3.  If you want updates to be sent only for a particular new value (value after update) occurs for the selected updated field, enter that value.
        
    4.  Click **Add**.
        
    5.  Repeat these steps for other fields as necessary.
        
6.  To customize email message text, click the **Customize Message** subtab.
    
    1.  In the **From** field, enter optional custom text. You can include values from search results fields by entering field IDs enclosed in curly braces {fieldID}.
        
    2.  In the **Subject** field, enter optional custom text. You can include values from search results fields by entering field IDs enclosed in curly braces {fieldID}.
        
    3.  In the **Introduction** field, enter optional custom text to appear before search results.
        
    4.  Enter custom message body text in the **Single-Record Results** field.
        
        -   You can include values from search results fields in this text by entering field IDs enclosed in curly braces {fieldID}. Select a field in the **Insert Field** dropdown list to insert its field ID.
            
        -   Use the syntax <%=formula%> to add formulas to the text. Formulas can include {fieldID} references.
            
        -   You can define email body text as an entire HTML page (by enclosing it with HTML tags), to send email content exactly as specified, with no additional styles, View Record link, or introduction.
            
7.  Click **Preview**, **Save**, **Save & Run**, or **Save & Email**.
    

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html)
-   [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html)
-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)
-   [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

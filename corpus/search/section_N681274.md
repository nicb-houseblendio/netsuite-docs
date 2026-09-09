---
id: "section_N681274"
type: "section"
title: "Enabling Saved Search Scheduled Email"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Enabling Saved Search Scheduled Email"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html"
anchors: ["procedure_N681392"]
sha256: "bc77f507733a9f08e15cf35487a8967d2ba82e057065255abf62e71ed224c508"
---

Set up a schedule to email saved search results to yourself and other users on certain dates or at regular intervals. This option works well for:

-   Searches that take a long time to run. For exceptionally long searches, consider persisting search results. For more details, see [Persisting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1029112142.html).
    
-   Regular status updates. Send full results to some users, and filtered results to others.
    

Add recipients by user name or group name, or use a field like **Sales Rep** to set recipients based on search results. For more information, see [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html).

If a Saved Search is inactive, the schedules don't run. Both the search and the schedule still remain, but no email is sent.

To avoid sending emails for searches with no results, disable the **Send if No Results** option on the **Email** subtab. For information, see [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html).

By default, targeted scheduled emails send a summary of each user's results in one email message on each scheduled date. You can change it to send a separate email for each result, so that each user receives multiple messages on each date. This is useful for activities like drip marketing. For more information, see [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html).

Customize the email text and choose to embed results or to attach a .csv or .xls file. For more information, see [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html).

Set the sender for saved search emails. See [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html).

Scheduled saved search emails in your production account don't run in the Release Preview account. To email results from the Release Preview account, set up the schedule there.

Warning:

Only one scheduled saved search can run at a time per user, up to 200 simultaneously per NetSuite account. If you schedule too many saved searches for the same time, only one runs and the rest are set on hold. This may block the scheduling process. If this happens, update the schedules to cancel all waiting processes. You can avoid this issue by scheduling searches at different times.

#### To enable scheduled email for a saved search: {#procedure_N681392}

1.  On the saved search page's **Email** subtab, enable the **Send Emails According to Schedule** option.
    
2.  To set up the schedule for sending emails, click the **Schedule** subtab.
    
    1.  Select the interval at which you would like to send emails, or click **Single Event** to send it only one time.
        
    2.  Each interval gives further options. For example, **Weekly Event** lets you choose which day to send the results.
        
    3.  Choose a start date as the first day the results are emailed.
        
        For monthly or weekly events, be sure the **Start Date** matches the interval choice. For example, for a start date of 9-8-2025, which is a Monday:
        
        -   For a monthly event, the day of the start date should match the selection in the option buttons. In this example, you should enter 8 for **Day**, if this option is selected, or select the second Monday.
            
        -   For a weekly event, the day of the start date should match the selected day of the week. In this example, you should check the **Monday** box.
            
    4.  Set a start time. This is the time of day that the search is run and its results are emailed.
        
    5.  Set an end date in the **End By** field, or check the **No End Date** box to continue running the search and emailing its results indefinitely.
        
3.  To specify recipients by user name, group name, or both, click the **Specific Recipients** sublist.
    
    Each scheduled time, an email message goes out to all the recipients listed in the **To** field (except those marked as Bcc) with full results. If a group that has an email address is chosen, that address is used in the **To** or **Bcc** fields of the message. Otherwise, the individual addresses of the members are used.
    
    1.  In the **Recipient** field, select a user or group. Click the ![Expand arrows icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/ArrowList.png) button and select ![List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/list.png)**List** to open a dialog. You can limit options to a specific type: contacts, customers, employees, groups, partners, or vendors. All types are listed by default.
        
    2.  To hide the recipient from others, use the **Bcc** option.
        
    3.  Click **Add**.
        
    4.  Repeat these steps for other users and groups as needed.
        
4.  To target recipients using results fields values, go to the **Recipients from Results** sublist.
    
    On each scheduled date, recipients that match a field get separate email messages. These messages include only the results with values that match the recipient. By default, each recipient receives a message with a summary of the results.
    
    1.  Select a field from **Recipient Field** and click **Add**, repeating as necessary.
        
        Available options include entity and email type fields. For example, for a Customer saved search, you can select Sales Rep.
        
    2.  To send separate messages for each result to each recipient instead of a summary, disable the **Summarize Scheduled Emails** option.
        
        This option can be used for drip marketing.
        
5.  To customize the message text, click the **Customize Message** subtab.
    
    Some options apply to all emails, others only work for single-record results (when the **Summarize Scheduled Emails** option has been disabled).
    
    1.  In **From**, enter the sender's name and email address. For required format details, see [Required Format for Saved Search Email Sender](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html#bridgehead_N684272).
        
    2.  In **Subject**, enter the custom text. For single-record results, you can add field values by entering field IDs enclosed in curly braces {fieldID}.
        
    3.  In **Introduction**, add custom text to appear before the results.
        
    4.  For single-record results only, add custom message body text in the **Single-Record Results** field.
        
        -   Add field values by entering field IDs enclosed in curly braces {fieldID}. Select a field in the **Insert Field** dropdown list to insert its field ID.
            
        -   Use <%=formula%> to add formulas, these can use {fieldID} references.
            
        -   You can define email body text as an entire HTML page by enclosing it with HTML tags. Use this to send email content exactly as specified, with no additional styles, View Record link, or introduction.
            
    5.  Select one of the following options to send the results:
        
        -   **Send within Message** - Embeds the results in the message.
            
        -   **Send as CSV** - Sends the results attached as a .csv file.
            
        -   **Send as Microsoft ® Excel** - Sends the results attached as an .xls file.
            
        -   **Send as Tableau ® Workbook** - Sends the results attached as a Tableau Workbook file.
            
        
        Note:
        
        This option doesn't apply to single-record results.
        
    6.  If you don't want to include a separate link for each row, disable **Include View Record Link**. When this option is disabled, one single link appears at the bottom. When it's enabled, a link appears for each row/record.
        
6.  Click **Preview**, **Save**, **Save & Run**, or **Save & Email**.
    

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html)
-   [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html)
-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)
-   [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

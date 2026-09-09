---
id: "section_N684976"
type: "section"
title: "Customizing Saved Search Email Content"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Customizing Saved Search Email Content"
parent: "section_N680983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html"
anchors: []
sha256: "bf3a131bd9338d54786ac6c3c80917a210ad56831ed6bcd76349b4702425df24"
---

You can customize much of the text for scheduled and alert email messages. Some customizations are available only for emails containing results from one record, referred to as single-record results, meaning all alerts, and scheduled emails to recipients derived from the Recipients from Results subtab when the Summarize Scheduled Emails option is disabled. An option to choose whether to include search results as embedded content, as an attached .csv file, or as an attached .xls file applies to scheduled email with full or summarized results.

To customize text, click the Customize Message subtab of a saved search Email subtab:

-   In the **From** field, enter an optional sending email address.
    
    -   Your entry in this field must use the following format: **'name' <email address>**. For details, see [Required Format for Saved Search Email Sender](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html#bridgehead_N684272).
        
    -   For single-record results only, you can include values from search results fields by entering field IDs enclosed in curly braces **{fieldID}**.
        
    -   If the **From** field is blank, email messages are sent from the email address defined in the search owner's employee record. For details, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).
        
    -   If the **From** field is blank, and no email address is set in the search owner's employee record, email messages are sent from the email address defined in the **Return Email Address field** at _Setup > Company > Company Information_. For details, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).
        
-   In the **Subject** field, enter optional custom text. For single-record results only, you can include values from search results fields by entering field IDs enclosed in curly braces **{fieldID}**.
    
-   In the **Introduction** field, enter optional custom text to appear before search results.
    
-   For single-record results only, enter custom message body text in the **Single-Record Results** field.
    
    -   You can include values from search results fields in this text by entering field IDs enclosed in curly braces **{fieldID}**. Select a field in the **Insert Field** dropdown list to insert its field ID.
        
    -   Use the syntax **<%=formula%>** to add formulas to the text. Formulas can include **{fieldID}** references.
        
    -   You can define email body text as an entire HTML page (by enclosing it with HTML tags), to send email content exactly as specified, with no additional styles, View Record link, or introduction.
        
    -   You cannot enter more than 4000 characters as custom message body text.
        

Note:

You can include multiple matching rows in a saved search alert email by using a {results} parameter in the text for the **Single-Record Results** field. See [Enabling Multi-Row Results for Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685250.html).

-   Select an option button to indicate whether search results should be: embedded in the email message, attached as a CSV file, attached as an XLS file, or attached as a PDF file.
    
    (This option is unavailable to single-record results.)
    
-   If you do not want to include a separate record link for each results row, disable the **Include View Record Link** option. When this option is disabled, one link appears at the bottom.
    

### Related Topics

-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html)
-   [Canceling Scheduled Saved Search Emails When No Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681801.html)
-   [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html)
-   [Types of Saved Searches Available for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682531.html)
-   [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html)
-   [Defining the Sender for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684160.html)
-   [Defining Recipients for Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684570.html)
-   [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

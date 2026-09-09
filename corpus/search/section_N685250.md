---
id: "section_N685250"
type: "section"
title: "Enabling Multi-Row Results for Email Alerts"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Email > Customizing Saved Search Email Content > Enabling Multi-Row Results for Email Alerts"
parent: "section_N684976"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685250.html"
anchors: []
sha256: "7a8ac57e7e7601ba57d8e10db85a0b35961dc04aabdfe2d8f485097926bfd874"
---

Normally, each saved search alert email includes only one row, because the search is filtered by the triggering record. However, certain searches, such as those with results fields from one-to-many joins, or transaction searches, can return multiple rows for each triggering record.

In this case, you can include multiple matching rows in each alert email by using a {results} parameter in the text for the Single-Record Results field.

The following procedure provides steps for how you could set up a search alert in these instances:

#### To enable multi-row results for email alerts:

Warning:

The {results} parameter cannot be used in a scheduled saved search email that is not summarized, because the results are all single rows sent out individually. For this type of email, instead of adding the {results} parameter, use the Insert Field dropdown list to insert a field ID enclosed in curly braces for each column for which you want results returned. See [Sending Summarized vs. Single-Record Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685536.html) and [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html).

1.  Go to _Reports > Saved Searches > All Saved Searches > New_.
    
2.  On the New Saved Search page, select Transaction.
    
3.  On the Saved Transaction Search, go to the Standard subtab of the Criteria subtab.
    
    1.  Select Type from the Filter dropdown list and in the popup, select Sales Order and click Set.
        
    2.  Select Main Line from the Filter dropdown list and in the popup, choose No and click Set. (This choice means that the search will return transaction line items but not the transaction header.)
        
4.  Click the Results subtab.
    
    1.  Select Item from the Field dropdown list and click **Add**.
        
    2.  Select Quantity from the Field dropdown list and click **Add**.
        
    3.  Select Amount from the Field dropdown list and click **Add**.
        
    4.  Select each additional field that is listed and click **Remove**.
        
5.  Click the Email subtab.
    
    1.  Enable the Send Email Alerts When Records are Created/Updated option.
        
    2.  Click the Specific Recipients subtab and select user or group names, clicking Add after each one.
        
    3.  Click the Customize Message subtab. In the Single-Record Results field, enter the following text:
        
        **Here are the items of the order: <CR><CR> {results}**
        
        Note that each <CR> indicates a carriage return.
        
6.  Click **Preview**, **Save**, **Save & Run**, or **Save & Email**.
    
    Each alert email includes all rows for each transaction.
    

### Related Topics

-   [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

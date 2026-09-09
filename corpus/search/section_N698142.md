---
id: "section_N698142"
type: "section"
title: "Creating a Search Email Alert for De-escalated Cases"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating a Search Email Alert for De-escalated Cases"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N698142.html"
anchors: ["procedure_N698164"]
sha256: "951e7c732f30549c143efa008fa7f1156f9c9ed66ddabff2acf1ac9b1ca7c837"
---

You can create a saved search with an email alert that sends email to assigned support reps when cases are de-escalated

#### To send alerts for de-escalated cases: {#procedure_N698164}

1.  Click Saved Searches > New to open a Saved Case Search page.
    
2.  Enter a descriptive Search Title, such as De-escalated Case Alert.
    
3.  On the **Criteria** subtab, in the Filter dropdown list:
    
    1.  Select **System Notes** fields, select Date, select 'on' and 'today', and click Set.
        
    2.  Select **System Notes** fields again, select Old Value, select 'contains' and 'escalated', and click Set.
        
4.  Set up an email alert for the search on the **Email** subtab.
    
    1.  Check the **Send Email Alerts When Records are Created/Updated** box.
        
    2.  On the **Recipients from Results** subtab, check Send on Update, and select Assigned To from the Recipient Field dropdown list.
        
    3.  On the **Updated Fields** subtab, select Status from the Field dropdown list, and type 'Escalated' for the old value.
        
5.  Save the search.
    

For more information about creating saved search email alerts, see [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html).

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

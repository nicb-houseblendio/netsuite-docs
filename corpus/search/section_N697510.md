---
id: "section_N697510"
type: "section"
title: "Creating a Search Email Alert for Leads Created through Online Forms"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating a Search Email Alert for Leads Created through Online Forms"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N697510.html"
anchors: ["procedure_N697531"]
sha256: "0bbe0f57af6ba5d088a4dbcbcd7c532c4b96048a34eee0236a0fc3ee8cf6b658"
---

You can create a saved search with an email alert that sends customized email to Sales Reps when new leads are created through online forms.

#### To send alerts for leads from online forms: {#procedure_N697531}

1.  Create a lead source (campaign) for the online form. For details about how to do this, see [Lead Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N975884.html).
    
2.  Create an online form.
    
    1.  Set Send Email Notification to False.
        
    2.  Set Lead Source to the name of the online form.
        
    3.  Set up other values for the online form as needed. For details, see [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html).
        
3.  Create a new customer saved search.
    
    1.  Click Saved Searches > New to open a Saved Customer Search page.
        
    2.  Enter a descriptive Search Title.
        
    3.  On the **Criteria** subtab, in the Filter dropdown list, select Lead Source, and in the popup, select the online form name and click Set.
        
4.  Set up an email alert for the search on the **Email** subtab.
    
    1.  Check the **Send Email Alerts When Records are Created/Updated** box.
        
    2.  On the Recipients from **Results** subtab, select Sales Rep from the Recipient Field dropdown list.
        
    3.  On the **Customize Message** subtab, customize the message text as needed, for example by adding CRMSDK tags. For details, see [Customizing Saved Search Email Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N684976.html).
        
5.  Save the search.
    

For more information about creating saved search email alerts, see [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html).

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Capturing Leads](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N973827.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

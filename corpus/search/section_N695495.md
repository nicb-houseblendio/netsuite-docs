---
id: "section_N695495"
type: "section"
title: "Creating a Campaign Response Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating a Campaign Response Search"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N695495.html"
anchors: ["procedure_N695521"]
sha256: "d315fb15c11df46e0a800793fa90af4aa064aa5d115395d83ec680829eb91f41"
---

You can create a saved search to review responses to email marketing campaigns. This search lets you obtain a list of recipients who did not open emails or did not receive them because they were bounced. Then you can resend campaign emails to these recipients.

#### To create a saved search of campaign non-respondees: {#procedure_N695521}

1.  Click Saved Searches > New to open a Saved Customer Search page.
    
2.  Enter a descriptive Search Title.
    
3.  On the **Criteria** subtab, define a filter for a specific campaign:
    
    1.  In the Filter dropdown list, scroll down and select **Campaign Response Fields**.
        
    2.  In the first popup, select Title.
        
    3.  In the second popup, enter the name of the marketing campaign, and click **Set**.
        
4.  Next, define a filter for responses:
    
    1.  In the Filter dropdown list, scroll down and select **Campaign Response Fields**.
        
    2.  In the first popup, select Response.
        
    3.  In the second popup, press Ctrl and select one or more responses, and click Set.
        
5.  On the **Results** subtab, select the fields you want to appear in the results list. It would be helpful to include **Campaign Response:Response**, and perhaps to sort by this field.
    
6.  If you want to be able to dynamically filter results list records by campaign response, you can select the **Campaign Response:Response** field on the **Available Filters** subtab and check the **Show in Filter Region** box.
    
    You then will be able to select a single response, such as Bounced, from a dropdown list in the results list filter area and view only customers with bounced responses for the selected campaign.
    
7.  Enter any other search definitions that you want to include.
    
8.  Save the search.
    

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)
-   [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

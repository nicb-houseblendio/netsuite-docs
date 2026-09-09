---
id: "section_N696025"
type: "section"
title: "Creating an Average Items Per Order Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating an Average Items Per Order Search"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N696025.html"
anchors: ["kaltura_player_43", "procedure_N696048"]
sha256: "806375041e375763996cd79e21a73c56136f3abfc5c74331aac51b257fb386fe"
---

You can create a saved search to obtain the average number of unique items per sales order. A maximum type summary result field with a formula calculates this amount.

Watch the following video for a tutorial on how to create a saved search that calculates the average number of items per order.

<a id="kaltura_player_43"></a>

#### To create a saved search of average items per order: {#procedure_N696048}

1.  Click Saved Searches > New to open a Saved Transaction Search page.
    
2.  Enter a descriptive Search Title.
    
3.  On the **Criteria** subtab in the Filter dropdown list:
    
    1.  Select Type, choose Sales Order in the popup, and click **Set**.
        
    2.  Select Main Line, choose No in the popup, and click **Set**.
        
    3.  Select Shipping Line, choose No in the popup, and click **Set**.
        
4.  On the **Results** subtab's **Columns** subtab:
    
    1.  Select Formula (Numeric).
        
    2.  Select a Summary Type of Maximum.
        
    3.  Select a Function of Round to Hundredths.
        
    4.  Enter a Formula as follows:
        
        max(1)\*count(distinct {item}||','||{internalid})/count(distinct {internalid})
        
    5.  (Optional) Enter a custom label for the formula.
        
5.  To enable use of the saved search as a custom KPI, click the **Available Filters** subtab and select a Date field from the Filter dropdown list.
    
    This filter lets you compare search results for different date ranges, display them as KPIs, and even illustrate them in trend graphs.
    
    If you want to include a dropdown list date selector on results pages, check the **Show in Filter Region** box.
    
6.  Enter any other search definitions that you want to include.
    
7.  Save the search.
    

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

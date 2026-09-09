---
id: "section_N696584"
type: "section"
title: "Creating a Daily Inventory Additions Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating a Daily Inventory Additions Search"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N696584.html"
anchors: ["procedure_N696601"]
sha256: "702a4bbb87a8c5f9099ae57cf8ce46795625b039ff9229532b09bd122d1e581e"
---

You can create a saved search that provides the names and quantities of items added to inventory each day.

#### To create a daily inventory additions search: {#procedure_N696601}

1.  Go to _Reports > Saved Searches > All Saved Searches > New_ and click **Transaction**.
    
2.  Enter a descriptive search title.
    
3.  On the **Criteria** subtab, add the following filters to the **Filter** column:
    
    1.  **Date** - Set the date to be **today**.
        
    2.  **Account** - Select your inventory account.
        
    3.  **Posting** - Select a **Yes** value for this filter.
        
    4.  **Formula (Numeric)** - In the **Formula** field, type **{quantity}**, set **Formula (Numeric)** to **greater than** and **Value** to **0**.
        
4.  On the **Results** subtab's **Columns** subtab, add the following fields:
    
    1.  **Item** - Select a **Summary Type** of **Group** for this field.
        
    2.  **Quantity** - Select a **Summary Type** of **Sum** for this field.
        
    3.  Add and remove other fields as needed.
        
5.  Complete other subtabs as needed.
    
6.  Save the search.
    

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

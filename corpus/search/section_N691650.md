---
id: "section_N691650"
type: "section"
title: "Creating Saved Searches for Bin Numbers"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating Saved Searches for Bin Numbers"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691650.html"
anchors: ["bridgehead_N691701", "procedure_N691718", "bridgehead_N691797", "procedure_N691819"]
sha256: "9323dd514b3239f8291488fdf83c78e60bf792ce53ccc3050fae4be8aa4eebf6"
---

You can return bin number data for transaction and item searches. The following fields are available as criteria and results:

-   For transaction searches: Transaction Bin Number, Transaction Bin Quantity
    
-   For item searches: Bin Number, Bin on Hand Count, Bin on Hand Available, Preferred Bin (whether the bin is the preferred bin for the location)
    
-   Other Bin Number record fields are available as join fields for both transaction and item searches.
    

## Creating a Transaction Bin Numbers Search {#bridgehead_N691701}

The following search returns all transactions that use bins, and indicate the quantities moved between bins.

#### To create a transaction saved search with bin number data: {#procedure_N691718}

1.  Start a transaction saved search.
    
2.  On the **Criteria** subtab, select **Transaction Bin Number** in the Filter field.
    
3.  In the popup window, select 'is not empty' in the dropdown list and click **Set**.
    
4.  On the **Results** subtab, select the following fields in the **Field** column, clicking Add after each one: **Date**, **Type**, **Transaction Number**, **Amount**, **Transaction Bin Number**, and **Transaction Bin Quantity**. (You can remove other selected fields as necessary.)
    
5.  Click **Preview** or **Save & Run** to view your search results.
    

## Creating an Item Bin Numbers Search {#bridgehead_N691797}

The following search returns all items that use bins and includes all bin information, including bin numbers, quantity on hand, quantity available, whether bin is preferred, and if multi-location inventory is in use, location.

#### To create an item saved search with bin number data: {#procedure_N691819}

1.  Start an item saved search.
    
2.  On the **Criteria** subtab, select Bin Number in the **Filter** field.
    
3.  In the popup window, select 'is not empty' in the dropdown list and click Set.
    
4.  On the **Results** subtab, select the following fields in the **Field** column, clicking Add after each one: **Name**, **Type**, **Base Price**, **Bin Number**, **Bin On Hand Count**, **Bin On Hand Available**, and **Preferred Bin**. (You can remove other selected fields as necessary.)
    
5.  In the **Field** column, scroll down through all fields and click **Bin Number** fields. In the popup, click Add Multiple, select Location and Memo, and click Add.
    
6.  Click **Preview** or **Save & Run** to view your search results.
    

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

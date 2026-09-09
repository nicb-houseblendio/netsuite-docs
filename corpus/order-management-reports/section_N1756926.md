---
id: "section_N1756926"
type: "section"
title: "Enabling the Gross Profit Feature"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Setting Up Gross Profit > Enabling the Gross Profit Feature"
parent: "section_N1756747"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756926.html"
anchors: ["procedure_N1756941"]
sha256: "b0652979d458206077e79e582c4400a91d3f15becc4fde685a7345c98a6a8b7f"
---

#### To enable the Gross Profit feature: {#procedure_N1756941}

1.  Go to _Setup > Company > Enable Features_.
    
2.  On the **Transactions** subtab, in the Sales section, check the **Gross Profit** box.
    
3.  Enable other features as desired.
    
    The Gross Profit feature is not directly dependent on other features, but may have limited utility without them. For example, the following related features can affect user access to gross profit data:
    
    -   **Inventory** - required for certain item types and costing information
        
    -   **Sales Orders, Opportunities, Estimates** - required to get gross profit data for these transaction types
        
    -   **Project Management** - required to get job costing information on sales transactions
        
    -   **Drop Shipments & Special Orders, Purchase Orders** - required to use the Purchase Order Rate cost estimate type.
        
4.  Click **Save**.
    

When you enable the Gross Profit feature, related fields become available as follows:

-   Gross profit fields automatically become available on standard transaction forms. For details, see [Using Gross Profit Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html).
    
-   If you use custom transaction forms in your business, you must add gross profit fields to these forms to see them. See [Creating Custom Transaction Form HTML Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873464.html#subsect_163733107381).
    
-   Gross profit fields are available for use in custom reports, advanced and saved searches, and custom KPIs. See [Including Gross Profit Values in Reports, Searches, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1763752.html).
    
-   Gross profit fields are available for CSV import, SOAP web services integrations, and SuiteScript. See [Using Gross Profit Values in CSV Import, SOAP Web Services, and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html).
    

The Cost Estimate Type field is available on item records and on transaction item lines. For information about setting values for this field, see [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html).

Warning:

If you later disable the Gross Profit feature, gross profit fields are no longer included in forms, reports, and searches. Also, any SuiteScripts and SOAP web services integrations that use these fields no longer function correctly.

### Related Topics

-   [Setting Up Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756747.html)
-   [Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html)
-   [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

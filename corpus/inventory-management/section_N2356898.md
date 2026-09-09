---
id: "section_N2356898"
type: "section"
title: "Demand History by Item Report"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Reporting > Demand History by Item Report"
parent: "chapter_N2353200"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2356898.html"
anchors: ["bridgehead_N2356963"]
sha256: "04286f015da68a1b897980a92468c66eece87cb527cb24fcb03db7965258fd63"
---

The Item Demand History by Item report shows the demand history for your items as the number of units sold over time. The demand history shown is the historical data that is used for analysis in demand calculations.

To see demand across a specific period, select a range in the date field, or enter a custom date range.

The historical demand displayed is based on the Transactions to Consider preference. This determines the transactions that are included in demand calculations.

-   If your setting is Orders, then demand is calculated using approved, non-canceled sales orders. If you use the Assemblies feature, then work orders are considered also.
    
-   If your setting is Actual Sales, demand is calculated using cash sales and invoices. Sales orders are _not_ used to calculate demand. If you use the Assemblies feature, then assembly builds are considered also.
    

Inventory demand calculations consider only transactions that decrease an item's stock level. For example, an assembly build increases the stock level for the assembly item and decreases the stock level for the assembly item's components. In this case, the demand plan calculation considers the assembly build only for the assembly item's components and not for the assembly item.

For details about setting this preference, read [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html).

## To see the item demand history by item report: {#bridgehead_N2356963}

Go to _Reports > Demand Planning > Item Demand History by Item_.

A message appears indicating that your report is loading. The status bar indicates the progress as your report loads. You can click **Cancel Report** to stop the report from loading.

To see demand across a specific period, select a range in the Date field or enter a custom date range.

### Related Topics

-   [Item Demand Plan by Item Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2357062.html)
-   [Item Demand Forecast vs. Actual Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2357186.html)
-   [Gross Requirements Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295603.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

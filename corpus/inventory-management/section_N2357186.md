---
id: "section_N2357186"
type: "section"
title: "Item Demand Forecast vs. Actual Report"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Reporting > Item Demand Forecast vs. Actual Report"
parent: "chapter_N2353200"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2357186.html"
anchors: ["bridgehead_N2358369"]
sha256: "291b04efad4d931ecfcd5ffbb4b8fca1bda59c0aec7c659ec9c777e9a25a2092"
---

The Item Demand Forecast vs Actual report shows the forecasted demand for an item versus demand for the item across a certain period. This report helps you determine the accuracy of the forecast as well as whether supply or pricing needs to be adjusted for an item.

For example, the forecast predicted a spike in sales for the month. However, sales remained flat. Therefore, adjustments may be needed to your forecasting values.

Additionally, you can make short-term assessments about supply and pricing adjustments:

-   In a demand-pull environment, a discrepancy between the forecast and actual numbers may imply that the production or procurement amount needs to be adjusted.
    
-   In a supply-push environment, a discrepancy between the forecast and actual numbers may imply that the price needs to be adjusted. This adjustment should be based on the expected amount being produced or procured. For example, an item with a large amount of unexpected overstock can be placed on sale with a special price.
    

You can display demand for an item by the week or by the month.

The historical demand displayed is based on your setting for the Transactions to Consider preference. This determines the transactions that are included in demand calculations.

-   If your setting is Orders, then demand is calculated using approved, non-canceled sales orders.
    
-   If your setting is Actual Sales, then demand is calculated using cash sales and invoices. Sales orders are _not_ used to calculate demand.
    

For details about setting this preference, read [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html).

## To see the item demand forecast vs. actual report: {#bridgehead_N2358369}

Go to _Reports > Demand Planning > Item Demand Forecast vs Actual_.

A message appears indicating that your report is loading. The status bar indicates the progress as your report loads. You can click **Cancel Report** to stop the report from loading.

To see demand across a specific period, select a range in the Date field or enter a custom date range.

Note:

This report does not support reporting by period even when the Report by Period preference is set to All Reports. The Report by Period preference can be configured at _Home > Set Preferences_, on the Analytics subtab.

### Related Topics

-   [Demand History by Item Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2356898.html)
-   [Item Demand Plan by Item Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2357062.html)
-   [Gross Requirements Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295603.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

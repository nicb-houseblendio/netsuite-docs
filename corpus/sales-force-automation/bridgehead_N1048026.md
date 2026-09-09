---
id: "bridgehead_N1048026"
type: "bridgehead"
title: "Advanced Forecasting With Multiple Projected Amounts"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Sales Forecasting > Opportunities in the Forecast and Pipeline > Advanced Forecasting With Multiple Projected Amounts"
parent: "section_N1047903"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1048026.html"
anchors: ["bridgehead_157245274604"]
sha256: "6f822dd16515ee95e6f21a70f5a3d08a016b8e736d0ff8766061b616c8ca9820"
---

If your company uses the Multiple Projected Amounts preference, you can designate a range of projected values for each opportunity. Set this preference at _Setup > Sales > Preferences > Sales Preferences_.

The lower amount in the projected range represents the low, or worst case, forecast amount. The higher amount represents the high, or upside, forecast amount. The Projected Total field represents the middle, or most likely, forecast amount.

The forecast type you choose for an opportunity determines which amount NetSuite includes in the forecast according to the following:

-   NetSuite includes Worst Case opportunities and estimates in each forecast category.
    
-   NetSuite includes opportunities in the Most Likely category in the Most Likely and the Upside forecasts.
    
-   NetSuite includes opportunities in the Upside category in the Upside forecast.
    

With the Multiple Projected Amount preference enabled, NetSuite includes the projected amount in each category in the corresponding forecast category.

The following example explains how NetSuite calculates an opportunity's total based on the forecast type you select.

## Example {#bridgehead_157245274604}

A Wolfe Electronics sales rep enters an opportunity record for a customer. After selecting the items the customer is interested in, the projected total for the opportunity is calculated to $2000.

The rep thinks the deal could be worth half that amount or potentially worth more. In the Range fields the rep enters a lower amount of $1000 and a higher amount of $3000.

The forecast amounts for this opportunity are:

-   Worst case - $1000
    
-   Most likely - $2000
    
-   Upside - $3000
    

The amount NetSuite uses to calculate the forecast amount of this opportunity depends on the forecast type the rep assigns to the opportunity.

| Forecast type | Worst Case Forecast | Most Likely Forecast | Upside Forecast |
| --- | --- | --- | --- |
| Worst Case | $1000 | $2000 | $3000 |
| Most Likely |  | $2000 | $3000 |
| Upside |  |  | $3000 |

If you track weighted forecasts, NetSuite includes the weighted amount of opportunities and estimates in each category in the forecast.

### Related Topics

-   [Sales Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1045230.html)
-   [Advanced Forecasting Without Multiple Projected Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1048380.html)
-   [Advanced Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047034.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

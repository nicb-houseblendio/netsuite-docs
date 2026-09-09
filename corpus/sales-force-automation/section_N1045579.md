---
id: "section_N1045579"
type: "section"
title: "Setting Up Sales Forecasting"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Sales Forecasting > Setting Up Sales Forecasting"
parent: "chapter_N1045230"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1045579.html"
anchors: ["bridgehead_N1045591", "bridgehead_N1045643", "bridgehead_N1045666", "bridgehead_N1045681", "bridgehead_N1045900", "bridgehead_N1046047"]
sha256: "c601f634d41cd9d35c0a749144db8ec6f798a36f45e2a2d91ab344bef1895d3c"
---

The NetSuite forecasting feature doesn't require a lot of setup. As sales reps create opportunities and close deals, NetSuite automatically adds these amounts to your sales forecast. To further customize this feature, see [Forecasting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046772.html).

## The Calculated Forecast {#bridgehead_N1045591}

NetSuite calculates your sales forecast as the sum of the following:

-   Opportunities with no estimates attached or with estimates that are not set to be included in the forecast
    
-   Estimates set to be included in the forecast that have not been converted to closed sales
    
-   Unbilled sales orders that have not been converted to cash sales or invoices
    
-   Cash sales and invoices within the time period you are forecasting
    

If you use weighted forecasting, the calculated amount for each opportunity or estimate is multiplied by the probability of close. For example, an opportunity with a total of $1000 and a 40% probability of close would have a weighted forecast amount of $400.

## Forecasting Updates and Overrides {#bridgehead_N1045643}

No one knows their sales forecast better than the sales rep. If the calculated forecast does not match what a sales rep anticipates for their sales numbers, they can override the forecast with the Forecast Editor.

When a rep saves their forecast, NetSuite creates a snapshot of the rep's best prediction of their sales at that point in time. To ensure that the company-wide forecast is accurate, reps should review and update their forecasts regularly.

Sales managers can use the Manager Forecast Editor to enter override forecasts that roll up into reports viewed by successive levels of your organization. The Manager Forecast Editor relies on sales managers' judgement and experience to assess the accuracy of individual reps' sales and pipeline reports.

Sales reps cannot see manager overrides to their forecasts. Sales reps continue to work for the best deal they can close regardless of what the manager thinks is a more likely outcome.

## Three-tiered Probability System {#bridgehead_N1045666}

When sales reps create opportunities and estimates, they place each record into one of three categories: worst case, most likely, and upside. These categories, which you can rename as required, indicate how likely it is that a deal will close. Use worst case for deals that are likely to close. Use upside for deals that are not likely to close. Use most likely for deals that are somewhere in between the other two categories.

This three-tiered probability system gives the sales rep initial control over how an opportunity is reflected in the forecast, so you get more accuracy as soon as the rep enters the opportunity.

## Forecast KPIs and Snapshots {#bridgehead_N1045681}

With NetSuite you can view real-time forecast Key Performance Indicators (KPIs) and Snapshots on your dashboard. This includes closed sales and recurring revenue as well as the opportunities and quotes in your pipeline.

You can show a variety of forecast key indicators and snapshots that provide an accurate view of your forecast numbers.

You can view many different forecast snapshots on your dashboard, including, but not limited to:

| Snapshot | Description |
| --- | --- |
| Total Open Estimates | Shows the estimates (quotes) that are open as of the date you select. |
| Total Open Opportunities | Shows the opportunities that are open as of the date you select. |
| Forecast by Status | Shows a forecast divided by customer status, which provides a sense of where potential sales are in the sales cycle. |
| Sales Reps by Forecast | Shows the top sales reps by forecast for the date range you choose. |

When you are logged in as sales manager, you'll see forecast and quota key indicators for your team. Sales reps see their personal forecast and quota amounts.

You can also include [Historical Metrics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1051008.html) in your forecast snapshots and reports.

To add key performance indicators and snapshots, go to Home and click **Personalize**. For more information, see [Dashboard Personalization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N578457.html).

## Sales Management Snapshots {#bridgehead_N1045900}

You can add sales management report snapshots as dashboard portlets. These show real-time sales, forecast, and order totals, visible by the sales team.

The following portlets are available:

| Portlet | Description |
| --- | --- |
| Sales Managers by Forecast | Shows the sales forecast for each sales team. |
| Sales Managers by Sales Orders | Shows the approved sales order totals for each sales team. |
| Sales Managers by Sales | Shows the sales totals for each sales team. |

#### To show sales management snapshots: {#bridgehead_N1046047}

1.  On your Home tab, click **Personalize**.
    
2.  In the Standard Content frame, click on **Report Snapshots**. A report snapshots portlet will appear on your dashboard.
    
3.  Click on the three dots in the top right corner of the portlet and select **Set Up**. A Report Options pop-up window will appear.
    
4.  In the **Snapshot** field, select the sales management report you want to see: Sales Managers by Forecast, Sales Managers by Sales Orders, or Sales Managers by Sales.
    
5.  Select the hierarchy level.
    
6.  Click **Save**.
    

Click the icon next to a manager to expand or collapse the sales team. Click a currency amount or the three dots in the top right corner of the portlet and then the **View Report** link to open a report relevant to the snapshot. For example, when you click a forecast amount for a sales rep, the Sales by Sales Rep Detail report opens.

### Related Topics

-   [Forecasting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046772.html)
-   [A Sales Person's Guide to Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046401.html)
-   [Forecasting Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046608.html)
-   [Advanced Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047034.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

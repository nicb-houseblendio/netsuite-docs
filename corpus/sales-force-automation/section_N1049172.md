---
id: "section_N1049172"
type: "section"
title: "Saving Sales Rep Forecasts"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Sales Forecasting > Saving Sales Rep Forecasts"
parent: "chapter_N1045230"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049172.html"
anchors: ["procedure_N1049298"]
sha256: "fb5f45c78f9c65014e77b8bb7bbaa0a6c4ebf145791f14d9c4f34d10d0b8217a"
---

Sales reps can use the Forecast Editor to:

-   view the transactions in their sales forecast
    
-   enter an override forecast, if needed
    
-   adjust the probability and status of opportunities in the forecast
    

Any changes you make to a forecast updates the forecast amounts in your forecast reports. For more information about forecast reports, see [Forecast Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1051173.html).

If you use the Alternate Sales Amount (ASA) feature, you can track one forecast based on sales amounts and another forecast based on ASA. For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).

If you use NetSuite OneWorld, you can save one forecast per sales rep for each subsidiary. For example, if your company has three subsidiaries, a sales rep can save a different forecast for each of these subsidiaries.

If you use the Team Selling feature, sales reps can only edit transactions where they are the primary sales rep. For more information, see [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html).

#### To edit a sales rep forecast: {#procedure_N1049298}

1.  Go to _Forecast > Setup > Edit Sales Rep Forecast_.
    
2.  If you use NetSuite OneWorld, select the subsidiary for this forecast.
    
    If you select a parent subsidiary, this forecast represents the forecast for this subsidiary and all of its child subsidiaries. You can save only one forecast for a sales team per subsidiary.
    
3.  In the **Sales Rep** field, select the sales rep whose forecast you want to edit and save.
    
    The sales reps you see in this field depend on the permissions granted for your login role.
    
4.  Select the start date of the period you want to view the forecast for.
    
5.  Check the **Alt.Sales** box if this is an alternate sales amount (ASA) forecast.
    
    For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
    
    The sales rep's quota shows in the **Quota** field. You can establish quotas at _Forecast > Setup > Establish Quotas_.
    
    The **Calculated** and **Override** forecast amounts are shown. If you use the Advanced Forecasting feature, you can see forecast amounts in each forecast category.
    
6.  You can change the **Override** amounts on this forecast.
    
    **Override** amounts appear on forecast reports in addition to the calculated forecast.
    
7.  At any time, you can click **Restore Calculated** to change the **Override** forecast to match the calculated forecast amount.
    
8.  On the **Opportunities** and **Estimates** subtabs, you can do the following:
    
    -   change the forecast type for a transaction
        
        Note:
        
        This change affects which forecast types the transaction is included in. For more information, see [Opportunities in the Forecast and Pipeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047903.html).
        
    -   click the date to view the transaction
        
    -   change a transactions expected close date
        
    -   change a transactions probability of close
        
    -   change the projected amounts for any transaction
        
    -   adjust the status or probability of a transaction
        
    
    Note:
    
    An administrator can set probability in Forecast Editor preferences. Go to _Setup > Sales & Marketing Automation > Sales Preferences_. Click the Forecasts subtab.
    
9.  On the **Unbilled Orders** and **Actuals** subtabs, you can click the date to view a transaction.
    
10.  Click **Save**.
     

After you save a forecast, your reports show the updated forecast amounts.

Sales managers can edit a saved forecast. Go to _Forecast > Setup > Edit Sales Rep Forecast > List_. Click Edit next to the forecast.

Important:

NetSuite updates new opportunities automatically in the Sales Rep Forecast. However, it **doesn't** update them in the Sales Manager Forecast to ensure the forecast excludes tentative opportunities. To include a new opportunity in the Sales Manager forecast, the rep should update their forecast in edit mode and save the forecast. The figures are then updated on the manager forecast.

### Related Topics

-   [Saving Sales Manager Forecasts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1048767.html)
-   [Sales Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1045230.html)
-   [Advanced Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047034.html)
-   [Forecasting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046772.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

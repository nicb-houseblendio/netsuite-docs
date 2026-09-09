---
id: "section_N1038328"
type: "section"
title: "Overassignment and Adjustment Reps"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Team Selling > Overassignment and Adjustment Reps"
parent: "section_N1037318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038328.html"
anchors: ["procedure_N1038363", "procedure_N1038453"]
sha256: "d3b4443358bddaf8be6c13543e1f9eabc4cb3c1366debc0290727ce123132143"
---

If you let contribution percentages go over 100%, you need to create adjustment sales reps for each sales team. Adjustment sales reps ensure that sales reports show the right totals.

Overassignment lets you permit sales reps to count the full transaction amount when you calculate quota, commission, or sales forecast, even if other reps were involved.

Before you create an adjustment rep record, you need to create an adjustment rep sales role. For more info, see [Creating a Sales Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037578.html#bridgehead_N1037602).

#### To create an adjustment sales rep record: {#procedure_N1038363}

1.  Go to _Setup > Sales & Marketing Automation > Sales Preferences_.
    
2.  Check the **Allow Overassignment in Sales Team** box.
    
3.  At the bottom of the page, enter a name for the adjustment rep.
    
    You should name your adjustment reps to clearly identify which sales manager or supervisor they were created for. For example, **AdjustmentRep\_Linda Smith**.
    
4.  In the **Sales Role** field, select **Adjustment Rep**.
    
5.  Select the sales manager or supervisor whose sales totals you want this adjustment rep to correct.
    
6.  Click **Add**.
    

Now you can add this adjustment rep to a sales team.

#### To add an adjustment rep to a sales team: {#procedure_N1038453}

1.  Open the sales team group record at Setup > Sales > Sales Management > Sales Teams.
    
2.  On the **Members** subtab, select the adjustment rep for the team's supervisor or manager in the **Name** column.
    
3.  In the **Sales Role** column, select the adjustment rep for this team's manager or supervisor.
    
4.  In the **Contribution %** column next to the adjustment rep, enter the percentage amount that goes over the total 100% contributed by the other sales team members.
    
5.  Click **Add**.
    
6.  Click **Save**.
    

Adjustment reps show up on the sales team in sales reports and KPIs.

### Related Topics

-   [Overassignment and Adjustment Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038328.html)
-   [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html)
-   [Split Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1148007.html)
-   [Estimates and Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1047809.html)
-   [Opportunities and Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1048674.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

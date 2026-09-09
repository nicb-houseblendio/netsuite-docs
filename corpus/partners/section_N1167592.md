---
id: "section_N1167592"
type: "section"
title: "Overassignment and Adjustment Partners"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Managing Partners > Setting Up the Multi-Partner Management Feature > Overassignment and Adjustment Partners"
parent: "section_N1167284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167592.html"
anchors: ["procedure_N1167626", "procedure_N1167675"]
sha256: "4421adbd84b93b6fda423bd87bb083d2f684dc424e1f2b02e92c553bd13569dc"
---

With the Multi-Partner Management feature, you can decide how much of a sales transaction is used to calculate commission for each partner. The total contribution percentage assigned to partners on a single transaction or customer can't total more than 100%, unless you use an adjustment partner. With customers or transactions where the partner contribution exceeds 100%, add this adjustment partner and assign it the negative percentage amount that exceeds 100%.

For example, Wolfe Electronics assigns two partners to a sales order each with 100% contribution percentage. Wolfe then adds the adjustment partner and assigns it -100%. Each partner on the order receives commission based on the entire value of the order.

Before you create an adjustment partner, first create an adjustment partner role.

#### To create an adjustment partner role: {#procedure_N1167626}

1.  Go to _Setup > Sales > Setup Tasks > CRM Lists_.
    
2.  Click **New**.
    
3.  Click **Partner Category/Role**.
    
4.  In the **Partner Category/Role** field, enter **Adjustment**.
    
5.  Click **Save**.
    

#### To create an adjustment partner record: {#procedure_N1167675}

1.  Go to _Lists > Relationships > Partners > New_.
    
2.  In the **Company Name** or the **Name** field, enter **Adjustment Partner**.
    
3.  Under Primary Information, in the **Category** field, select **Adjustment**.
    
4.  Click **Save**.
    

Now, you can assign this partner to customers and sales transactions.

### Related Topics

-   [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html)
-   [Setting Up the Multi-Partner Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167284.html)
-   [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

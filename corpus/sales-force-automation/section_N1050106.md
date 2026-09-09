---
id: "section_N1050106"
type: "section"
title: "Calculating ASA"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Sales Forecasting > Alternate Sales Amounts > Calculating ASA"
parent: "section_N1049780"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050106.html"
anchors: []
sha256: "09a4ba478c42a7d2f60c26322440a09bada1b3f0056739f37b96cac2aaad0650"
---

There are two ways to calculate alternate sales amounts:

-   Set ASA with SuiteScript.
    
    With custom code, you can calculate ASA any way you want. For example, you can base ASA on the item's gross profit by subtracting the item's average cost from its sales price.
    
    Note:
    
    If you set alternate sales amount with scripting, the ASA for a transaction is still affected by discount or markup items.
    
    For more information, see [SuiteScript 2.x Scripting Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623184.html).
    
-   Calculate ASA as the first year revenue for item.
    
    The Default Alternate Sales Amount to First Year Revenue preference automatically calculates ASA as the first year's revenue for the line item. If you don't use the Revenue Recognition feature, NetSuite assumes that the sales amount entered is based on a 12 month term. In this case, the ASA is the same as the sales amount.
    
    If you use the Revenue Recognition feature, the first year revenue is based on specific fields. These fields are Rev. Rec. Start Date, Rev. Rec. End Date, and Rev. Term in Months.
    

For example, a line item is set to the following:

-   Sales Order Date: 1/1/2019
    
-   Rev. Rec. Start Date: 3/1/2019
    
-   Rev. Rec. End Date (either set manually or determined by the Rev. Term in Months field): 2/28/2021
    
-   Sales Amount: $2400
    

NetSuite calculates ASA as the months remaining in the first year divided by the term in months multiplied by the sales amount. For example, (10/24) \* $2400. The ASA is $1000. NetSuite uses the Rev. Rec. Start Date field to determine the first year revenue term, 3/1/2019 to 12/31/2019, or 10 months. For information about the Rev. Term in Months field, see [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html).

Note:

If you add a discount line item after a line item with a 0 ASA, NetSuite doesn't apply the discount to the ASA. If the alternate sales amount field of the discount line item is empty, NetSuite applies the discount to the transaction ASA. If you change the alternate sales amount on a discounted line item, you may need to reapply the discount to make sure the ASA is correct.

### Related Topics

-   [Setting Up ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049956.html)
-   [Basing Commission on ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050405.html)
-   [ASA Sales Forecasts and Quotas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

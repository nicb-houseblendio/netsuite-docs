---
id: "section_N1170168"
type: "section"
title: "Choosing the Basis of the Commission"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Partner Commissions & Royalties > Partner Commission Schedules > Choosing the Basis of the Commission"
parent: "section_N1170114"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1170168.html"
anchors: ["procedure_0513015441"]
sha256: "fdd0bef61641522e9254f03c3ce8ed3cffbc16728156fb37fc9bfe9ec9cd5c3f"
---

Commission schedules define the rules that determine how commissions are calculated. When you are creating a commission schedule, first choose the basis of the commission. Partner commission can be based on total sales, quantity sold, total profit, or on profitability.

To create a new partner commission schedule, go to _Lists > Commissions > Partner Schedules > New_. Enter a name for the schedule.

#### To choose the basis of the commission: {#procedure_0513015441}

1.  In the **Commission on** field, choose the basis on which commission will be awarded.
    
    Note:
    
    The fields on the commission schedule change as you make selections in other fields. For example, if you select **Quota (Sales Amount)** in the **Commission on** field, the **per** field appears and is set to **Period**.
    
    Select one of the following:
    
    1.  **Sales** - Awards commission based on sales amounts
        
    2.  **Alt.Sales Amount** - Awards commission on alternate sales amounts
        
        To base commission on alternate sales amounts, you must first enable the **Alternate Sales Amount (ASA)** feature. For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
        
    3.  **Quantity** - Commission is based on quantity of an item sold
        
    4.  **Inventory Profitability** - Awards a percentage based on the profitability of sales transactions
        
    5.  **Inventory Total Profit** - Awards commission based on the total profit of sales
        
    6.  **Custom Field** - displays the **Custom Field** field from which you select the custom transaction column field on which to base the commission. Custom transaction column fields must be defined by **Type**: **Currency**. These can be based on any standard or custom currency amount field. Commission is then calculated on each transaction line. For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html), [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html), and [Transaction Line Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3775025.html).
        
    
    Important:
    
    Commission calculations based on inventory item profit are based on the last purchase price on the item record, not on the purchase order price.
    
    Note:
    
    Your selection in this field determines your choices in the **Per** and **Categorized By** fields.
    
2.  In the **Per** field, select one of the following:
    
    1.  **Period** - Commission is awarded based on sales over a sales period.
        
    2.  **Transaction Total** - Commission is calculated based on the total transaction amount.
        
    3.  **Transaction Line Item** - Commission is awarded based on transaction line items.
        
3.  If your commission is calculated per period, select the length of your commission periods in the **Per** list.
    

### Related Topics

-   [Determining Commission Categorization and Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0513020459.html)
-   [Creating a Commission Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0513021302.html)
-   [Partner Commission Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1170924.html)
-   [Creating a Partner Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1171112.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

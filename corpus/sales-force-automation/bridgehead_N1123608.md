---
id: "bridgehead_N1123608"
type: "bridgehead"
title: "Choose the Basis of the Commission"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Creating an Employee Commission Schedule > Choose the Basis of the Commission"
parent: "section_N1123495"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1123608.html"
anchors: ["procedure_N1123626"]
sha256: "e40bf472dccd41cc67a89dca7403a53d158226ae09aa7531c3fb82eedcc0127b"
---

The first step in creating an employee commission schedule is to determine the basis for the commission.

#### To set commission basis: {#procedure_N1123626}

1.  In the **Commission on** field, choose the basis on which NetSuite awards commission.
    
    Your selection determines your choices in the **per** and **Categorized by** fields.
    
    Note:
    
    The fields on the commission schedule change as you make selections in other fields. For example, if you select **Sales** in the **Commission on** field and **Quota** in the **Quota Type** field, the **per** field appears and defaults to **Period**.
    
    Select one of the following:
    
    -   **Sales** - Awards commission based on sales amounts
        
    -   **Alt. Sales Amount** - Awards commission on alternate sales amounts
        
        To base commission on alternate sales amounts, you must first enable the Alternate Sales Amount (ASA) feature. For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
        
    -   **YTD Quota** - NetSuite bases commission on the percentage of the quota fulfilled for the year to date
        
    -   **Quota (Sales Amount)** - Awards commission based on percentage of quota fulfilled in a period
        
    -   **YTD Quota (Alt. Sales Amount)** - NetSuite bases commission on the percentage of the quotas fulfilled by ASA for the year to date
        
    -   **Quota (Alt. Sales Amount)** - Awards commission based on percentage of alternate sales amount ASA quota fulfilled in a period
        
        For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
        
    -   **Quantity** - NetSuite bases commission on quantity of an item sold
        
    -   **Inventory Profitability** - Awards a percentage based on the profitability of sales transactions
        
        Important:
        
        NetSuite bases commission calculations for inventory item profit on the last purchase price on the item record, not on the purchase order price.
        
    -   **Inventory Total Profit** - Awards commission based on the total profit of sales
        
    -   **Custom Field** - Displays the **Custom Field** and **Quota Type** fields
        
        To see custom fields, an administrator must go to Setup > Company > Enable Features (Administrator) > Employee subtab. Check the **Commission on Custom Fields** box, and then click **Save**.
        
        In the **Custom Field** list, select the custom transaction column field on which to base the commission. Custom transaction column fields must be defined by **Type**: **Currency** and can be based on any standard or custom currency amount field. NetSuite calculates commission on each transaction line. For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html), [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html), and [Transaction Line Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3775025.html).
        
        In the **Quota Type** field, choose from the following options:
        
        -   **No Quota** - Awards commission that is not based on quota
            
        -   **Quota** - Awards commission based on the percentage of quota fulfilled in a period
            
        -   **YTD Quota** - Awards commission based on the percentage of the quota fulfilled for the year to date
            
2.  In the **per** field, select one of the following:
    
    -   **Period** - Awards commission based on sales over a sales period
        
    -   **Transaction Total** - Calculates commission based on the total transaction amount
        
    -   **Transaction Line Item** - Awards commission based on transaction line items
        
    
    Important:
    
    Commission calculations are rounded when they are calculated, and then totaled, which can result in differences between expected and actual totals. If calculations are based upon a larger number of small transactions, then that difference can be larger. To minimize the impact of rounding, select **Period** or **Transaction Total** instead of **Transaction Line Item**.
    
    Note:
    
    The choices available in this field depend on the type of commission you are creating. For example, commission schedules based on quota require you to select **Period** in the **per** field.
    
3.  If NetSuite calculates commission per period, select the length of your commission periods in the **per** list.
    
4.  Check the **Manager Schedule** box to calculate commission based on the sales of subordinates as well as sales made directly by the manager.
    
    Manager schedules award commission only to sales people who supervise other sales reps.
    

Note:

After a commission schedule has authorizations associated with it, you cannot change the selections for the **per** or **Categorized by** fields.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html)
-   [Determine Commission Categorization and Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1123880.html)
-   [Set Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124420.html)
-   [Set Commission Schedule Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124587.html)
-   [Create a Commission Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124704.html)
-   [Save the Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N1124778.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

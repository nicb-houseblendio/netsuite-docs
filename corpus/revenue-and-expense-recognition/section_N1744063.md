---
id: "section_N1744063"
type: "section"
title: "Two-Step Revenue Allocation"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > Two-Step Revenue Allocation"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1744063.html"
anchors: ["bridgehead_N1744108", "bridgehead_N1744184"]
sha256: "19396f499be6ff520a94897969b2e8c8866b0883e38b90b156482eb3eccee490"
---

EITF 08-01 Revenue Recognition supports recognizing revenue for multiple element sales where both the EITF 08-01(ESP) and SOP 97-2 (VSOE) accounting rules apply. By identifying the allocation type for each item on a sales order, you can then allocate revenue according to the appropriate recognition rule.

The allocation types are Excluded, Normal, and Software. You assign an allocation type on the item record, but you can change the type when creating a sales order. For more information about allocation types, see [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html).

To use this feature, you must enable the Two-Step Revenue Allocation preference. For more information, see [Setting EITF 08-01 Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html#bridgehead_N1746683).

## Two-Step Calculation Process {#bridgehead_N1744108}

The two-step allocation calculation occurs when a sales order includes items with an allocation type of Normal and Software and the Two-Step Revenue Allocation preference is enabled.

Allocation price calculates as follows:

-   **Step 1:** NetSuite allocates revenue for all items on a sales order using the ESP value and EITF 08-01 rules. This calculation is performed for items of type Normal and Software. The results are displayed in the Allocation Amount field in the VSOE column popup. When the VSOE price is available for an item, the VSOE price is used for the ESP value.
    
-   **Step 2:** For items with an allocation type of Software, revenue allocation is recalculated using the SOP-97-2 rule and overwrites the value in the Allocation Amount field.
    
    -   If the VSOE price is available for all software items, no recalculation is needed.
        
    -   If the VSOE price isn't available for some of the software items, NetSuite uses the residual method to reallocate according to SOP 97-2 rules.
        
        Note:
        
        Open the ESP Allocation popup for a line item to quickly identify whether an item has a VSOE price. If the **Estimate** box is checked, the VSOE price isn't available for the item. This setting populates from the "IsVSOE" value for the item on the Multiple Allocation Price List.
        
    -   All software items on a sales order are placed in one sub-group.
        

## Two-Step Revenue Allocation Example {#bridgehead_N1744184}

In this example, a multiple element sales order for $6,500 that includes items that follow different revenue allocation rules:

-   **Excluded** - Registration Fee
    
-   **Normal** - Hardware, Hardware Support - EITF 08-01 rules apply
    
-   **Software** - Software, Software Support - SOP 97-2 rules apply
    

The table below shows the revenue allocation calculated for each step:

| Item | Allocation Type | Sales Price | VSOE | ESP | Is VSOE | Esti-mate | % | Step 1 Allocation | Deliv'd | Step 2 Allocation |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| One time Registration Fee (non refundable) | Excluded | 2,000.00 | \- | \- | Yes | No | \- | 2,000.00 | Yes | 2,000.00 |
| Hardware | Normal | 1,000.00 | 1,500.00 | 1,500.00 | Yes | No | 27% | 1,227.27 | Yes | 1,227.27 |
| Hardware Maintenance | Normal | 1,500.00 | 1,500.00 | 1,500.00 | Yes | No | 27% | 1,227.27 | Yes | 1,227.27 |
| Software | Software | 1,000.00 | \- | 1,000.00 | No | Yes | 18% | 818.18 | Yes | 545.45 |
| Software Support | Software | 1,000.00 | 1,500.00 | 1,500.00 | Yes | No | 27% | 1,227.27 | No | 1,500.00 |
| Total | \- | 6,500.00 | \- | 5,500.00 | \- | \- | \- | 6,500.00 | Yes | 6,500.00 |

For Registration Fee, the sales price for the item is used for revenue recognition because this type of item is excluded from the revenue reallocation process. Based on the Multiple Allocation Price List, the VSOE (ESP) total amount for the remaining items is $5,500. The ratio of each of these items to the VSOE (ESP) total is 27%, 27%, 18%, and 27%, respectively. NetSuite uses these percentages to calculate the revenue allocation amounts in the first step of the allocation. Then, the second calculation occurs for the software items. The revenue allocation amounts recalculate as $545.45 and $1500.00. These amounts are calculated using the residual method of revenue recognition. See [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html).

The Allocation Price for each item on the sales order now displays the amounts shown in Step 2 Allocation column in the table: $2,000.00, $1,227.27, $1,227.27, 545.45, and $1,500.00.

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [EITF 08-01 Allocation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2323037"
type: "section"
title: "Marking Work Orders Closed"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items > Marking Work Orders Built > Marking Work Orders Closed"
parent: "section_N2322811"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323037.html"
anchors: ["procedure_N2323105"]
sha256: "1a01bf068b92318cc2e0e03e163658f02c84924fe978d63e42478e4e4f376569"
---

For some work orders you may want to show the items as being assembled without completing all the steps. In such a case you can skip the steps and mark the order as closed.

When you mark an order as closed, the required items are marked closed and added to inventory.

Note:

Associated variances are created when you mark an order built. For information about variances, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

#### To mark a work order closed: {#procedure_N2323105}

1.  Go to _Transactions > Manufacturing > Close Work Orders_.
    
2.  In Primary Options and Criteria, complete the following:
    
    1.  Select the **Posting Period** you want to post this transaction to. You cannot post to a closed period.
        
    2.  Enter a transaction **Date**.
        
    3.  Select a transaction **Location**.
        
    4.  Select an assembly **Item** to filter the list and show only work orders for the item.
        
    5.  Select a **Customer** to filter the list for transactions associated with the customer. Select All to show all transactions.
        
    6.  Check the **Include In-Process Work Orders** box to include work orders with In Process and Built status.
        
    7.  In the **Under-Produced Variance Tolerance (%)** field, enter a percentage to close only orders that produced less than planned. This helps you determine whether to keep some orders open because they haven't produced enough finished product.
        
        Order variance calculation: (quantity ordered - quantity built/quantity ordered) = variance percentage
        
        Entering a percentage in this field filters the list of orders to close to show only orders with a variance lower than the percentage entered.
        
    8.  In the **Production Variance Tolerance (%)** field, enter a percentage to filter orders with a specific value variance.
        
        Order variance calculation: absolute value (remaining WIP value / WIP of assembly) = variance percentage
        
        Entering a percentage in this field filters the list of orders to close to show only orders with a variance lower than the percentage entered.
        
3.  In Date Range Criteria, choose from the following:
    
    -   To filter by an order date range, enter a beginning date in the **Order Date From** field. Enter an end date in the **Order Date To** field.
        
    -   To filter by a production start date range, enter a beginning date in the **Production Start Date From** field. Enter an end date in the **Production Start Date To** field.
        
    -   To filter by a production end date range, enter a beginning date in the **Production End Date From** field. Enter an end date in the **Production End Date To** field.
        
4.  In Orders, complete the following:
    
    1.  Check the **Close** box next to each order to be closed.
        
    2.  Verify the quantities and variances displayed for each order.
        
    3.  Click **Submit**.
        

### Related Topics

-   [Marking Work Orders Built](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2322811.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

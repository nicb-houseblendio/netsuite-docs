---
id: "section_N2340152"
type: "section"
title: "Entering Work Order Closes"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Using WIP on Work Orders > Entering Work Order Closes"
parent: "section_N2337938"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html"
anchors: ["procedure_N2340191"]
sha256: "ba0123e3d043a8beb62d396dae94835def38c612d1ccf971a590a95b9fb41a45"
---

Use Manufacturing WIP to enter a work order close to finalize the accounting for that order. The work order close reconciles the accounting by reviewing all issues and completions associated with that work order.

#### To bulk enter work order closes: {#procedure_N2340191}

1.  Go to _Transactions > Manufacturing > Close Work Orders_.
    
2.  Select the **Posting Period**.
    
3.  Select the transaction **Date**.
    
4.  Select a **Location**.
    
5.  Optionally, select the following to filter the list of work orders:
    
    -   **Item**
        
    -   **Customer**
        
6.  To include work orders with In Process or Built status, check the **Include In Process Work Orders** box.
    
7.  This list includes work orders in Released and Planned status.
    
    To show only work orders in Built and In Progress status:
    
    1.  Go to _Transactions > Manufacturing > Close Work Orders_
        
    2.  In the **Close Work Orders** page, click **Customize**.
        
    3.  In the **Customize Sublist** page, click the **Additional Filters** subtab.
        
    4.  Beside the **Status** field, check the **Include** checkbox.
        
    5.  Click **Save.**
        
8.  In the **Under-Produced Variance Tolerance (%)** field, enter a percentage to close only orders that produced less than planned.
    
    This helps determine whether some orders should not be closed because enough finished products haven't been produced.
    
    **Order Variance Calculation**: quantity ordered - quantity built/quantity ordered = variance percentage
    
    A percentage in this field filters the list to show only orders that have a variance lower than the percentage entered.
    
    For example, if order quantity is 10 and built quantity is 5, then the variance percentage is (10-5)/10 = 50%.
    
    If you enter a tolerance of 60%, this order shows in the list for closing.
    
    If you enter a tolerance of 10%, this order doesn't show in the list.
    
9.  In the **Production Variance Tolerance (%)** field, enter a percentage to filter out orders that have a specific value variance.
    
    The order variance calculation is: absolute value (remaining WIP value / WIP of assembly) = variance percentage
    
    A percentage in this field filters the list to show only orders that have a variance lower than the percentage entered.
    
    For example, the WIP account value is $10, and the cost of building the assembly is $20. Therefore, the variance percentage is (10/20) = 50%.
    
    If you enter 10% in this field, this order doesn't show in the list for closing.
    
    If you enter 60% in this field, this order shows in the list.
    
10.  You can filter the list order by selecting a range of dates.
     
     If you use demand planning, optionally filter the list by selecting a production start date and end date.
     
     1.  To filter by an order date range, enter a beginning date in the **Order Date From** field. Enter an end date in the **Order Date To** field.
         
     2.  To filter by a production start date range, enter a beginning date in the **Production Start Date From** field. Enter an end date in the **Production Start Date To** field.
         
     3.  To filter by a production end date range, enter a beginning date in the **Production End Date From** field. Enter an end date in the **Production End Date To** field.
         
11.  Next to all orders you want to close, check the **Close** box.
     
12.  Click **Submit**.
     

Important:

Cost discrepancies may occur because of currency decimal precision and rounding off values. To lessen the probability of substantial variances, reduce the decimal precision used for the cost of components to 2.

### Related Topics

-   [Entering a Close for an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607541480.html)
-   [Entering Work Order Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html)
-   [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

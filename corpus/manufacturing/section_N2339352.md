---
id: "section_N2339352"
type: "section"
title: "Entering Work Order Completions"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Using WIP on Work Orders > Entering Work Order Completions"
parent: "section_N2337938"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html"
anchors: ["procedure_N2339406"]
sha256: "8767b5ed492fc7cb967594577af1781ae021dc6b577474359f52fb8ef26e44aa"
---

To use the Manufacturing WIP, enter a completion transaction to log the number of assemblies you completed and stocked for a work order. This transaction indicates the number of finished goods produced.

Entering a completion doesn't record the consumption of materials. It only records the work done on the assembly process and journals the value of the assembly out of the assigned WIP account.

You can enter a work order completion with backflush to issue components and complete the assembly at one time.

Note:

A Work order completion with Backflush is created for backflush orders. As of NetSuite 2024.1 work order completions and work order issues are created separately. Both transaction records are updated in the Manufacturing Mobile production record.

#### To enter a work order completion: {#procedure_N2339406}

1.  Go to _Transactions > Manufacturing > Enter Completions_.
    
2.  Select an assembly **Item** to filter the list and show only work orders for the item.
    
3.  Select the **Customer** or vendor providing this item.
    
    Alternatively, select an employee to associate with this transaction.
    
4.  Select the **Posting Period** to post this transaction to.
    
5.  Accept today's **Date** as the transaction date, or select another date.
    
6.  Select a **Location** to use to build orders, issue components, or enter completions.
    
    This location appears in the location field in the header of all work order completions created.
    
7.  To enter completions with backflush, check the **Backflush** box.
    
    Backflush records component consumption at the same time. Component consumption is based on the proportion designated on the original work order and the build quantity.
    
    Clear this box to enter the completion without backflush and not record consumption.
    
8.  Enter a **Sales Order Number** or scan a transaction bar code.
    
9.  Check the box in the **Complete** column for each order to be completed.
    
10.  Verify or enter the quantity completed for each order.
     
     The field shows the quantity remaining on the order by default.
     
11.  Click **Submit**.
     
     After a completion is entered against a work order, that quantity of assemblies is recorded as being built and stocked in inventory.
     

Note:

The work order completion **Projected Value** field displays the cost of the assembly. It doesn't display individual components (unless you use backflush). A Work Order Close for the work order shows the difference between the cost of the assembly and the components.

### Related Topics

-   [Entering Work Order Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html)
-   [Entering Work Order Closes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2404305"
type: "section"
title: "Editing a Purchase Order"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Editing a Purchase Order"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html"
anchors: ["procedure_N2404324"]
sha256: "5e77a74c2cf24035703854d4dbece20c562e4a12adb2db484921105b6ac2712f"
---

If you need to change a saved, approved, or unapproved purchase order, you first find the transaction, and then make the changes.

Note:

If the PO has already been approved, you must recall it before you can edit it.

#### To edit a purchase order: {#procedure_N2404324}

1.  Go to _Transactions > Purchases/Vendors > Enter Purchase Orders > List_.
    
2.  Click **Edit** next to the purchase order you want to change.
    
3.  On the purchase order, make the necessary changes.
    
    If the vendor has received the earlier version of the purchase order, state that this is a revised order in the **Vendor Message** field.
    
4.  To make changes to line items:
    
    1.  Click the **Items** subtab.
        
    2.  Click the line item you want to change.
        
    3.  Enter the changes in the appropriate fields.
        
    4.  Clear the **Closed** box for a line item if you know the item won't be received.
        
    5.  When you finish changing information about an item, click **Done**.
        
5.  Continue to change additional items as required.
    
    Note:
    
    Take note of the following:
    
    -   If you change the quantity on all items on the purchase order to zero, the purchase order moves to the **Closed** status.
        
    -   If you add a new item to the purchase order, the **Department** field value is sourced from the employee record set on the purchase order. If the employee doesn't have a set department or if there is no employee set on the purchase order, note the following. The **Department** field value is sourced from the item record. If neither the employee nor the item record have a set department, the **Department** field remains blank.
        
    
6.  Click the **Communication** subtab.
    
7.  Check the appropriate box to send a copy of the revised purchase order to the vendor by printing, emailing or faxing a copy.
    
8.  Click **Save**.
    
    If the purchase order is closed, clearing the **Closed** status for one or more items opens the purchase order
    

Important:

Avoid non-backward compatible changes as they can break integrations. For example:

-   removing public lists
    
-   changing a publicly exposed field identifier
    
-   changing a type of publicly exposed field
    
-   changing a behavior
    

### Additional Information

-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)

### Related Topics

-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
-   [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html)
-   [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html)
-   [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html)
-   [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html)
-   [Viewing the Status of a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html)
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)
-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

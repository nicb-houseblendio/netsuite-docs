---
id: "section_N1256787"
type: "section"
title: "Advanced Billing and Advanced Shipping"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing and Advanced Shipping"
parent: "chapter_N1232486"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html"
anchors: []
sha256: "6b16a19dc16faf17cc6b37e4230026d2e7e01f93608f150a6fa3dc21f8400e44"
---

When you use the Advanced Billing feature and the Advanced Shipping feature together, order processing is based on whether each item on an order is able to be fulfilled or received.

Items are able to be fulfilled or received based on the status set on the item record. Some item types have a permanent status that marks them fulfilled or received. Other item types permit you to set the status for always fulfilling and receiving them or never doing so. You can set item statuses as follows:

-   **Always Fulfillable/Receivable**
    
    -   Inventory
        
    -   Assembly/Bill of Materials
        
-   **Never Fulfillable/Receivable**
    
    -   Group
        
    -   Description
        
    -   Discount
        
    -   Markup
        
-   **Allows Changes to Fulfillable/Receivable Status**
    
    -   Kit/Package
        
    -   Non-Inventory
        
    -   Download
        
    -   Gift Certificate
        
    -   Other Charge for Sale or Resale
        
    -   Service Item for Sale or Resale
        

To set an item's fulfillable/receivable status, go to _List > Accounting > Items_, and click **Edit** next to a Gift Certificate, Other Charge or Service item record. On the **Preferences** subtab, check or clear the **Can be Fulfilled/Received** box, and click **Save**.

After setting the fulfillable/receivable status for items, NetSuite processes the appropriate items based on the following conditions:

-   If the order includes unbilled items
    
-   If the order includes associated billing schedules
    
-   If the order includes fulfillable items
    
-   Setting for the **Invoice in Advance of Fulfillment** preference
    

### Related Topics

-   [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html)
-   [Billing Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257068.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

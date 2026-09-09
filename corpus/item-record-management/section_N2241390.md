---
id: "section_N2241390"
type: "section"
title: "Selling a Drop Ship Item"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Drop Ship Items > Selling a Drop Ship Item"
parent: "section_N2239232"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2241390.html"
anchors: ["procedure_N2241413", "procedure_N2241499", "procedure_N2241694", "procedure_N2241786"]
sha256: "6194338d1bb6f4d3063853535ca72945a8424422c87281f6e8a57c9d81f74fc7"
---

A drop ship item is sold using a sales order. When you approve the sales order, NetSuite generates a purchase order for the preferred vendor that shows the customer's shipping address. Drop ship items ship directly from your vendor to your customer. You can drop ship inventory items and non-inventory for resale items.

Sales orders are created automatically when a customer orders drop ship items from your web store. You can also manually create sales orders. You can set items to drop ship automatically or manually.

#### To automatically drop ship an item: {#procedure_N2241413}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the item you want to automatically drop ship.
    
3.  On the item record, check the **Drop Ship Item** box.
    
    After the item is entered on a sales order and approved, NetSuite generates a purchase order.
    

#### To manually drop ship an item on a new sales order: {#procedure_N2241499}

1.  Go to _Transactions > Sales > Enter Sales Orders_.
    
2.  In the **Custom Form** field, choose one of the following:
    
    -   **Enhanced Sales Order - Progress Billing**
        
    -   **Standard Sales Order**
        
    -   **Standard Sales Order - Cash Sale** to record check or credit card information before shipping
        
    -   **Standard Sales Order - Invoice** to arrange terms for payment after shipping
        
    -   **Standard Sales Order - Progress Billing** to invoice your customers for orders in stages
        
3.  Select a **Customer** or job.
    
4.  Verify or enter the **Date**.
    
5.  Select a **Status** from the list.
    
    Select **Pending Fulfillment** to skip the sales order approval process to create the purchase order when the order is submitted.
    
6.  Enter any additional information necessary.
    
7.  On the **Shipping** subtab, in the **Ship To** field, verify the customer's shipping address.
    
8.  On the **Items** subtab, select an item. If the item's record is marked for drop shipment and has a preferred vendor, the **Create PO** field defaults to **Drop Ship**.
    
    If the item is not marked for drop shipment, the **Create PO** field is dimmed and uneditable.
    
9.  Enter the item quantity.
    
10.  Accept or change the default information.
     
11.  Complete any custom fields.
     
12.  Click **Add**.
     
13.  Repeat steps 8 - 12 for each additional item.
     
14.  Click **Save**.
     

When the sales order is approved, a purchase order is generated for drop ship items.

To generate your drop ship purchase order based on a custom form, you must link your sales order form to your custom purchase order form. For more information, see [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html).

You can drop ship items on an existing sales order if the item has not yet been fulfilled. You can set specific items to drop ship whether the sales order has or has not been approved.

#### To manually drop ship an item on an unfulfilled purchase order: {#procedure_N2241694}

1.  Go to _Transactions > Sales > Enter Sales Orders > List_.
    
2.  Click **Edit** next to the order that contains the unfulfilled item you want to drop ship.
    
3.  On the **Shipping** subtab, verify that the sales order shows the correct customer shipping address.
    
4.  Click the item you want to drop ship.
    
5.  Click the **Items** subtab.
    
6.  In the **Create PO** column next to the item, select **Drop Ship**.
    
7.  Click **Done**.
    
8.  Repeat steps 4 - 6 for unfulfilled items you want to drop ship.
    
9.  Click **Save**.
    

If a sales order is approved, click the **Drop Ship** button to drop ship all inventory items and non-inventory for resale items on the order.

#### To drop ship items grouped by vendor on an approved order: {#procedure_N2241786}

1.  Go to _Transactions > Sales > Enter Sales Orders > List_.
    
2.  Click **View** next to the sales order.
    
3.  On the **Shipping** subtab, verify that the sales order shows the correct customer shipping address.
    
4.  Click the **Items** subtab.
    
5.  In the **Create PO** column next to the item, click **Drop Ship**.
    
    A purchase order is created for any unfulfilled inventory items and non-inventory for resale items.
    
    A purchase order is created for one vendor at a time. To drop ship items on this order from a different vendor, after step 7 click **Drop Ship**.
    
6.  Verify that the purchase order is correct.
    
7.  Click **Save**.
    
    The sales order opens and the **Create PO** column displays the number of the purchase orders created.
    
8.  If there are more items on the sales order that you want to drop ship, repeat steps 5 - 7.
    

### Related Topics

-   [Drop Shipping Kit Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1521820144.html)
-   [Setting Up Drop Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239482.html)
-   [Marking an Item for Drop Shipment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239986.html)
-   [Viewing a Drop Ship Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2241194.html)
-   [Fulfill and Receive Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242062.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

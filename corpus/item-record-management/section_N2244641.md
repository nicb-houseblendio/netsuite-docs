---
id: "section_N2244641"
type: "section"
title: "Identifying Special Orders"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Special Order Items > Identifying Special Orders"
parent: "section_N2242662"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244641.html"
anchors: ["bridgehead_N2244673", "procedure_N2244685", "bridgehead_N2244788", "procedure_N2244800", "bridgehead_N2244874"]
sha256: "5fb01b7dbb75a56fea0eb917f9c78fd522fbc6647373c782a01fa4e64f0a6cf4"
---

You can special order any inventory items and non-inventory for resale items. Items can be tagged as special orders in two ways:

-   Marking the item when you create the sales order
    
-   Tagging the item record
    

Note:

You must identify a preferred vendor and a purchase price on an item record for that item to be selected as a special order.

## On Item Records {#bridgehead_N2244673}

You can set an item to automatically default as a special order by tagging the item record. Then, when the item is selected on a transaction, the field in the Create PO column autofills as Special Order.

#### To set an item to default to special order: {#procedure_N2244685}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the item.
    
    You can set up inventory item and non-inventory for resale item records to default as special orders.
    
3.  Click the **Purchasing/Inventory** subtab of the item record.
    
4.  Check the **Special Order** box.
    
5.  Identify a **Preferred Vendor**.
    
    If you use the Multiple Vendors feature, this field is on the **Vendors** subtab.
    
6.  Enter a **Purchase Price**.
    
7.  Click **Save**.
    

Note:

Drop Shipments are a function of the Drop Shipments and Special Orders feature. After you enable the feature, an item can be either a drop ship or special order, but not both.

## On Sales Transactions {#bridgehead_N2244788}

Items can be tagged as special orders when you create a sales transaction by selecting Special Order in the Create PO column list. Then, when you save or approve the order, NetSuite creates a purchase order that is linked to the sale.

#### To mark an item as a special order on transactions: {#procedure_N2244800}

1.  Click the **Transactions** subtab.
    
2.  Click the type of sales transaction you want to create.
    
    You can enter special order items on sales orders, invoices, and cash sales.
    
3.  Enter information in the transaction fields as needed.
    
4.  In the **item** field, select an inventory or non-inventory for resale item.
    
5.  In the **Create PO** list, select **Special Order**.
    
6.  Enter additional information as needed for this line item.
    
7.  Click **Add**.
    
8.  Click **Save**.
    

When you save a transaction that contains a special order item, NetSuite automatically creates a purchase order that is linked to the sales transaction.

## Special Order Kit Members {#bridgehead_N2244874}

When you initially enter a sales order that includes a kit with a special order member item, note the following. NetSuite automatically generates a special order purchase order for the member item.

If you change an existing order to add a kit with a special order member item, NetSuite doesn't automatically generate a purchase order. If you change an existing order to add a non-kit special order item, you can generate a purchase order for the drop ship item.

First, edit the sales order to add the special order item, and then save. Next, edit the sales order again to click Special Order next to the item you added. Then, save.

### Related Topics

-   [Enabling Drop Shipments and Special Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244482.html)
-   [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

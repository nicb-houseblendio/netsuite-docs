---
id: "section_N2281951"
type: "section"
title: "Fulfilling Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Sales and Fulfillment > Fulfilling Inventory"
parent: "section_N2281204"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281951.html"
anchors: ["bridgehead_N2282020", "bridgehead_N2282072", "bridgehead_N2282116", "bridgehead_N2282190", "bridgehead_N2282227"]
sha256: "dacb40f2e52851d6d391f9e02da35404e751df258d1a60b2061f67930bc67c01"
---

An item fulfillment is a transaction that specifies that you shipped some or all items on an order to the customer.

How each fulfillment is processed depends on whether you use the Advanced Shipping feature.

-   If you do not use the Advanced Shipping feature, the fulfillment and invoicing processes are combined. When you fulfill an item, you create a customer invoice for it simultaneously, based on the fulfillment.
    
-   If you do use the Advanced Shipping feature, you have separate processes to fill orders and bill customers. Then, you can track your shipments separately from creating invoices.
    

Note:

Order fulfillments should always be entered against sales orders to track the status of items and orders.

To enable the Advanced Shipping feature, read [Items and Inventory Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N235482.html).

## Fulfilling Items Without Advanced Shipping {#bridgehead_N2282020}

After you ship items to the customer, process the order by fulfilling the items and creating an invoice for them.

When an order is fulfilled without Advanced Shipping:

-   An Item Fulfillment record is created.
    
-   Inventory records are updated with new quantities.
    
-   The total value of the inventory fulfilled is deducted from your Inventory Asset account.
    
-   A customer Invoice is created.
    

If you do not use the Advanced Shipping feature, you can bill a customer for only the items you ship. This is because sales orders are fulfilled and billed in the same transaction. You can partially fulfill a sales order and any items fulfilled are also be billed.

## Fulfilling Items Using Advanced Shipping {#bridgehead_N2282072}

Advanced Shipping gives your shipping and accounting departments separate processes for fulfilling and billing sales orders. Your shipping department fulfills part or all of a sales order when it is ready to ship. Then, your accounting department creates an invoice or cash sale for the shipped items and rendered services.

With advanced shipping, you can track partial shipments and invoice customers for partial or entire orders.

When an order is fulfilled with Advanced Shipping:

-   An Item Fulfillment record is created.
    
-   Inventory records are updated with new quantities.
    
-   The total value of the inventory fulfilled is deducted from your Inventory Asset account.
    

## Using Advanced Billing with Advanced Shipping {#bridgehead_N2282116}

When you use Advanced Billing and Advanced Shipping features, processing orders is based on whether items on orders can be fulfilled or received.

Some item types have a permanent status that enables or disables them to be fulfilled or received. Other item types allow you to set the status for always fulfilling and receiving them, or never doing so. Item statuses can be set as follows:

-   **Always Fulfillable/Receivable** - Assembly, Kit, Inventory, and Non-inventory items.
    
-   **Never Fulfillable/Receivable** - Group, Description, Discount, Markup, Payment, and Download items.
    
-   **Allows Changes to Fulfillable/Receivable Status** - Gift Certificate, Other Charge, and Service items.
    

## Fulfillment Reporting {#bridgehead_N2282190}

To access information about items and orders that need to be fulfilled, you can go to the **Reports** tab and view these reports:

-   **Items Pending Fulfillment** - This report shows all open transaction lines for items on sales orders, grouped by item. For each item, the report shows the quantity ordered, quantity fulfilled and quantity committed.
    
-   **Sales Orders Pending Fulfillment** - This report shows all open transaction lines for items committed and ready to be fulfilled on sales orders, grouped by sales order.
    

## Closing Lines on Fulfillments {#bridgehead_N2282227}

If an order includes items that are not yet fulfilled and you do not plan to fulfill them, you should close those transaction lines. For more information, read [Closing Line Items That Will Not Be Fulfilled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227091.html).

### Related Topics

-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Purchasing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html#bridgehead_N2251155)
-   [Warehouse Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317586.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

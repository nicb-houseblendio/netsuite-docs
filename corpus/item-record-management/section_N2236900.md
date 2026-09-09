---
id: "section_N2236900"
type: "section"
title: "Selling and Fulfilling Lot Numbered Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Lot Numbered Items > Selling and Fulfilling Lot Numbered Items"
parent: "section_N2235684"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236900.html"
anchors: ["procedure_N2238306", "bridgehead_N2238420", "bridgehead_N2238283"]
sha256: "e74757feb701bef3546b032ed1133cb1deb641cebe2591002e6db9b9b47fe2a1"
---

On sales transactions in the Item field, you can select a lot item from the inventory list by entering the item name or lot number. When a lot number is entered, the item name autofills in the Item field.

Lot items that are added to sales transactions must include a lot number for each item when the transaction posts.

-   **Non-posting** - If a lot item is selected on a non-posting sales transaction, you can enter a lot number when the order is fulfilled.
    
    Non-posting sales transactions include estimates and sales orders.
    
    Note:
    
    If a lot number is entered on a non-posting sales transaction, that lot number is on hold and not available for sale on new transactions.
    
-   **Posting** - If a lot item is selected on a posting sales transaction, you must enter a lot number on that transaction.
    
    Posting sales transactions include the following:
    
    -   Invoices
        
    -   Cash Sales
        
    -   Sales Order Fulfillments
        
        In the Serial/Lot Number field on a posting sales transaction, enter or select the lot number of the item you are selling.
        

When you view a saved sales transaction that includes a lot numbered item, note the following. You can click the lot number to view or edit values in the Memo field or a custom field on the inventory number record. For more information, see [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html).

For information about receiving lot numbered inventory using Multiple Units of Measure, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

For information about best practices for committing numbered inventory, see [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html).

#### To fulfill a sales order that contains a lot item: {#procedure_N2238306}

1.  Go to _Transactions > Sales > Fulfill Sales Orders_.
    
2.  In the **Customer** field, select a customer or **All**.
    
3.  Click **Fulfill** in the **Process** column next to the sales order you want to fulfill.
    
4.  On the Item Fulfillment page, click the line that shows the lot item.
    
5.  In the **Serial/Lot Number** field, enter the lot number of the item.
    
    Lot numbers must be entered in this format: **LOT#(Quantity)**
    
    For example, to enter a quantity of 100 items as Lot number ABC1234, enter **ABC1234(100)** in the **Lot Numbers** column.
    
    Note:
    
    You can enter a maximum of 4000 characters in this field.
    
    1.  To choose multiple lot numbered items on transactions, click the **Select Multiple** link next to the **Serial/Lot Numbers** field.
        
    2.  In the popup list click items in the left pane to add it in the list right pane.
        
    3.  Click **Done**.
        
        All items in the right pane of the popup window are added to the transaction. You can also enter a quantity to add more than one item from that lot. If you do not enter a quantity for a lot number, NetSuite assumes a quantity of one.
        
6.  Click **Save**.
    
    After an order is fulfilled and billed, the lot number on the cash sale or invoice appears for information purposes only. Changes made to the lot number no longer affect inventory.
    

## Bulk Fulfillment {#bridgehead_N2238420}

To bulk fulfill a batch of sales orders, sales orders with lot items must include the corresponding lot numbers.

If a lot item on a sales order doesn't have a lot number entered, you can't bulk fulfill. You must fulfill the sales order individually to enter the lot number.

## Fractional Quantities {#bridgehead_N2238283}

You can stock, buy, and sell lot-numbered items in fractional quantities. This can be useful if you track items that are measured by volume or weight.

For example, an industrial chemical manufacturer produces 100 liters of a chemical compound and identifies it as lot #1010 on its item record. A 0.5 liter quantity of the compound is sold to a customer. The item fulfillment shows 0.5 quantity of lot item #1010 sent to the customer and the item record shows 95.5 liters remaining of lot #1010.

Note:

Lot-numbered items can't be sold in fractional quantities through your web store. They can be sold only in integer quantities.

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Enabling Lot Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163360479619.html)
-   [Creating Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236287.html)
-   [Receiving a Purchase Order With a Lot Numbered Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236584.html)
-   [Building a Lot Numbered Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238544.html)
-   [Viewing Lot Numbered Inventory Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163360798322.html)
-   [Selecting Lot Numbers on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2236107.html)
-   [Lot Auto Numbering SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162780241331.html)
-   [Allergen Statements SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1562672738.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

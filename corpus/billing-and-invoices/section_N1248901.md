---
id: "section_N1248901"
type: "section"
title: "Billing Items to Customers"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Billing Costs to Customers > Billing Items to Customers"
parent: "section_N1248576"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248901.html"
anchors: ["procedure_N1248950", "procedure_N1249580", "procedure_N1249638", "bridgehead_N1249697"]
sha256: "fe2b522993a6bf76be9d91aad05cb431a545fb8458a2ecc559476c0a1e0ee50e"
---

Billing items back to customers lets you to purchase items and supplies for an order or project, and then bill the cost to the customer. For example, a locksmith can bill a customer for a special safe they installed.

To bill items to customers, enable the feature first. An administrator can go to _Setup > Company > Enable Features_ > Transactions, check the **Bill Costs To Customers** box, and click **Save**.

When you enable the feature, you can bill items to customers on purchase orders or other purchase transactions.

Note:

If the Advanced Pricing feature is enabled, the value displayed in the Rate column on the Billable Items sublist is determined by your configured price rules. The rate will be sourced based on the transaction date specified on the Invoice or Cash Sale form. This may result in a different rate from the standard pricing.

Income from billable items goes to the income account setup in your Chart of Accounts.

Note:

For OneWorld accounts, you must also set up at least one tax schedule because Advanced Taxes is enabled in all OneWorld accounts.

Warning:

In accounts without OneWorld, you can bill costs to customers using items created before enabling the Advanced Taxes feature. If you enable Advanced Taxes after creating an item, you must assign a tax schedule to the item to bill a customer.

#### To bill items to customers using purchase orders: {#procedure_N1248950}

1.  Enter a purchase order for an item you want to bill to a customer.
    
    When you enter a purchase order for a billable item, select the item and identify the customer or project, and then check the **Billable** box.
    
    Note:
    
    You must bill the purchase order before you can bill the customer for the billable item.
    
    To enter a purchase order for a billable item, go to _Transactions > Purchases/Vendors > Enter Purchase Orders_.
    
    For more information about purchasing billable items, read [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html).
    
2.  Bill the purchase order that includes the item you want to bill to a customer.
    
    The bill for the billable item needs to identify the customer or project and have the **Billable** box checked.
    
    To bill a purchase order, go to _Transactions > Purchases/Vendors > Bill Purchase Orders_.
    
    For more information, read [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html).
    
    After the purchase order is billed, this item can show on the Billable Items subtab of the customer bill.
    
3.  Enter an invoice or cash sale to bill the customer for the billable item.
    
    When you create an invoice, apply the appropriate billable item on the **Billable Items** subtab. Click **Mark All** or **Unmark All** to check or clear all items that show on the subtab.
    
    -   To create an invoice, go to _Billing > Sales > Create Invoices_.
        
    -   For more information about creating an invoice, read [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html).
        
    -   To create a cash sale, go to _Billing > Sales > Enter Cash Sales._. For more information, see [Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244343.html).
        
        For more information about creating a cash sale, read [Entering a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244457.html).
        
4.  If you track class, department, and location at the line-item level, you can change these settings for this billable item.
    

When you create the invoice or cash sale, the customer is billed for the item.

#### To bill items to customers using checks: {#procedure_N1249580}

1.  Enter a check to pay a vendor for the item you want to bill to a customer. For more information, read [Adding Items to a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1544711.html).
    
2.  On the **Items** subtab of the check, select the item you want to bill to the customer.
    
3.  Identify the customer or project and check the **Billable** box.
    
4.  Complete additional fields on the check as necessary.
    
5.  Click **Save**.
    

Now, this item can show on the Billable Items subtab of the customer bill.

#### To bill items to customers using credit card transactions: {#procedure_N1249638}

1.  Enter a credit card transaction to pay a vendor for the item you want to bill to a customer. For more information, read [Entering Company Credit Card Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548500.html).
    
2.  On the **Items** subtab of the credit card transaction, select the item you want to bill to the customer.
    
3.  Identify the customer or project and check the **Billable** box.
    
4.  Complete additional fields on the credit card transaction as necessary.
    
5.  Click **Save**.
    

Now, this item can show on the Billable Items subtab of the customer bill.

## Items Billable By Default {#bridgehead_N1249697}

You can set the Items Billable by Default preference. This preference lets you check the **Billable** box by default when you're purchasing items. After you select a customer on an item line of a purchase transaction, the **Billable** box is automatically checked.

You can set the Items Billable by Default preference at _Setup > Accounting > Preferences > Accounting Preferences_ > Time & Expenses. This preference is dependent on the Bill Costs to Customers feature.

When billing items back to customers, you can include the date of service on all custom invoices except finance charge invoices. This is the date the bill for the items was entered.

### Related Topics

-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Billing Time to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1249803.html)
-   [Billing Expenses to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250082.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

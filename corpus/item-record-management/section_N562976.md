---
id: "section_N562976"
type: "section"
title: "Printing Labels From Transactions"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Bar Codes and Item Labels > Printing Labels From Transactions"
parent: "chapter_N2215205"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N562976.html"
anchors: ["procedure_N563041", "procedure_N563138", "subsect_1528235903", "procedure_1528235755", "subsect_1540225557"]
sha256: "45da0b2558b8549f8f89ae8e0213f26e58ac99b05490ade04bc9a250af2d7fc0"
---

You can generate labels for items directly from a purchase order, item receipt, or item fulfillment. This lets you print labels specifically for the items you are receiving, or expect to receive.

For example, a warehouse receiving employee views the PO for items delivered on the dock. The employee confirms that all items on the PO were shipped, and then clicks Print Labels. The PO is marked received and a PDF file opens with a label for each item in the shipment. The employee prints the labels and attaches one to each item before placing them on the shelves in stock.

To print labels, you need Adobe Reader. Visit the [Adobe Web](http://www.adobe.com/products/acrobat) site to download the latest version at no charge.

#### To print labels for items on a purchase order or item fulfillment: {#procedure_N563041}

1.  View the purchase order or item fulfillment you want to print a label for.
    
2.  Click the print icon, and select **Print Labels**.
    
    NetSuite opens the labels in the Adobe® application.
    
3.  Click the printer button in the Adobe application.
    
4.  Specify the number of copies on the print message that appears.
    
5.  Click **OK**.
    

#### To print labels for items from an item receipt: {#procedure_N563138}

1.  Go to _Transactions > Purchases/Vendors > Enter Purchase Orders > List_.
    
2.  Click **View** next to the receipt.
    
3.  Click the **Print** button.
    
    NetSuite opens the labels in the Adobe application.
    
4.  Click the printer button in the Adobe application.
    
5.  Specify the number of copies on the print message that appears.
    
6.  Click **OK**.
    

## Printing Lot Numbered Item Labels {#subsect_1528235903}

By default, when you print item labels from transactions, labels for lot numbered items are printed per lot number. You can use the Print Lot Item Labels From Transactions By Quantity accounting preference to configure labels to be printed by quantity. For example, consider an item receipt that has a line for Lot Item A, with a quantity of 12. By default, with the Print Lot Item Labels From Transactions By Quantity box cleared, one item label is printed for Lot Item A. If you check the box, 12 item labels are printed for Lot Item A.

#### To print lot numbered item labels from transactions by quantity: {#procedure_1528235755}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  On **the Items/Transactions** subtab, under Inventory, check the **Print Lot Item Labels From Transactions By Quantity** box.
    
3.  Click **Save**.
    

## Print a Shipping Label for a Vendor Return Authorization {#subsect_1540225557}

You can generate shipping labels for an authorized return from the vendor return authorization form. This enables you to print labels specifically for the items you're returning to a vendor. For more information, see [Shipping Authorized Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387332.html).

Note:

When printing a shipping label for a Vendor Return Authorization, the label Reference Number value (`label.refnumber`) is sourced from the **Ref. No.** field. All other shipping labels source the label Reference Number value from the **PO#** field.

You can customize the layout of your printed forms at _Transactions > Purchases/Vendors > Enter Purchase Orders > List_. For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

Note:

If you use the Canada Edition of NetSuite, you must set your preferred layout to the Standard Cheque Layout to comply with the most recent Canadian Payment Association guidelines.

Your administrator can customize the layout of your printed forms using Advanced PDF/HTML templates. For more information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

For more information about printing checks and forms for transactions, see [Printing Checks and Other Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566722.html) and [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html).

### Related Topics

-   [Using Code 128 Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292085605.html)
-   [Enabling the Bar Coding and Item Labels Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292087805.html)
-   [Printing Bar Code and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2215536.html)
-   [Scanning Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2218627.html)
-   [Processing Orders Using Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N561778.html)
-   [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2215536"
type: "section"
title: "Printing Bar Code and Item Labels"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Bar Codes and Item Labels > Printing Bar Code and Item Labels"
parent: "chapter_N2215205"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2215536.html"
anchors: ["bridgehead_N2218202", "bridgehead_N2218230"]
sha256: "abbf716d9377aae8bb1048814e1f5edb6b0ef5cceae434f630d0a5660c9bf058"
---

You can print labels to stick on your items. Labels can include the SKU (item number), item price, and item bar code. For serialized items, the label can also include the serial number bar code and serial number.

Your administrator can customize the layout of your printed forms using Advanced PDF/HTML templates. To learn more, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

Your user role must have Items permission set to the Edit or Full level to print bar codes and item labels. To learn more, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

The following applies to all bar codes when printing:

-   If a bar code is not resizable, NetSuite ignores Height and Width during printing. A third-party library used by NetSuite determines if a bar code is resizable.
    
-   Only for resizable bar codes, default Height and Width are used as follows:
    
    -   EAN13, UPCA =1 inch
        
    -   Code128 =none.
        
-   If the value for Height causes the Width to exceed the specified Width, the Width and Height are both adjusted to fit the label. If the value entered for Height does not cause the Width to exceed the specified width, the default width is used.
    

Note:

To print labels, you need Adobe Reader. Visit the [Adobe Web site](http://www.adobe.com/products/acrobat) to download the latest version at no charge.

You can print bar codes and item labels in the following ways:

-   [Bar Codes on Transactions](#bridgehead_N2218202)
    
-   [Item Labels From Item Records](#bridgehead_N2218230)
    
-   [Printing Item Labels in Bulk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2218255.html)
    
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N562976.html)
    

## Bar Codes on Transactions {#bridgehead_N2218202}

To print bar codes on transactions, click Print on the transaction as usual. Bar codes are automatically included on the transaction. You can also go to _Transactions > Management > Print Checks and Forms > Item Labels_ > Item Labels.

## Item Labels From Item Records {#bridgehead_N2218230}

#### To print a label for an item:

1.  From the item record, go to _Lists Accounting > Items._.
    
2.  Beside the item record you want to print a label for, click **View**.
    
3.  On the item record, click the **Print Label** button.
    
4.  When the barcode page opens, click the printer icon (![Printer icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/PrinterIcon.png)).
    
5.  In the **Destination** field, select your printer.
    
6.  Click **Print**.
    

### Related Topics

-   [Using Code 128 Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292085605.html)
-   [Enabling the Bar Coding and Item Labels Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292087805.html)
-   [Scanning Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2218627.html)
-   [Processing Orders Using Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N561778.html)
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N562976.html)
-   [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

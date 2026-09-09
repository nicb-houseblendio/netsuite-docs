---
id: "bridgehead_N2218255"
type: "bridgehead"
title: "Printing Item Labels in Bulk"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Bar Codes and Item Labels > Printing Bar Code and Item Labels > Printing Item Labels in Bulk"
parent: "section_N2215536"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2218255.html"
anchors: ["procedure_N2218264", "bridgehead_1493732461", "bridgehead_N2218560"]
sha256: "ddd74005e3700a67f4b05dc09a76e37abf7167fbbdd2e51ac5f51dfa54df0a76"
---

Use the following procedure to print item labels in bulk.

#### To bulk print labels: {#procedure_N2218264}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Item Labels**.
    
3.  On the Print Item Labels page, the **Item Type** field defaults to **Inventory Item**.
    
    You can select another item type, such as **Numbered Inventory**, to print labels for.
    
4.  Check the **Print Non-sellable Items** box to print labels for items not generally sold on a sales transaction. These items are more often used for information or pricing. Non-sellable items include description, discount, markup, and payment items.
    
5.  In the **Item Label Layout** field, select the layout you prefer to use to print.
    
    Note:
    
    The standard item label layout supports Avery 5260 labels.
    
    To create custom label layouts, go to _Customization > Forms > Transaction Forms_ and click **Customize** link next to **Standard Item Label Layout**.
    
6.  If you use Multiple Currencies, select which currency you want to print labels for.
    
7.  In the **Starting Label** field, enter a number to identify the location on the page you want to begin printing. For example, entering **1** starts printing in the first label on the sheet. This lets you save labels by printing on sheets that are partially used.
    
8.  Optionally, check one or more of the following boxes:
    
    -   **Print Name/Number Bar Code** - print the item name and bar code on each label
        
    -   **Print Display Name/Number** - print the display name on each label
        
    -   **Print Serial Number Bar Code** - print a bar code generated from the serial number in addition to the name/number bar code on each label
        
    -   **Print Expiration Date** - if you use lot items, print the expiration date on lot item labels
        
9.  If you want to print the price on each label:
    
    -   Check the **Print Sales Price** box
        
    -   Select a price level to print in the **Price Level** field
        
        Note:
        
        If a selected price level is not set on an item record, the next available set price level prints on the item's label. For more information, see [Setting Up Items for Multiple Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182221.html).
        
10.  Enter values in one or more of the item label list columns. For more information, see [Item Label List Columns](#bridgehead_1493732461).
     
11.  Click **Print**.
     
     -   If you don't use the Download PDF Files preference, a preview of your labels appears in Adobe Acrobat or Adobe Reader. This preference is in Home > Set Preferences.
         
     -   If you use the Download PDF Files preference, you must first save your labels, and then open them with the Adobe application.
         
     
     Place your labels in your printer tray.
     
12.  Click the printer button in the Adobe application frame.
     
13.  Click **OK**.
     

## Item Label List Columns {#bridgehead_1493732461}

| Field | Description |
| --- | --- |
| **Primary Information** |
| Print | Check the box next to each item you want to print a label for. |
| No. of Labels | Enter the number of labels you want to print for each item. The value in this field defaults to one label. |
| Starting Serial Num | If you've the Serialized Inventory feature enabled, enter the first serial number in the range you want to print. |
| Ending Serial Num | If you've the Serialized Inventory feature enabled, enter the last serial number in the range you want to print. |
| On Hand Only | If you've the Serialized Inventory feature enabled, check this box to print labels for only serial numbers in stock as of the transaction date. Clear this box to print labels for all serials numbers in the range. |

## Assemblies and Labels {#bridgehead_N2218560}

When you print labels for assembly items, you can print labels for each member item in addition to the assembly item. For more information, see [Printing Assembly Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324547.html).

### Related Topics

-   [Printing Bar Code and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2215536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

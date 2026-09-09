---
id: "section_N2277819"
type: "section"
title: "Updating Bin Putaway Worksheets"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Updating Bin Putaway Worksheets"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2277819.html"
anchors: ["procedure_N2275313", "procedure_N2277976"]
sha256: "29b5c1aca23d68e98df3eb41bb2ec4a773a4fbed4ab2c73359661554483af9ea"
---

Important:

The functions discussed in this topic require the Advanced Bin / Numbered Inventory Management feature to be enabled.

On a worksheet, you can enter the bin put away details, which include the bin numbers and item quantities. For advanced Bin Management, you can use worksheets to assign bins to specific lots or serial numbers.

If you have existing items or quantities prior to enabling basic or advanced Bin Management, worksheets enable you to assign the bins. You can also use them if you do not specify bins on inventory transactions, such as inventory adjustments or transfers.

Based on your worksheet entries, NetSuite automatically adjusts on-hand bin quantities. You can view the adjusted quantities on item records. For more information about worksheets, see [Put Away Items in Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html#bridgehead_N2270434).

Depending on which bin feature you use, follow the instructions in one of these topics:

-   [To update a basic putaway worksheet:](#procedure_N2275313)
    
-   [To update an advanced putaway worksheet:](#procedure_N2277976)
    

#### To update a basic putaway worksheet: {#procedure_N2275313}

1.  Go to _Transaction > Inventory > Bin Putaway Worksheet_.
    
2.  The **Date** field defaults to today's date. You can edit this date to put away items from previous days.
    
3.  If you use the Multi-Location Inventory feature, select your location.
    
4.  In the **Memo** field, you can enter notes for this day's putaway sheet.
    
5.  The **Quantity** column shows the total on-hand amount for each item at the location selected. Click this field to edit the total quantity.
    
6.  The **Units** column displays the unit of measurement used to determine the on-hand quantity. Click this field to select a different unit of measurement.
    
7.  The **Bins** column displays the bins associated with each item.
    
8.  The **Bin Numbers** column displays the preferred bin by default.
    
    -   If the total quantity is placed in the preferred bin, no edits are needed.
        
    -   If some items were or will be placed in some of the other bins listed in the **Bins** column, click the **Bins** icon. Edit the quantity for each bin, and click **Done**.
        
        You can also enter bin numbers separated by commas with on-hand quantities in parentheses. For example, you can enter **A101(50), A102(43)**.
        
9.  Click **Save**.
    

#### To update an advanced putaway worksheet: {#procedure_N2277976}

1.  Go to _Transaction > Inventory > Bin Putaway Worksheet_.
    
2.  The **Date** field defaults to today's date. You can edit this date to put away items from previous days.
    
3.  If you use the Multi-Location Inventory feature, select your location.
    
4.  In the **Memo** field, you can enter notes for this day's put away sheet.
    
5.  The **Quantity** column shows the total on-hand amount for each item at the location selected. Click this field to edit the total quantity.
    
6.  The **Units** column displays the unit of measurement used to determine the on-hand quantity. Click this field to select a different unit of measurement.
    
7.  Click the icon in the **Inventory Detail** column next to an item to edit bin quantities.
    
8.  In the Inventory Detail popup window, specify the bins and quantities to be put away as follows:
    
    1.  If the item is numbered, in the **Serial/Lot Number** list, select the appropriate number.
        
    2.  In the **Bin** list, select the bin you want the items put into.
        
        The **Bin** column displays the preferred bin by default.
        
    3.  In the **Quantity** field, enter the quantity of items to be put in this bin.
        
    4.  Click **Add**.
        
    5.  Repeat steps a - d to put away more of this item in other bins.
        
    6.  Click **OK**.
        
9.  Repeat steps 7 and 8 for any additional items you want to make changes to.
    
10.  Click **Save**.
     

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2229184"
type: "section"
title: "Adding Items to a Matrix"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Matrix Items > Adding Items to a Matrix"
parent: "section_N2227654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229184.html"
anchors: ["procedure_N2229227"]
sha256: "1c6f392a90a9df1267a32c1fb2154f0759ee82dd09b82cd3fb0a659694c11eb3"
---

A matrix item is a series of the same item available in different options.

You create matrix items by setting up the options and creating a parent item. After you create your matrix, you can create subitems for each option combination. These different options can have varying prices. If you use the web store feature, each option and price displays in the item's list.

Important:

Before you add subitems, make sure that you've created custom lists to represent all options for subitems.

For example, you want to create subitems of different sizes and colors for a parent t-shirt item. You should first create a custom list of size values and a custom list of color values. Go to Customization > Lists, Records, & Fields > Lists > New. For more information, see [Setting up Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html#bridgehead_N2228735).

#### To add items to a matrix: {#procedure_N2229227}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the parent item to which you want to add items.
    
3.  If an item you are adding has a price different from the parent item, enter pricing information about the **Pricing** subtab.
    
    Prices are listed in the option list for the item in the web store.
    
4.  Click the **Matrix** subtab, and then review the lists of available values for each matrix option.
    
5.  Select option values that you want to be available as subitems of the parent item.
    
    -   If a value you want to add for a matrix option is listed, select it.
        
    -   If a value you want to add is not listed, click the plus button to open the popup window. Enter a name and abbreviation for the new value, and then click **Save**. The new value is selected automatically, and this value is also added to the custom list for that matrix option.
        
    -   Pre-existing values **must remain selected** to avoid an error.
        
6.  Click **Add Items**.
    
7.  On the Add Matrix Items page, in the **Include** column, clear the boxes for any subitems you do not want to add.
    
8.  Click **Submit**.
    

Note:

You can add matrix items from CSV data files using the Import Assistant. For more information, see [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html).

### Related Topics

-   [Removing a Subitem From Your Item Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163335500375.html)
-   [Using the Matrix Item Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227918.html)
-   [Creating a Matrix Item Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228397.html)
-   [Setting up an Item Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html)
-   [Editing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229497.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

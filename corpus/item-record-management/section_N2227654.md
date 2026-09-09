---
id: "section_N2227654"
type: "section"
title: "Matrix Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Matrix Items"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html"
anchors: ["procedure_1173253451"]
sha256: "b613e6e122e6e6e156004b33541dffb4a07968d91183cafa769a6e16d2aca83d"
---

You can create and maintain your item records using an item matrix. An item matrix lets you track your items by options such as size and color. An item matrix consists of a parent item and subitems. With an item matrix, each combination is tracked separately.

For example, Wolfe Electronics sells blank compact disks for recording. These compact disks are available in different storage capacities and colors. With an item matrix, Wolfe can track each combination of color and storage separately without having to create an item record for each combination.

Note:

The parent item doesn't appear on transactions. Only child items that show each option can be chosen on transactions.

There are two methods for creating matrix items:

1.  You can create matrix items by using the Matrix Item Assistant. This functionality lets you create an item and all of the available options in single step-by-step interface.
    
2.  If you don't use the assistant, you can manually create matrix items. However, you must first set up matrix options using custom lists and fields.
    
    -   Use a **custom list** to create a list of the available options for matrix items. A separate list is required for each option.
        
        For example, you sell CD-Rs in different sizes and colors. You need a list of size options and a separate list of color options. After you create your lists of options, you need to create a custom item field for each list.
        
    -   **Custom item fields** are used on item records to select available options from your custom lists. You must create an item field for each option list.
        
    -   If the item appears in your commerce web store, you should also set up a **custom transaction item option**, which allows users to select the option on the item's product details page (PDP).
        

Please note the following:

-   Matrix items can't be created for groups or kits.
    
-   You can use the Import Assistant to import matrix options for the following items:
    
    -   inventory items
        
    -   lot numbered inventory items
        
    -   serialized inventory items
        
    -   non-inventory items
        
    -   other charge items
        
    -   assembly items
        
    -   service items
        
    
    For more information, see [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html).
    
-   The maximum number of the total combinations of matrix options is 2000.
    

#### To enable matrix items: {#procedure_1173253451}

1.  Go to Setup > Company > Enable Features.
    
2.  In the **Items & Inventory** subtab, check the **Matrix Items** box.
    
3.  Click **Save**.
    

### Related Topics

-   [Using the Matrix Item Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227918.html)
-   [Creating a Matrix Item Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228397.html)
-   [Setting up an Item Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html)
-   [Adding Items to a Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229184.html)
-   [Editing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229497.html)
-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
-   [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)
-   [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html)
-   [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)
-   [Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247990.html)
-   [Service Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248153.html)
-   [Download Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248348.html)
-   [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html)
-   [Subtotal Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248793.html)
-   [Description Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248894.html)
-   [Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248975.html)
-   [Expense Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4042372470.html)
-   [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html)
-   [Other Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249208.html)
-   [Payment Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249363.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

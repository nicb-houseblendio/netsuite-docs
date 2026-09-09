---
id: "section_N2229497"
type: "section"
title: "Editing Matrix Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Matrix Items > Editing Matrix Items"
parent: "section_N2227654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229497.html"
anchors: ["procedure_N2229627", "procedure_N2229689"]
sha256: "59a8f63029ac3f7fe59993ef953d4a21fc12c905ed1e639068a9882361282e15"
---

Matrix subitems can be edited individually or as a group from the parent item record.

Alternatively, you can use the Import Assistant to update matrix subitems by editing each subitem. For more information, see [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html).

You can edit the following fields on matrix subitems:

-   Item Name/Number
    
-   Display Name/Code
    
-   Vendor Name/Code
    
-   Purchase Description
    
-   Sales Description
    
-   Shipping Cost
    
-   Handling Cost
    
-   Item Weight
    
-   Purchase Price
    
-   Sales Price
    
-   Reorder Point
    

The remaining fields can only be edited on the parent matrix item. Fields edited on subitems are only changed for that item. Fields edited on the parent item can be applied to all or some of the subitems.

#### To edit a single matrix subitem: {#procedure_N2229627}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the matrix subitem you want to change.
    
3.  Make changes to any of the fields listed above.
    
4.  Click **Save**.
    

Only changes made to the fields listed above are saved on the individual subitem record. Any changes made to other fields are not saved.

#### To edit multiple matrix items: {#procedure_N2229689}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the parent matrix item for the matrix you want to change.
    
3.  Make changes to any of the fields for this matrix.
    
4.  Click **Update Matrix**.
    
5.  In the **Include** column, clear the boxes for any subitems you do not want to be updated with the new information.
    
6.  Click **Submit**.
    

If you use the Multiple Vendors feature, you can set a vendor code and price for each vendor on each child item. You can also set a preferred vendor for each child item. When you edit a parent item and then click **Update Matrix**, check the **Include** box next to vendor-related fields you want updated on child items.

Note:

When using Multiple Units of Measure, you can't edit Units Type on a parent item when a child item has a units type assigned. For more information, see [Assigning Units of Measure to Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212390.html).

#### To delete a matrix item:

1.  Go to Lists > Accounting > Items.
    
2.  Click **Edit** next to the matrix item for the matrix you want to change.
    
3.  Open the matrix you want to delete.
    
4.  In the **Actions** list, click **Delete**.
    
    Note:
    
    You can't delete a matrix item or matrix child item when the child item is referenced in a transaction.
    
5.  In the warning box, click **OK**.
    
6.  In the Mass Update Performed popup window, click **OK**.
    

#### To remove matrix options:

1.  Go to Lists > Accounting > Items.
    
2.  Beside the matrix item you want to change, click **Edit**.
    
3.  In the **Matrix** subtab, click **Remove Matrix Options**.
    
4.  On the Remove Matrix Options page, check the box beside the option you want to remove.
    
    At least one option must remain in the matrix.
    
    Note:
    
    You cannot remove matrix option items that are being used in other transactions.
    
5.  Click **Next**.
    
6.  After the matrix option has been removed, select the items you want to keep.
    
    Unselected items are deleted.
    
7.  Click **Submit**.
    
8.  In the warning box, click **OK**.
    

### Related Topics

-   [Using the Matrix Item Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227918.html)
-   [Creating a Matrix Item Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228397.html)
-   [Setting up an Item Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html)
-   [Adding Items to a Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229184.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

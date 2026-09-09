---
id: "section_N2228669"
type: "section"
title: "Setting up an Item Matrix"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Matrix Items > Setting up an Item Matrix"
parent: "section_N2227654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html"
anchors: ["bridgehead_N2228735", "procedure_N2228748", "bridgehead_N2228884", "procedure_N2228897", "subsect_164383640667"]
sha256: "f6c9bae24ced5ea2a56bfe9b2059470e8e433ffe828b0f6c948a2d41f6a1fe6f"
---

To create matrix item records, first set up your matrix options using custom lists and fields.

1.  Create a custom list for each available option. For example, set up a list of colors and then set up a list of sizes.
    
    For more information, see [Setting up Custom Lists](#bridgehead_N2228735).
    
2.  Set up a custom item field for each list you created. For example, create a custom item field for the list of colors. Then, create a custom item field for the list of sizes.
    
    For more information, see [Setting up Custom Item Fields](#bridgehead_N2228884).
    
3.  Set up a custom transaction item option for each option you create. This step lets users select the option on the product details page (PDP) of your web store.
    
    For more information, see [Setting Up Custom Transaction Item Options](#subsect_164383640667).
    

## Setting up Custom Lists {#bridgehead_N2228735}

A custom list is used to create a list of the available matrix item options. A separate list is required for each option. For example, you sell T-shirts in different sizes and colors. Therefore, you need a list of size options and a separate list of color options.

#### To set up a custom list of matrix options: {#procedure_N2228748}

1.  Go to _Customization > List, Records, & Fields > Lists > New_.
    
2.  In the **Name** field, enter a name for your custom list.
    
3.  Select the custom list **Owner** from the list. Only the owner can edit this record.
    
4.  Enter a **Description** of this list.
    
5.  Choose to show these options in either **The Order Entered** or in **Alphabetical Order**.
    
6.  To indicate that this list is for an item matrix, check the **Matrix Option List** box.
    
7.  Click the **Values** subtab and then complete the following:
    
    1.  In the **Value** column, enter the first value for your list.
        
    2.  In the **Abbreviation** column, enter an abbreviation for this value.
        
    3.  Check the **Inactive** box if you don't want this to show in lists.
        
    4.  Click **Add**.
        
    5.  Continue adding values and translations.
        
8.  When you've finished, click **Save**.
    
    Repeat these steps for each list of options for your matrix items.
    

After you create your lists of options, you need to create a custom item field for each of your lists.

## Setting up Custom Item Fields {#bridgehead_N2228884}

Custom item fields are used on your item records to select available options from your custom lists. You must create an item field for each option list.

#### To set up a custom item field for matrix items: {#procedure_N2228897}

1.  Go to _Customization > Lists, Records, & Fields > Item Fields > New_.
    
2.  In the **Label** field, enter the name of one of the custom lists you entered for this item matrix.
    
3.  Select the custom item field **Owner** from the list. Only the owner can edit this record.
    
4.  Enter a **Description** of this custom field.
    
5.  To indicate that this field is an option for matrix items, check the **Matrix Option** box.
    
    The **Type** field is automatically set to **Multiple Select** and the **Subtab** field is set to **Matrix**.
    
6.  Select the **Type** of field you want to create. The type of field is determined by the kind of information collected in this field.
    
    To use sourcing with this field, the field type must match the sourced field. If you checked the **Matrix Option** box, type is automatically set to **Multiple Select**.
    
7.  In the **List/Record** field, select your custom list.
    
8.  The **Store Value** box is checked by default. All information entered in this custom field is stored in your NetSuite account.
    
    Clear this box to indicate that the information stored in this custom field is for display only. The information isn't stored in your account.
    
9.  To have your custom item field appear in your items list, check the **Show In List** box.
    
10.  To index this custom field for global search, check the **Global Search** box. This field's values are searched for matches to global search keywords and records with matches are returned as global search results.
     
     If this box is unavailable, check **Store Value** box. If it is still unavailable, global search indexing isn't supported for the selected data type.
     
11.  If you're creating a List/Record custom field, check the **Record is Parent** box to indicate that the record type selected is a parent record. This field is used to create a parent-child relationship between two record types.
     
12.  Click the **Applies To** subtab and then check the boxes next to the kind of items you want to apply this field to.
     
     You can create matrix items for inventory, non-inventory, other charge, service, group, kit/packages, assembly/BOM items.
     
13.  Click **Save**.
     
     Repeat the steps on for each list of options for your matrix items.
     

### Setting Up Custom Transaction Item Options {#subsect_164383640667}

A custom transaction item option adds the option you created for the item matrix to the product details page (PDP). You only need to complete this step if you're setting up a matrix item for a web store.

#### To set up a custom transaction item option:

1.  Go to _Customization > Lists, Records, & Fields > Transaction Item Options > New_.
    
2.  Enter a **Label** and **ID** in the corresponding fields.
    
    Note:
    
    If you want multiple images to be displayed for an option, you'll need the ID when configuring the multi-image option for your SuiteCommerce website. See [(Optional) Configure Multi-Image Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162137343254.html#subsect_162137376332).
    
3.  In the **Type** field, select **List/Record**. In the **List/Record** field, select the name of the your custom list.
    
4.  Make sure the **Store Value** box is checked.
    
5.  In the **Applies To** subtab, check the boxes for **Purchase**, **Sale**, **Opportunity**, **Web Store**, **Transfer Order**, and **Apply to Kit/Assembly Component**. These checkboxes determine the transaction types the option can apply to.
    
6.  In the **Items** field, enter items you want to apply the option to. The custom option appears on the PDP for each item entered in this field. Don't check the **All Items** checkbox.
    
    Note:
    
    You can edit this transaction item option at any time to add or remove items from this list.
    
7.  Go to the **Sourcing & Filtering** subtab.
    
    1.  In the **Source List** field, select **Item**.
        
    2.  In the **Source From** field, select your custom item field.
        
8.  Click **Save**.
    

After you create your custom lists and custom item fields, you are ready to create your item matrix. Go to _Lists > Accounting > Items_.

### Related Topics

-   [Using the Matrix Item Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227918.html)
-   [Creating a Matrix Item Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228397.html)
-   [Adding Items to a Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229184.html)
-   [Editing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229497.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

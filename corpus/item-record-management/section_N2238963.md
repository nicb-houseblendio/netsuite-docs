---
id: "section_N2238963"
type: "section"
title: "Customizing Lot or Serial Numbered Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Customizing Lot or Serial Numbered Item Records"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html"
anchors: []
sha256: "23b8a4e23bbfe6ca0c44a2e09f673116058e1d370c23ef0413400a896a3d48da"
---

Serial and lot numbered inventory records can be customized with item number fields. These are fields you can add to item records to track information specific to each item or workflow unique to your business.

For example, you can track the status and results of quality control procedures specific to each serialized item. You can otherwise track recall information about lot records.

After you enter information in custom item number fields, you can search for items on sales transactions based on properties from the inventory number record. To do so, click **Search** next to the **Serial/Lot Numbers** field. Complete the **enter item memo or information** procedure in the [Receiving a Purchase Order With a Lot Numbered Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2236584.html) help topic.

#### To enter item memo or information:

1.  Go to _Transactions > Purchases > Receive Purchase Order > List_.
    
2.  Beside the order, click **View**.
    
3.  Beside the Serial or Lot number, click the Open icon.
    
4.  In the popup window, enter a memo and values in any custom fields for each inventory number.
    

#### To create custom item number fields:

1.  Go to _Customization > Lists, Records, & Fields > Item Number Fields_.
    
2.  On the custom item number field record, enter a name for the **Label**.
    
3.  (Optional) Enter the following information about your custom item number field:
    
    -   **ID** - You use the ID value when scripting to instances of the transaction type. As a best practice, enter a name that begins with an underscore. The text you enter is prepended with the string custitemnumber. If you don't enter a value, NetSuite generates one.
        
        If you are editing an existing custom transaction type, you can change the ID value. Click **Change ID** at the top of the page.
        
    -   **Owner** - Select the owner of this field. Only the owner can edit this record.
        
    -   **Description** - Enter a description of this field.
        
    -   **Type** - Select the type of field you want to create. The type of field is determined by the kind of information collected in this field.
        
        If you want to use sourcing with this field, the field type must match the field being sourced from.
        
    -   **List/Record** - If you choose **List/Record** in the **Type** field, select a custom list or list of records to use with this field.
        
        You must choose **List/Record** in the **Type** field before you can select a list.
        
    -   **Store Value** - This field is checked by default. The information entered is stored in the custom field.
        
        Clear this box if you don't want any changes entered to be stored in the custom field. This lets you look at data that is stored elsewhere.
        
        Note:
        
        If you don't store the value, changes will be discarded, so you should make the field read-only.
        
    -   **Use Encrypted Format** - Check this box to encrypt stored values for this field in the database (values are still displayed in the UI).
        
        Note:
        
        After you save this field, this option can't be changed.
        
        Important:
        
        Be aware of the following precautions:
        
        -   Fields with stored encrypted values are not available to reporting, ODBC views, or for sourcing or filtering. However, they can be returned in the results of searches and saved searches.
            
        -   The nlapiLookupField SuiteScript function is not supported for fields with stored encrypted values. Other SuiteScript API functions that rely on search may not be supported.
            
        -   Encryption of stored field values increases their size and may have performance implications.
            
        -   The data type of a field with stored encrypted values can't be changed to a type that doesn't support stored encrypted values.
            
        
    -   **Show in List** - Check this box to have your custom item field appear in your items list. The field appears on the **Serial Numbers** subtab of item records.
        
    -   **Inactive** - Check this box to inactivate this custom field. Similar to a deleted field, inactive custom fields don't appear on any forms or in global searches. You cannot select this kind of field from any lists on entities, items, or transactions.
        
        The data and settings of inactive fields are maintained in NetSuite. If you later make a field active again, all of its data is restored. In addition, the field appears on all of the same forms as before it was made inactive.
        
        Note:
        
        Inactive fields don't appear on the list page unless you check the **Show Inactives** box.
        
4.  Click the **Applies To** subtab.
    
5.  To add your custom field to a desired lot or serial numbered item record, select one of the following options:
    
    -   **Specific Items** - to apply your custom field to particular items.
        
        Choose the items the field applies to in the **Select Items to Apply Field**. Press and hold the **Ctrl** key to select more than one item.
        
    -   **All Items** - to apply your custom field to all active items.
        
        -   To apply this field to serialized items, check the **Serialized** box.
            
        -   To apply this field to lot numbered items, check the **Lots** box.
            
        -   To apply this field to gift certificates, check the **Gift Certificate** box.
            
6.  Click **Save**.
    

For more information, see [Creating Custom Item Number Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html) and [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).

Note:

Custom fields created for this record type are not available in SuiteAnalytics Workbooks or SuiteAnalytics.

### Related Topics

-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
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

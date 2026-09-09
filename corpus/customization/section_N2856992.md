---
id: "section_N2856992"
type: "section"
title: "Configuring Fields or Screens"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring Fields or Screens"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html"
anchors: ["procedure_N2857011"]
sha256: "a9290f928e91e4add2ba5fca388423f53196ead7f5448a15a5ad20c6f14b211a"
---

When the following subtabs are available on the current entry or transaction form, you can configure fields for that form:

-   **Screen Fields** subtab on transaction forms
    
-   **Fields** subtab on entry forms
    
-   **Sublist Fields** subtab on transaction forms
    

These fields can also be moved to display on an alternate subtab or in alternate field groups.

Note:

Even if you've disabled a subtab as described in [Configuring Subtabs for Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2855162.html), you can still configure fields for that subtab. This is useful if you later decide to include the subtab on your form.

#### To configure fields in the Screen Fields, Fields, or Sublist Fields subtab: {#procedure_N2857011}

1.  In the **Show** column, check the boxes next to the fields you want to display.
    
    Note:
    
    When configuring fields, be aware of the following:
    
    -   Hiding fields on a form can hide other related fields. For example, hiding **Credit Card Approved** on the sales order form also hides fields related to **Address Verification System (AVS)**.
        
    -   If you use multiple locations, you must show the **Location** field on the sales order form you use for your website to calculate shipping correctly.
        
    -   If an advanced template relies on a hidden sublist field, the template can fail to print. For more information, see [Using FreeMarker to Work with Hidden Fields Used in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156752233995.html).
        
    -   If Termination Reason Tracking is enabled, you can't save employee records if required termination fields are hidden. For more information, see [Termination Reason Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494530951.html).
        
    
2.  In the **Quick Add** column (Entry forms only), check the boxes next to the fields you want to define as inline editable and available in Quick Add portlets.
    
    If a field has both **Quick Add** and the **Enable Field Editing on Lists** checked, then that field can be directly edited, and the record is saved when you click off of the field. Inline editable fields are also available when attaching contacts or scheduling activities to records. For more information, see [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html).
    
    You can add Quick Add portlets to your dashboards. Quick Add portlets permit the quick addition of a selected record type without navigating to the record type page. For more information, see [Quick Add Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N588631.html).
    
3.  In the **Mandatory** column, check the boxes next to the fields that are required on your entry form.
    
    Note:
    
    You can't clear mandatory boxes for required NetSuite fields or custom fields defined as required in the custom field definition.
    
4.  In the **Display Type** column, select the display type for each field. For more information, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).
    
5.  In the **Check Box Default** column, choose one of the following options for each check box field on the form:
    
    -   **Use Field Default** - Use the default value set in the field definition.
        
    -   **Checked** - Set the default to checked, possibly overriding the default set in the field definition.
        
    -   **Unchecked** - Set the default to cleared, possibly overriding the default set in the field definition.
        
6.  In the **Label** field, edit the name of any of the fields as needed. Labels can be up to 200 characters long. However, you should consider how the length of a label appears on printed forms.
    
    -   If you change the label of a field on the **Sublist Fields** subtab, the new label is also applied to the field on the **Printing Fields** subtab.
        
    -   In accounts where the Multi-Language feature is enabled, the label you edit here applies only to your current language, as set at _Home > Set Preferences_. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).
        
    
    Note:
    
    Many forms and records in NetSuite include multiple types of address fields, such as billing (remittance), shipping, or site/pick-up addresses.
    
    When configuring your form, ensure you display the address field most relevant to your need (for example, the physical pick-up address rather than a remittance address). You can also update the label for the field label to clarify its purpose for users. For example, to prevent confusion, you could rename Address to Pick-up Address.
    
    If you're unable to find the correct address field, contact your administrator, because custom address fields may need to be added or made visible for your particular process.
    
7.  In the **Field Groups** list, select the group where you want the field to appear.
    
    Note:
    
    After you assign a field to a field group, the field can be moved only within the group. If you want to move the field elsewhere on a form, you must change its field group.
    
8.  In the **Column Break** column, check any field to insert a column break beginning with that field.
    
    Be aware that inserting a column break after a field can cause field text to display in a way you may not expect based on the display size attributes set for custom fields. For more information, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).
    
9.  To include a blank line before a field, enter the number of blank lines in the **Space Before** column.
    
10.  To associate a field with the field immediately above it, check the **Same Row as Previous** box. An associated field shares the same **Show** or **Hide** setting as the previous field. The field belongs to the same field group as the previous field and is displayed together on the form with the previous field. For more information, see [Associating Related Fields on Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857453.html).
     
11.  Rearrange fields as needed.
     
     -   To move each field to the preferred subtab, click **Move Elements Between Subtabs**. For more information, see [Moving Fields and Lists Between Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860592.html).
         
     -   Rearrange the order of the fields on each subtab. Select and drag each line item to the preferred position or click **Move to Top** or **Move to Bottom**.
         
         Note:
         
         Fields that belong to a field group can be moved only within the group. If you want to move the field elsewhere on a form, either change the field group for the field or rearrange the field groups.
         
         Unassigned fields are listed together below all other fields that are assigned to field groups. These unassigned fields are always displayed last and can be reordered among all other unassigned fields. If you want to move a field up higher on a subtab, assign it to a field group.
         
12.  For transaction forms only, set the following options:
     
     -   In the **Check Box Default** column, set the default value for check box fields. If you set the **Check Box Default** field to **Checked** for a transaction form field, the box for that field will automatically be checked. You can clear the box if needed.
         
     -   Click the **Sublist Fields** and arrange the line-item columns for your transaction entry form by moving fields as needed. The order of the columns on the screen does **not** have to match the order of the printed columns of your form.
         
13.  On the **Sublist Fields** subtab, in the **Items Filter** field, select a saved search to use to filter the items that appear in the Items list on this form. For more information, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
     
14.  On the **Total Box** subtab, specify which fields to show in the form totals.
     
     If you use SuiteTax, additional tax fields are available. For more information, see [Tax Details on Transactions in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4283867856.html).
     
15.  Click **Save**.
     
16.  If required, to create any new custom fields, click **New Field**.
     
     Note:
     
     Ensure that you save any changes before creating new fields from within the form. When you click **New Field**, you leave the custom form to go to the custom field page. For more information, see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html).
     
17.  For transaction forms only, after configuring the fields or screens, you should configure the printing fields. For more information, see [Configuring Printing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858172.html).
     

Important:

As you configure your custom form, consider whether the transactions to use on the form require tax data. You can't specify tax field names through form customization. You must go to _Setup > Accounting > Set Up Taxes_. For more details, see [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

### Related Topics

-   [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html)
-   [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html)
-   [Custom Transaction Forms Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html)
-   [Storing Custom Forms with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2854025.html)
-   [Configuring Subtabs for Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2855162.html)
-   [Moving Fields and Lists Between Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860592.html)
-   [Configuring Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856559.html)
-   [Configuring Buttons and Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857647.html)
-   [Configuring Printing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858172.html)
-   [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html)
-   [Configuring Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515597095.html)
-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
-   [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html)
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

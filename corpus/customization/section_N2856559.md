---
id: "section_N2856559"
type: "section"
title: "Configuring Field Groups"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring Field Groups"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856559.html"
anchors: ["procedure_N2856644"]
sha256: "9aa83a5b8dbd7fb41bc8ad0e996d3957adf9987c5879742f72b8a8ca348c26a9"
---

This topic provides an overview of field groups in NetSuite and describes how to configure field groups on standard forms. If you want to add or manage field groups on custom record custom forms, see [Adding Field Groups to Custom Forms of Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2856753.html).

Use the Field Groups subtab to customize the field groups that appear on your forms. Field groups support body fields only. You can't create a field group for sublist fields.

You can use the Field Groups subtab to change the UI label of a field group, the fields within the field group, and the placement of a field group on the page. You can also use the Field Groups subtab to create new field groups and organize all fields into specific field groups. The order of field groups on the Field Groups subtab determines the order of field groups on your form.

Any unassigned fields are listed together below all other fields that are assigned to field groups. These unassigned fields are always displayed last and can be reordered among all other unassigned fields. If you want to move a field up higher on a subtab, assign it to a field group.

Be aware that adding custom fields to field groups can change how field text displays, regardless of the display size attributes set for the custom fields. For more information, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).

#### To configure field groups: {#procedure_N2856644}

1.  Click the **Field Groups** subtab.
    
2.  To customize field groups that appear in the main body area of a page, click **Main**. To customize the field groups that appear on other subtabs on the form, click another field group subtab.
    
    ![Field Groups subtab menu.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/fieldGroups.png)
3.  In the **Label** column, edit field group headings.
    
4.  In the **Show** column, clear a field group to hide it on the form.
    
5.  In the **Single Column** column, to have the column display vertically rather than horizontally, check a field group. The following screenshot provides an example of the Primary Information field group displayed vertically.
    
    ![Sample field group vertical layout.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/fieldGroupVerticalLayout.png)
    
    Note that if you select **Single Column** for three field groups together, the field groups appear side by side in the UI, because three field group columns make a row.
    
    ![Sample field group side-by-side layout.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/FieldGroupsSideBySide.jpg)
6.  To delete a field group, click the **X** icon. The fields display at the bottom of the page. However, the fields aren't assigned to any field group because that field group has been deleted.
    
7.  After configuring your field groups, you can click the **Fields** subtab (for Entry forms) or the **Screen Fields** subtab (for Transaction forms) to configure the fields that appear in each field group. For more information, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).
    

For information about managing field groups on custom forms for custom records, see [Adding Field Groups to Custom Forms of Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2856753.html).

### Related Topics

-   [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html)
-   [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html)
-   [Custom Transaction Forms Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html)
-   [Storing Custom Forms with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2854025.html)
-   [Configuring Subtabs for Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2855162.html)
-   [Moving Fields and Lists Between Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860592.html)
-   [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html)
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

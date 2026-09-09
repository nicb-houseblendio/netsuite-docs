---
id: "bridgehead_N2859744"
type: "bridgehead"
title: "Configuring QuickViews for Upgraded Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring QuickViews > Configuring QuickViews for Upgraded Forms"
parent: "section_N2859666"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2859744.html"
anchors: ["procedure_N2859762"]
sha256: "648658a167abffbedf404642952e43bbe1fe9de58aba3bd4f0fa37adcde214d7"
---

This topic describes how to configure QuickViews on upgraded entry and transaction forms. For more information about QuickViews or instructions for custom records, see [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html).

QuickView customization works best if you've upgraded the custom forms in your account to include field groups and all other look-and-feel enhancements introduced in NetSuite in a previous release. After a form has been upgraded, a **QuickView** configuration subtab appears on the form customization page. You use this subtab to add, remove, and rearrange the fields in a QuickView.

#### To configure QuickViews: {#procedure_N2859762}

1.  Open the Custom Form or Custom Transaction form you want to edit. For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).
    
2.  On the Edit Custom Entry \[or Transaction\] Form page, click the **QuickView** subtab.
    
    If the page doesn't have a **QuickView** subtab, this means that the form hasn't been upgraded/deployed yet. For more information, see [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)
    
3.  In the **Field Description** column, add the fields you want to appear in the QuickView for records that use this form. After you select the field, click **Add**. To remove a field, click the X icon on the right side of the field.
    
4.  Click **Save**.
    

Note these additional guidelines when customizing your QuickViews:

-   If you customize a form's QuickView and select **Store Form with Record**, these customizations supersede any customization made to a form set to **Form is Preferred**.
    
-   During form customization, if you make field updates on the **Fields** subtab, you must save the form customization page before those updates appear on the **QuickView** subtab.
    
-   On the **Fields** subtab, if a field isn't set to **Show**, the field doesn't appear in the QuickView, even if you add the field on the **QuickView** subtab.
    
-   The fields that appear on the QuickView subtab match the fields listed in the **Description** column on the **Fields** subtab. However, on the QuickView subtab the custom label for the field displays.
    
-   The list of fields available on the **QuickView** subtab includes all of the fields that are on a record. The list includes fields that appear on a record when it's in View mode and Edit mode. Fields that appear on a record **only** when the record is in Edit mode don't appear in QuickViews. If you add a field to a QuickView, yet the field does not appear when the QuickView displays, you may have added a field that's visible only when the record is in Edit mode.
    

See also: [Configuring QuickViews for Nonupgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/ridgehead_N2860013.html).

### Related Topics

-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
-   [Configuring QuickViews for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_95152126340.html)
-   [Configuring QuickViews for Nonupgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/ridgehead_N2860013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

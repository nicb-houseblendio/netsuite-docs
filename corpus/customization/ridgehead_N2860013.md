---
id: "ridgehead_N2860013"
type: "ridgehead"
title: "Configuring QuickViews for Nonupgraded Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring QuickViews > Configuring QuickViews for Nonupgraded Forms"
parent: "section_N2859666"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/ridgehead_N2860013.html"
anchors: []
sha256: "925a1ed3f1c5511a9de2f16f1427d810f81fad27f22126e30a026adac9352cdc"
---

This topic explains the limitations of customizing QuickViews on nonupgraded forms and shows how you can indirectly control QuickView fields by configuring and deploying an upgraded form. For information about checking the upgrade status of your forms, see [How to Tell if the Custom Forms in Your Account are Upgraded](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2860381.html).

If you haven't upgraded the custom forms in your account to include the look-and-feel changes introduced in a previous version, you can't directly edit or customize the default QuickView fields assigned by NetSuite. Nonupgraded forms don't include the QuickViews configuration subtab on entry and transaction form customization pages.

You can, however, indirectly affect which fields appear in a QuickView by creating an equivalent upgraded form. You can then use the QuickViews subtab on the newly upgraded form to make QuickView customizations. Then you must set this form to Form is Preferred. By doing so, even the records in your account that use the nonupgraded version of the form show the QuickView customizations of the upgraded form.

Also note the following when attempting to customize QuickViews for nonupgraded forms:

-   A nonupgraded stored form shows the customizations of an upgraded preferred form or standard form if there's no preferred form.
    
-   Even if you click Store Form with Record on a nonupgraded form, the QuickViews that appear for records using this form show the QuickView customizations (if any) on the upgraded form.
    
-   If a standard form is marked as preferred, then all QuickViews for both nonupgraded and upgraded forms show the NetSuite default QuickView fields for that record type.
    

See also: [Configuring QuickViews for Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2859744.html)

### Related Topics

-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
-   [Configuring QuickViews for Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2859744.html)
-   [Configuring QuickViews for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_95152126340.html)
-   [How to Tell if the Custom Forms in Your Account are Upgraded](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2860381.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2898929"
type: "section"
title: "Upgrade Logic for Fields (Diagram)"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Understanding Form Layout Enhancement Upgrade Logic > Upgrade Logic for Fields (Diagram)"
parent: "section_N2897877"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2898929.html"
anchors: []
sha256: "840c386df42c72f0bab105ecc68c1fc94cf2464e324e57e39116883044b46bff"
---

The following diagram visually represents the field arrangement concepts discussed in [Upgrade Logic for Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2898251.html). Technically, all NetSuite fields appear on subtabs, even fields that appear in the main body of the form are (technically speaking) located on a subtab called **Main**.

The following diagram shows the subtab assignment for fields in a 'V1' (nonupgraded) environment and a 'V2' (upgraded) environment.

Note the following in the diagram:

-   V1 indicates the existing form, and V2 indicates the upgraded form
    
-   Boxes outlined in red highlight the scenarios where a field's location (subtab) changes when a form is upgraded.
    
-   <New Std Location> means that NetSuite automatically moves the field to a new subtab, existing subtab, or to the Main subtab based on the field's data.
    
-   Main is one example of a subtab that is valid for both V1 and V2 forms.
    
-   General is one example of a subtab that is removed when forms are upgraded.
    
-   Some standard fields that are common across forms have been moved to a new location for better logical grouping. The move is consistent across forms.
    

Note:

To enlarge the diagram, press Ctrl+Plus Sign. To return your screen to its usual size, press Ctrl+Minus Sign.

![Field assignment flow diagram.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/FieldAssignmentDiagram2CustomOnly.png)

To create custom layouts, go to _Customization > Forms > Transaction Form PDF Layouts or Customization > Forms > Transaction Form HTML Layouts_, and click the Customize link next to a layout. Make your changes and click Save. You can choose default layouts to apply to one or more types of forms by checking boxes in the Preferred column at Customization > Forms > Transaction Form PDF Layouts or Customization > Forms > Transaction Form HTML Layouts, and clicking Submit.

### Related Topics

-   [Understanding Form Layout Enhancement Upgrade Logic](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897877.html)
-   [Upgrade Logic for Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2898251.html)
-   [Upgrade Logic for Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2898743.html)
-   [Field Ordering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2899497.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

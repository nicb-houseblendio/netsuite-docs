---
id: "bridgehead_N2885392"
type: "bridgehead"
title: "Using NetSuite Tags"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Online Custom Record Forms > Creating HTML Templates for Online Custom Record Forms > Using NetSuite Tags"
parent: "section_N2885246"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885392.html"
anchors: ["procedure_N2885416"]
sha256: "5d631ed623959026ce26b9cf7f80f07fab2483c026ee15126544e9464e9ce526"
---

Field tags in an HTML form are defined as <NLTAG>, where TAG is the ID of the field. Each field in NetSuite has a unique ID and therefore a unique tag definition.

Note:

Field IDs are incorporated into tag definitions for fields. When creating custom fields to use in HTML templates, you should specify IDs for each field and use consistent naming conventions that make sense in your business environment. If the default NetSuite IDs are accepted when creating your custom fields, the tags may not make sense in your HTML code. The result can make it more difficult to know exactly what the field references.

If you've chosen to include a required Name field on your custom record, you must include the tag, <NLNAME>, for that field in your template.

#### To determine the tags to use for each field on your custom record: {#procedure_N2885416}

1.  Click _Customization > List, Records, & Fields > Record Types_.
    
2.  In the **Edit** column, click the name of the record type you want to create a template for.
    
3.  On the **Fields** subtab, click the name of the field you want to place in your template.
    
4.  The URL for this page is displayed in the Address bar of your browser. The ID for the selected field is at the end of the URL.
    

### Related Topics

-   [Creating HTML Templates for Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885246.html)
-   [Creating an HTML Template Locally](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885320.html)
-   [Uploading an HTML Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885453.html)
-   [Creating an HTML Form Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885567.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "bridgehead_N3211830"
type: "bridgehead"
title: "Determining Field IDs on a Child Record Sublist"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Custom Sublists > Custom Child Record Sublist Creation with SuiteScript > Custom Child Record Sublist IDs Overview > Determining Field IDs on a Child Record Sublist"
parent: "section_1502309332"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3211830.html"
anchors: []
sha256: "da20881aa3e9600f12909aa3485ce0382b741a7d040c3368d286b0e8b802188b"
---

This topic outlines the process for identifying field internal IDs on a custom child record sublist. For a general overview, see [Custom Child Record Sublist IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502309332.html).

Use these steps to get internal field IDs on a custom child record sublist:

1.  Go to the custom record definition page (for example, go to _Customization > Lists, Records, & Fields > Record Types_ and select your custom record in the **Record Types** list).
    
2.  On the Fields subtab of the Custom Record Type page, all field internal IDs appear in the ID column. These are the IDs you reference as the `fieldId` value in [Record.getSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273166148.html) or [CurrentRecord.getSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637583237.html).
    
    ![Sample Fixed Assest custom record type with ID fields highlighted on the Fields subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/recmachsublist10_2.png)
    
    **Example:**
    
                  `//Get the value of the Cost field on the first line (see the following figure) ... var sublistFieldValue = objRecord.getSublistValue({ sublistId: 'irecmachcustrecord102', fieldId: 'custrecord1', line: 1 });` 
                
    
    You can get or set values for fields that appear in the Fixed Assets sublist. You can also set or get values that exist on the record, but don't appear in the sublist UI.
    
    For example, the following line sets the value of the **Salvage Value** field in the fixed assets record 14 (see the following screenshot). The internal ID for Salvage Value is custrecord2. See this value on the Custom Record Type definition page for the fixed assets record type.
    
                  `objRecord.setCurrentSublistValue({ sublistId: 'recmachcustrecord102', fieldId: 'custrecord2', });` 
                
    
    ![Sample customer record highlighting a row on the Fixed Assets subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/recmachsublist11.png)

### Related Topics

-   [Custom Child Record Sublist IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502309332.html)
-   [Determining the Sublist ID for a Child Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3211618.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

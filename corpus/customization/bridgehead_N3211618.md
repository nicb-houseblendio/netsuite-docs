---
id: "bridgehead_N3211618"
type: "bridgehead"
title: "Determining the Sublist ID for a Child Record"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Custom Sublists > Custom Child Record Sublist Creation with SuiteScript > Custom Child Record Sublist IDs Overview > Determining the Sublist ID for a Child Record"
parent: "section_1502309332"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3211618.html"
anchors: ["subsect_161954855107", "procedure_N3211674", "subsect_161954865660"]
sha256: "3614444b7d9b472c549d8e81d0791985a5c8dd8309e0a083baac93ec48ac09ba"
---

This topic explains where and how to find the internal ID of a custom child record sublist in NetSuite. For a general overview, see [Custom Child Record Sublist IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502309332.html).

The internal ID for a custom child record sublist is **recmach** + field\_id\_for\_the\_parent\_field (for example: recmachcustrecord102).

Use [Record.getSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273166148.html) or [CurrentRecord.getSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637583237.html).

          `// Add code. ... var sublistFieldValue = objRecord.getSublistValue({ sublistId: 'item', fieldId: 'item', line: 3 }); ... // Add code.` 
        

## Finding the Internal ID of a Custom Child Record Sublist {#subsect_161954855107}

The following steps describe where to look in NetSuite to get the internal ID of a custom child record sublist.

#### To get the internal ID of a custom child record sublist (the field ID for the parent record): {#procedure_N3211674}

1.  Go to the record definition for the custom record type. For example, Fixed Assets, as shown in the following screenshot.
    
2.  On the **Fields** subtab, notice that the **ID** column lists a List/Record field type.
    
    The **New Customer** field (internal ID: **custrecord102**) is the parent field for the fixed assets records that appear as children on customer records. Therefore, the internal ID for the custom child Fixed Assets sublist on customer records is **recmachcustrecord102**.
    
    ![Sample Fixed Assets custom record type highlighting where to find the custom child internal ID.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/recmachsublist7.png)

## Obtaining the Internal ID of the Parent Field {#subsect_161954865660}

The following is an alternative approach for obtaining the internal ID of the parent field.

#### To obtain the internal ID of the parent field:

1.  On the custom child record sublist, click the New child record button. In the following example, the button is New Fixed Assets.
    
    ![Sample customer record Fixed Assets subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/recmachsublist8.png)
2.  When the new child record opens, notice the field that ties the child record to the parent record.
    
    In this case, the **New Customer** field shows that the customer record for Abe Simpson is the parent of the fixed assets record. The field level help popup window for **New Customer** lists the field's internal ID as custrecord102. Therefore, the internal ID for the Fixed Assets sublist appearing on the (parent) customer record is **recmachcustrecord102**.
    
    ![Sample Field Help highlighting the Field ID.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/recmachsublist9.png)

Note:

Internal IDs for custom child record sublists also appear in the SuiteScript Debugger when you load the record that includes the sublist.

### Related Topics

-   [Custom Child Record Sublist IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502309332.html)
-   [Determining Field IDs on a Child Record Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3211830.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

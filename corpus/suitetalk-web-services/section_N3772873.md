---
id: "section_N3772873"
type: "section"
title: "Entity Custom Field"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > Entity Custom Field"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3772873.html"
anchors: ["bridgehead_N3772891", "bridgehead_N3773095", "bridgehead_1523284961", "bridgehead_1523285026", "bridgehead_1523285038", "bridgehead_1523285048"]
sha256: "9cb8bfa1c73e46a02d6a344e83c0562f7f7c3309614121cd683901c4cda75fc9"
---

Custom entity fields are fields that you can add to your entity records to gather information specific to your business needs. Entity custom fields can be added to existing and custom subtabs on the entry forms you use to enter entity records in your NetSuite account.

For information about working with these fields in the UI, see [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html).

The entity custom field record is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3772891}

The following operations can be used with entity custom field.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3773095}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [entity custom field](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/entitycustomfield.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#bridgehead_1523284961}

The following sample adds a custom field to the customer record.

## Java {#bridgehead_1523285026}

          `public void testAddCustomField() throws Exception { EntityCustomField ClubCard = new EntityCustomField(); ClubCard.setLabel("Club-Card"); ClubCard.setAppliesToCustomer(Boolean.TRUE); ClubCard.setDefaultChecked(Boolean.FALSE); ClubCard.setFieldType(CustomizationFieldType._checkBox); c.addRecord(ClubCard); }` 
        

## SOAP Request {#bridgehead_1523285038}

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns6:EntityCustomField" xmlns:ns6="urn:customization_2017_1.setup.webservices.netsuite.com"> <ns6:fieldType xsi:type="ns7:CustomizationFieldType" xmlns:ns7="urn:types.customization_2017_1.setup.webservices.netsuite.com">_checkBox</ns6:fieldType> <ns6:label xsi:type="xsd:string">Club-Card</ns6:label> <ns6:defaultChecked xsi:type="xsd:boolean">false</ns6:defaultChecked> <ns6:appliesToCustomer xsi:type="xsd:boolean">true</ns6:appliesToCustomer> </record> </add> </soapenv:Body>` 
        

## SOAP Response {#bridgehead_1523285048}

          `<soapenv:Body> <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponse> <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/> <baseRef scriptId="custentity2" internalId="358" type="entityCustomField" xsi:type="platformCore:CustomizationRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/> </writeResponse> </addResponse> </soapenv:Body>` 
        

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

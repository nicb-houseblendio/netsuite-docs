---
id: "section_N3772071"
type: "section"
title: "Custom List"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > Custom List"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3772071.html"
anchors: ["bridgehead_N3772087", "bridgehead_N3772290", "bridgehead_N3772327"]
sha256: "f3a1d8ef5ac7e823714600510aba61c964f2e88c9ea33e036213d2bf443ccb3c"
---

A custom list is a list of values that you can use in custom fields on your forms and records. Custom lists enable you to set up predefined choices for your employees and customers to select when entering transactions and records.

For more information about working with this record in the UI, see [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html).

The custom list record is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3772087}

The following operations can be used with custom list.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3772290}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [custom list](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customlist.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3772327}

The following Java sample shows how to create a custom list with three values using SOAP web services.

          `CustomListCustomValue Beginner = new CustomListCustomValue();       Beginner.setValue("Beginner");       CustomListCustomValue Intermediate = new CustomListCustomValue();       Intermediate.setValue("Intermediate");       CustomListCustomValue Advanced = new CustomListCustomValue();       Advanced.setValue("Advanced");                     CustomListCustomValueList customValueList = new CustomListCustomValueList();       customValueList.setCustomValue(new CustomListCustomValue[]{Beginner, Intermediate, Advanced});              CustomList customList = new CustomList();       customList.setName("IT Proficiency Levels");       customList.setDescription("List of IT proficiency levels");       customList.setCustomValueList(customValueList);              c.addRecord(customList);` 
        

The following SOAP sample shows how to set a value from a custom list onto a record (in this case a Contact record) using SOAP web services.

          `<soapenv:Body> <platformMsgs:add xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:s0="urn:relationships_2017_1.lists.webservices.netsuite.com" xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformMsgs:record xsi:type="s0:Contact"> <s0:entityId>Clint Eastwood</s0:entityId> <s0:customFieldList> <platformCore:customField xsi:type="platformCore:SelectCustomFieldRef" scriptId="custentity6"> <platformCore:value typeId="7" internalId="2" /> </platformCore:customField> </s0:customFieldList> </platformMsgs:record> </platformMsgs:add> </soapenv:Body>` 
        

**Where:**

-   scriptId="custentity6" is the name of the custom list as it appears on the Contact record.
    
-   typeId="7" is the custom list internal id (Customization > Lists, Records, & Fields > Lists - Internal ID)
    
-   internalId="2" is the internal id of the second item on the custom list (Customization > Lists, Records, & Fields > Lists > List - ID)
    

Also note that when working with custom lists in SOAP web services, you can update specific values in a custom list using **valueId** as the key field for the CustomListCustomValue sublist and setting replaceAll flag to FALSE.

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3775025"
type: "section"
title: "Transaction Line Custom Field"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > Transaction Line Custom Field"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3775025.html"
anchors: ["bridgehead_N3775043", "bridgehead_N3775246", "bridgehead_N3775283", "bridgehead_N28990551", "bridgehead_N28990611"]
sha256: "e1bb2175e59c3a728ef7cd2fa2d8c1c142d563425f39f84b0815b7ec6ac37d47"
---

Custom transaction line fields are fields that you can add to the line items of your transaction records to gather information specific to your business needs.

For more information, see [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html).

The transaction line custom field record is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3775043}

The following operations can be used with transaction line custom field.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3775246}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record.

Note:

In the SOAP Schema Browser, this record is called transaction column custom field.

For details, see the SOAP Schema Browser's [transaction column custom field](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/transactioncolumncustomfield.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#bridgehead_N3775283}

The following sample shows how to set transaction line custom fields.

## SOAP {#bridgehead_N28990551}

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns9:SalesOrder" xmlns:ns9="urn:sales_2017_1.transactions.webservices.netsuite.com"> <ns9:entity internalId="2" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com" /> <ns9:itemList replaceAll="false" xsi:type="ns9:SalesOrderItemList"> <ns9:item xsi:type="ns9:SalesOrderItem"> <ns9:item internalId="34" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com" /> <ns9:quantity xsi:type="xsd:double">3.0</ns9:quantity> <ns9:customFieldList xsi:type="ns12:CustomFieldList" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"> <ns12:customField scriptId="custcol_my_bool" xsi:type="ns12:BooleanCustomFieldRef"> <ns12:value xsi:type="xsd:boolean">true</ns12:value> </ns12:customField> <ns12:customField scriptId="custcol_my_string" xsi:type="ns12:StringCustomFieldRef"> <ns12:value xsi:type="xsd:string">hello world</ns12:value> </ns12:customField> <ns12:customField scriptId="custcol_my_integer" xsi:type="ns12:LongCustomFieldRef"> <ns12:value xsi:type="xsd:long">100</ns12:value> </ns12:customField> </ns9:customFieldList> </ns9:item> </ns9:itemList> </record> </add> </soapenv:Body>` 
        

## Java {#bridgehead_N28990611}

          `SalesOrder so = new SalesOrder();  RecordRef entityRef = new RecordRef(); entityRef.setType(RecordType.customer); entityRef.setInternalId("2"); so.setEntity(entityRef);  SalesOrderItem soi = new SalesOrderItem();  RecordRef itemRef = new RecordRef(); itemRef.setType(RecordType.inventoryItem); itemRef.setInternalId("34"); soi.setItem(itemRef); soi.setQuantity(new Double(3));  BooleanCustomFieldRef cf1 = new BooleanCustomFieldRef(true, "custcol_my_bool"); StringCustomFieldRef cf2 = new StringCustomFieldRef("hello world", "custcol_my_string"); LongCustomFieldRef cf3 = new LongCustomFieldRef(100, "custcol_my_integer");  soi.setCustomFieldList(new CustomFieldList(new CustomFieldRef[]{cf1, cf2, cf3})); so.setItemList(new SalesOrderItemList(new SalesOrderItem[]{soi}, true));` 
        

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

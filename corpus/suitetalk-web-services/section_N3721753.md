---
id: "section_N3721753"
type: "section"
title: "Noninventory Resale Item"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Noninventory Resale Item"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3721753.html"
anchors: ["bridgehead_N3721765", "bridgehead_N3721988", "subsect_161485643659"]
sha256: "37e7cd793fb82b074089d28523ba2529d488139fd5adb880ec7cc848676b8fb6"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Non-Inventory Resale Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0120114938.html).

Noninventory resale item records are used to track something you buy and then sell for a profit, but do not stock.

For more information, see [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html).

## Supported Operations {#bridgehead_N3721765}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3721988}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser' s [noninventory resale item](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/noninventoryresaleitem.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#subsect_161485643659}

See the following code sample of the add operation:

            `NonInventoryResaleItem nonInventoryResaleItem = new NonInventoryResaleItem();         RecordRef taxSchedule = new RecordRef();         taxSchedule.setInternalId("1");         RecordRef department = new RecordRef();         department.setInternalId("2");         nonInventoryResaleItem.setItemId("New NonInventoryResaleItem");         nonInventoryResaleItem.setDisplayName("Item Display Name");         nonInventoryResaleItem.setTaxSchedule(taxSchedule);         nonInventoryResaleItem.setDepartment(department);         c.addRecord(nonInventoryResaleItem);      [SOAP request] <soapenv:Body>     <add xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">          <record xsi:type="ns7:NonInventoryResaleItem" xmlns:ns7="urn:accounting_2019_1.lists.webservices.netsuite.com">             <ns7:taxSchedule internalId="1" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2019_1.platform.webservices.netsuite.com"/>             <ns7:itemId xsi:type="xsd:string">New NonInventoryResaleItem</ns7:itemID>             <ns7:displayName xsi:type="xsd:string">Item Display Name</ns7:displayName>             <ns7department internalId="1" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2019_1.platform.webservices.netsuite.com"/>          </record>       </add> </soapenv:Body>  [SOAP response] <soapenv:Body>       <addResponse xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">          <writeResponse>             <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                <platformCore:statusDetail>                   <platformCore:afterSubmitFailed>false</platformCore:afterSubmitFailed>                </platformCore:statusDetail>             </platformCore:status>             <baseRef internalId="247" type="nonInventoryResaleItem" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com"/>          </writeResponse>       </addResponse> </soapenv:Body>` 
          

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3747185"
type: "section"
title: "Item Revision"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Item Revision"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3747185.html"
anchors: ["bridgehead_N3747230", "bridgehead_N3747396", "bridgehead_N3747433", "bridgehead_N3747452", "bridgehead_N3747464", "bridgehead_N3747476", "bridgehead_N3747492", "bridgehead_N3747504"]
sha256: "e0e1e75dd73cd127dc097e51b4fd49d64b7d4a880c15ec08521426e3943bc0cb"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Item Revision](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_9213001923.html).

The exact member components needed for assembly items are identified in the Bill of Materials (BOM), but required components may change over time. These changing requirements can be documented in item revision records, which are part of BOM member control functionality. Item revision records define which member items should be included in assembly builds during specific time frames.

An item revision record sets an effective date for a member item to be included in assembly builds. Each item revision record can be assigned to multiple assembly items, because one item can be a member of different assembly items.

For more details about this functionality, see [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html).

This record is available when the Assembly Items feature is enabled.

The item revision record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3747230}

The following operations can be used with the item revision record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3747396}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [item revision](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/itemrevision.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3747433}

The obsoleteDate field is read-only.

## Code Samples {#bridgehead_N3747452}

The following code adds an item revision.

## SOAP Request {#bridgehead_N3747464}

          `<soapenv:Body>   <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <record xsi:type="ns6:ItemRevision" xmlns:ns6="urn:accounting_2017_1.lists.webservices.netsuite.com">     <ns6:item internalId="109" type="assemblyItem" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>     <ns6:name xsi:type="xsd:string">WS added revision</ns6:name>     <ns6:effectiveDate xsi:type="xsd:dateTime">2012-03-06T23:00:00.000Z</ns6:effectiveDate>     <ns6:memo xsi:type="xsd:string">WS added memo</ns6:memo>     <ns6:inactive xsi:type="xsd:boolean">true</ns6:inactive>    </record>   </add> </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3747476}

          `<soapenv:Body>          <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef internalId="3" type="itemRevision" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>          </addResponse>       </soapenv:Body>` 
        

The following code gets item revision data.

## SOAP Request {#bridgehead_N3747492}

          `<soapenv:Body>            <get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <baseRef internalId="3" type="itemRevision" xsi:type="ns6:RecordRef" xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com"/>            </get>        </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3747504}

          `<soapenv:Body>          <getResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <readResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <record internalId="3" xsi:type="listAcct:ItemRevision" xmlns:listAcct="urn:accounting_2017_1.lists.webservices.netsuite.com">                   <listAcct:item internalId="109" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>assembly test item</platformCore:name>                   </listAcct:item>                   <listAcct:name>WS added revision</listAcct:name>                   <listAcct:effectiveDate>2012-03-06T00:00:00.000-08:00</listAcct:effectiveDate>                   <listAcct:memo>WS added memo</listAcct:memo>                   <listAcct:inactive>true</listAcct:inactive>                </record>             </readResponse>          </getResponse>       </soapenv:Body>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)
-   [Creating Revision Records for BOM Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335150.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

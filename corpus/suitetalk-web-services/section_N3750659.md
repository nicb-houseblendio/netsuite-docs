---
id: "section_N3750659"
type: "section"
title: "Manufacturing Routing"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Manufacturing Routing"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3750659.html"
anchors: ["bridgehead_N3750713", "bridgehead_N3750971", "bridgehead_N3751009", "bridgehead_N3751021", "bridgehead_N3751033", "procedure_N3751075", "bridgehead_N3751163", "bridgehead_N28871791", "bridgehead_N28871851", "bridgehead_N3751197"]
sha256: "de970c5ef9eafff71ba55cc1b4030b04a3ea15edfbebb81a5f4cf4ea2723c2a4"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_11203701840.html).

If the Manufacturing Routing and Work Center feature has been enabled, you can use SOAP web services to interact with manufacturing routing records. You can verify whether the feature is enabled by going to _Setup > Company > Setup Tasks > Enable Features_, and reviewing the Items & Inventory subtab.

The benefit of this feature is that it extends the Work In Process (WIP) feature, allowing you to specify a sequence of steps required for the completion of a WIP work order. You take advantage of this feature using a few records, including manufacturing routing. The routing record defines a series of tasks that must be completed by specific employee groups. When you save a WIP work order that references a particular manufacturing routing record, each step described in the routing record becomes a manufacturing operation task.

For details on manually creating a routing record, see [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html). For more information about the Manufacturing Routing and Work Center feature, see [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html).

The manufacturing routing record is defined in the [listScm](https://webservices.netsuite.com/xsd/lists/v2025_2_0/supplyChain.xsd) XSD.

## Supported Operations {#bridgehead_N3750713}

The following operations can be used with the manufacturing routing record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) |[getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) |[getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3750971}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [manufacturing routing](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/manufacturingrouting.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3751009}

Refer to the following sections for more details on working with manufacturing routing records.

## Prerequisites for Creating a Record {#bridgehead_N3751021}

When you create a routing record, certain records must already exist in NetSuite, as follows:

## Assembly Item {#bridgehead_N3751033}

Each routing record is created for use with a specific assembly item. You reference an assembly item using the Item element. For details on assembly items, see [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html). For details on using SOAP web services to interact with assembly items, see [Assembly Item (BOM Item)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713949.html).

## Cost Template and Work Center {#procedure_N3751075}

For each routing record you create, at least one entry is required in the routingStep sublist. Each sublist entry must reference one of the each of the following:

-   Cost Template - You reference an existing cost template record using the manufacturingCostTemplate element. For more on the cost template record in general, see [Creating Manufacturing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html). For details on using SOAP web services to interact with cost templates, see [Manufacturing Cost Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3748057.html).
    
-   Work Center - You set a value for work center using the manufacturingWorkCenter element. A work center is a static employee group record that has been flagged as a Manufacturing Work Center. For more details, see [Creating Manufacturing Work Centers or Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344727.html).
    

## Sample Code {#bridgehead_N3751163}

The following code illustrates how to add a manufacturing routing record.

## Java {#bridgehead_N28871791}

          `public void testAddRecord() throws Exception {   // This operation requires a valid session this.login(true);   ManufacturingRouting mfgRouting = new ManufacturingRouting();   //BODY FIELDS mfgRouting.setItem(mrr("167")); //Assembly Item mfgRouting.setName("ManufacturingRouting1"); mfgRouting.setMemo("ManufacturingRouting1Memo"); mfgRouting.setSubsidiary(new RecordRef(null, "1", null, RecordType.subsidiary));   RecordRefList rfList = new RecordRefList(); rfList.setRecordRef(new RecordRef[] {new RecordRef(null, "1", null, RecordType.location)});   mfgRouting.setLocationList(rfList); mfgRouting.setIsDefault(true);   //SUBLIST ManufacturingRoutingRoutingStepList stepsList = new ManufacturingRoutingRoutingStepList(); ManufacturingRoutingRoutingStep step1 = new ManufacturingRoutingRoutingStep(); step1.setOperationSequence(1L); step1.setOperationName("mfgRoutingOpName1"); step1.setManufacturingWorkCenter(new RecordRef(null, "3513", null, RecordType.entityGroup)); step1.setManufacturingCostTemplate(new RecordRef(null, "4301", null, RecordType.manufacturingCostTemplate)); step1.setSetupTime(1.11D); step1.setRunRate(2.22D);   stepsList.setManufacturingRoutingRoutingStep(new ManufacturingRoutingRoutingStep[] {step1});   mfgRouting.setRoutingStepList(stepsList);   c.addRecord(mfgRouting);` 
        

## SOAP Request {#bridgehead_N28871851}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">        <soapenv:Header>            <ns1:passport soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" soapenv:mustUnderstand="0" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">                <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">nlbuild@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">password</ns3:password>                <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">3604360</ns4:account>                <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>            </ns1:passport>        </soapenv:Header>        <soapenv:Body>            <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record xsi:type="ns6:ManufacturingRouting" xmlns:ns6="urn:supplychain_2017_1.lists.webservices.netsuite.com">                    <ns6:subsidiary internalId="1" type="subsidiary" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:item internalId="167" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:locationList xsi:type="ns9:RecordRefList" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns9:recordRef internalId="1" type="location" xsi:type="ns9:RecordRef"/>                                   </ns6:locationList>                    <ns6:name xsi:type="xsd:string">ManufacturingRouting1</ns6:name>                       <ns6:memo xsi:type="xsd:string">ManufacturingRouting1Memo</ns6:memo>                    <ns6:isDefault xsi:type="xsd:boolean">true</ns6:isDefault>                    <ns6:routingStepList replaceAll="false" xsi:type="ns6:ManufacturingRoutingRoutingStepList">                        <ns6:manufacturingRoutingRoutingStep xsi:type="ns6:ManufacturingRoutingRoutingStep">                         <ns6:operationSequence xsi:type="xsd:long">1</ns6:operationSequence>                         <ns6:operationName xsi:type="xsd:string">mfgRoutingOpName1</ns6:operationName>                         <ns6:manufacturingWorkCenter internalId="3513" type="entityGroup" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                         <ns6:manufacturingCostTemplate internalId="4301" type="manufacturingCostTemplate" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                         <ns6:setupTime xsi:type="xsd:double">1.11</ns6:setupTime>                         <ns6:runRate xsi:type="xsd:double">2.22</ns6:runRate>                     </ns6:manufacturingRoutingRoutingStep>                 </ns6:routingStepList>             </record>         </add>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N3751197}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">                   <platformMsgs:nsId>WEBSERVICES_3604360_031120131494382039617284600_ea972a8d42cc</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             <baseRef internalId="2201" type="manufacturingRouting" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          </writeResponse>       </addResponse>    </soapenv:Body> </soapenv:Envelope>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [Manufacturing Cost Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3748057.html)
-   [Manufacturing Operation Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684116.html)
-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

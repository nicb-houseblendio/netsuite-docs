---
id: "section_N3748057"
type: "section"
title: "Manufacturing Cost Template"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Manufacturing Cost Template"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3748057.html"
anchors: ["bridgehead_N3748111", "bridgehead_N3748369", "bridgehead_N3748406", "bridgehead_N3748418", "bridgehead_N3748430", "bridgehead_N3748458", "bridgehead_N3748505", "bridgehead_N28866911", "bridgehead_N28866971", "bridgehead_N3748538"]
sha256: "0040d9b66051dd95cb944acb01b5a3d650cf35fb613e8bb67cb81894d0ca0ff6"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Manufacturing Cost Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_34202720474.html).

If the Manufacturing Routing and Work Center feature has been enabled, you can use SOAP web services to interact with manufacturing cost template records. You can see whether the feature is enabled by going to _Setup > Company > Setup Tasks > Enable Features_, and reviewing the Items & Inventory subtab.

The benefit of this feature is that it lets you specify a sequence of tasks required for the completion of a Work In Process (WIP) work order. You take advantage of this feature using a few records, including cost template. The purpose of the cost template record is to group together the various expenses associated with a specific activity. These expenses might include the cost of paying employees, operating machinery, and so on.

For details on the process of manually creating a cost template, see [Creating Manufacturing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html). For more information about the Manufacturing Routing and Work Center feature, see [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html).

The manufacturing cost template record is defined in the [listScm](https://webservices.netsuite.com/xsd/lists/v2025_2_0/supplyChain.xsd) XSD.

## Supported Operations {#bridgehead_N3748111}

The following operations can be used with the manufacturing cost template record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) |[getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) |[getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3748369}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [manufacturing cost template](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/manufacturingcosttemplate.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3748406}

Refer to the following sections for more details on interacting with manufacturing cost template records.

## Prerequisites for Adding a Record {#bridgehead_N3748418}

When you create a cost template record, at least one row is required in the costDetail sublist. Each sublist entry must reference certain records that already exist in NetSuite, including at least one cost category and one item, as described below.

## Cost Category {#bridgehead_N3748430}

You reference an existing cost category record using the costCategory element. Note that the category referenced must use one of the cost types designed for use with manufacturing routing. These types are described in [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html). This topic also describes important restrictions regarding cost types that can be referenced only one time on a cost template record. Failure to follow these guidelines results in an error.

## Item {#bridgehead_N3748458}

You reference an existing item record using the item element. The function of the item record is to represent a specific expense that belongs to a manufacturing routing cost category. Only certain types of items can be set up this way. For more details, see [Defining a Manufacturing Charge Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2343650.html).

## Sample Code {#bridgehead_N3748505}

The following code illustrates how to add a manufacturing cost template record.

## Java {#bridgehead_N28866911}

          `public void testAddRecord() throws Exception    {   // This operation requires a valid session this.login(true);   ManufacturingCostTemplate mct = new ManufacturingCostTemplate();   //subsidiary mct.setSubsidiary(new RecordRef(null, "1", null, RecordType.subsidiary));   //name mct.setName("ManufacturingCostTemplate");   //memo mct.setMemo("ManufacturingCostTemplateMemo");   //cost detail ManufacturingCostTemplateCostDetailList mctcdl = new ManufacturingCostTemplateCostDetailList();   ManufacturingCostTemplateCostDetail mctcd1 = new ManufacturingCostTemplateCostDetail();   //line #1 mctcd1.setCostCategory(new RecordRef(null, "1", null, RecordType.costCategory)); mctcd1.setItem(new RecordRef(null, "4639", null, RecordType.otherChargePurchaseItem));   mctcdl.setManufacturingCostTemplateCostDetail(new ManufacturingCostTemplateCostDetail[] {mctcd1});   mct.setCostDetailList(mctcdl);   c.addRecord(mct); }` 
        

## SOAP Request {#bridgehead_N28866971}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">        <soapenv:Header>            <ns1:passport soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" soapenv:mustUnderstand="0" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">                <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">nlbuild@netsuite.com</ns2:email>                <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">password</ns3:password>                <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">3604360</ns4:account>                <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>            </ns1:passport>        </soapenv:Header>     <soapenv:Body>         <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns6:ManufacturingCostTemplate" xmlns:ns6="urn:supplychain_2017_1.lists.webservices.netsuite.com">                 <ns6:subsidiary internalId="1" type="subsidiary" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:name xsi:type="xsd:string">ManufacturingCostTemplate</ns6:name>                 <ns6:memo xsi:type="xsd:string">ManufacturingCostTemplateMemo</ns6:memo>                 <ns6:costDetailList replaceAll="false" xsi:type="ns6:ManufacturingCostTemplateCostDetailList">                     <ns6:manufacturingCostTemplateCostDetail xsi:type="ns6:ManufacturingCostTemplateCostDetail">                         <ns6:costCategory internalId="1" type="costCategory" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                         <ns6:item internalId="4639" type="otherChargePurchaseItem" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                     </ns6:manufacturingCostTemplateCostDetail>                 </ns6:costDetailList>             </record>         </add>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N3748538}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">          <platformMsgs:nsId>WEBSERVICES_3604360_031120131489538171800510632_a6b8a93ca56e</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef internalId="4402" type="manufacturingCostTemplate" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>          </addResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

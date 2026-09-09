---
id: "section_N3684116"
type: "section"
title: "Manufacturing Operation Task"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Manufacturing Operation Task"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684116.html"
anchors: ["bridgehead_N3684170", "bridgehead_N3684437", "bridgehead_N3684474", "bridgehead_N3684486", "bridgehead_N3684498", "bridgehead_N3684573", "bridgehead_N28449481", "bridgehead_N28449541", "bridgehead_N3684606"]
sha256: "acd11f64b4c33d682d1e83d08436d67c5fd1ba8f06d1b8ccd2c99a03ba75e47b"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Manufacturing Operation Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_66202904244.html).

If the Manufacturing Routing and Work Center feature has been enabled, you can use SOAP web services to work with manufacturing operation task records. You can verify that the feature is enabled by going to _Setup > Company > Setup Tasks > Enable Features_, and reviewing the Items & Inventory subtab.

The Manufacturing Routing and Work Center feature lets you specify a sequence of tasks required for the completion of a Work In Process (WIP) work order. This record represents a job that must be completed by a specific employee group. In the UI, generally these records are created automatically when you save a WIP work order that references a specific routing record - each step described in the routing record becomes an operation task record, viewable on the work order's Operations subtab. You can also manually create an operation task record by clicking the New Operation Task button on the work order's Operations subtab. You can view all existing manufacturing operation task records by going to _Transactions > Manufacturing > Manufacturing Operation Tasks_.

For more details about this record, see [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html). For more information about the Manufacturing Routing and Work Center feature, see [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html).

The manufacturing operation task record is defined in the listScm XSD.

## Supported Operations {#bridgehead_N3684170}

The following operations can be used with the operation task record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) |[getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) |[getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3684437}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [manufacturing operation task](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/manufacturingoperationtask.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3684474}

Refer to the following sections for more details on working with manufacturing operation task records.

## Prerequisites for Creating a Record {#bridgehead_N3684486}

Before you can add a manufacturing operation task record, a WIP work order that references a routing record must already exist in your system. To create an operation task record, you must reference this work order using the workOrder element.

## Required Fields {#bridgehead_N3684498}

Be aware of the following characteristics of this record's required fields:

-   Operation Sequence - The numeric value entered for this field must be greater than the largest Operation Sequence value already listed on the work order's Operations subtab. You set this field using the operationSequence element.
    
-   Operation Name - In SOAP web services, you set this value using the title element.
    

Other fields are also required. It may be useful to refer to [Manufacturing Operation Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2347042.html) for more details about the record and its required fields.

## Sample Code {#bridgehead_N3684573}

The following code illustrates how to add a manufacturing operation task record.

## Java {#bridgehead_N28449481}

          `public void testAddOperationTask() throws Exception{ // This operation requires a valid session this.login(true);   ManufacturingOperationTask manufacturingOperationTask = new ManufacturingOperationTask(); RecordRef workOrderRef = new RecordRef(); workOrderRef.setInternalId("65"); manufacturingOperationTask.setWorkOrder(workOrderRef); manufacturingOperationTask.setTitle("Task title"); manufacturingOperationTask.setOperationSequence(3L); manufacturingOperationTask.setSetupTime(30.0); manufacturingOperationTask.setRunRate(20.0); RecordRef costTemplateRef = new RecordRef(); costTemplateRef.setInternalId("1"); manufacturingOperationTask.setManufacturingCostTemplate(costTemplateRef); RecordRef workCenterRef = new RecordRef(); workCenterRef.setInternalId("113"); manufacturingOperationTask.setManufacturingWorkCenter(workCenterRef); manufacturingOperationTask.setMachineResources(14L); manufacturingOperationTask.setLaborResources(17L); c.addRecord(manufacturingOperationTask); }` 
        

## SOAP Request {#bridgehead_N28449541}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <ns1:passport soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" soapenv:mustUnderstand="0" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">nlbuild@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">password</ns3:password>             <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">3604360</ns4:account>             <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>          </ns1:passport>          <ns6:preferences soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" soapenv:mustUnderstand="0" xmlns:ns6="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns6:ignoreReadOnlyFields>true</ns6:ignoreReadOnlyFields>          </ns6:preferences>       </soapenv:Header>       <soapenv:Body>          <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns7:ManufacturingOperationTask" xmlns:ns7="urn:supplychain_2017_1.lists.webservices.netsuite.com">                <ns7:manufacturingWorkCenter internalId="113" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns7:manufacturingCostTemplate internalId="1" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns7:title xsi:type="xsd:string">Task title</ns7:title>                <ns7:operationSequence xsi:type="xsd:long">3</ns7:operationSequence>                <ns7:workOrder internalId="65" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns7:setupTime xsi:type="xsd:double">30.0</ns7:setupTime>                <ns7:runRate xsi:type="xsd:double">20.0</ns7:runRate>                <ns7:machineResources xsi:type="xsd:long">14</ns7:machineResources>                <ns7:laborResources xsi:type="xsd:long">17</ns7:laborResources>             </record>          </add>       </soapenv:Body>    </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N3684606}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_3604360_0311201314979673951785156835_4047dcfafa5</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef internalId="716" type="manufacturingOperationTask" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>          </addResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

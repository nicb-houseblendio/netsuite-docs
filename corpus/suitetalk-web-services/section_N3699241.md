---
id: "section_N3699241"
type: "section"
title: "Work Order Close"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Work Order Close"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3699241.html"
anchors: ["bridgehead_N3699277", "bridgehead_N3700958", "bridgehead_N3700995", "bridgehead_N3701007", "bridgehead_N3701054", "bridgehead_N3701090", "bridgehead_N3701102", "bridgehead_N3701114", "bridgehead_N28563801", "bridgehead_N28563861", "bridgehead_N28563921", "bridgehead_N28563981", "bridgehead_N3701169", "bridgehead_N3701180", "bridgehead_N28564221", "bridgehead_N3701203", "bridgehead_N3701214"]
sha256: "1903a53b21e53636b0740a3b40a96f348856966d8b9b962dbf47081a5b0bb2e8"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Work Order Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_37213527353.html).

If the Manufacturing Work In Process (WIP) feature has been enabled, you can use SOAP web services to interact with work order close records. You can verify whether WIP is enabled by going to Setup > Company > Enable Features, and reviewing the Items & Inventory subtab.

With WIP, instead of creating a single assembly build record to denote that a work order has been addressed, you track progress of the work using three records: work order issue, work order completion, and work order close. This approach lets you manage the assembly process in a more granular way, and to keep the General Ledger up to date as materials move through the different phases of assembly. For more on the benefits of WIP, see [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html).

The work order close record is used to indicate that all accounting variances that might have arisen during the assembly process have been resolved. In the UI, you can view the form used for creating this record by viewing the work order and clicking the Close button.

The work order issue record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

## Supported Operations {#bridgehead_N3699277}

The following operations can be used with work order close records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3700958}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [work order close](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/workorderclose.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3700995}

Refer to the following sections for more details on interacting with work order close records.

## Prerequisites for Creating a Record {#bridgehead_N3701007}

Before you can create a work order close record, a work order record must already exist, and the work order must be configured to use WIP (the WIP box on the work order record must be selected). This is true regardless of whether you are creating the work order close record using initialize and add, or add by itself. If you try to create a work order close record referencing a work order that has _not_ been configured to use WIP, the system generates an error reading in part, 'One of the following problems exists: You have an invalid work order < _work order ID_ >, the work order does not use WIP, or the work order is already closed.'

You can create and modify work orders by choosing _Transactions > Manufacturing > Enter Work Orders_. You can also interact with work orders using SOAP web services, as described in [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html).

It does not matter if a work order issue record or a work order completion exists for your work order. You can go straight from entering the work order to creating the work order close record.

## Using Initialize Versus Add {#bridgehead_N3701054}

You can initialize a work order close record from a [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html) record. This is the preferred approach, though you can also create the record using the add operation by itself.

The initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

If you are using the add operation by itself, note that you must use the createdFrom field to identify the appropriate work order. If you fail to set a value for this field, the system generates an error reading, 'Transaction can only be created from a work order.'

## The ComponentList Sublist Is Not Returned During a Get {#bridgehead_N3701090}

Note that the componentList sublist is not exposed, so performing a get operation on the work order close record will not include the items. This is true even though you can view the sublist in the UI when you display the work order close record there. The sublist is read only, and read-only sublists generally are not exposed.

## Sample Code {#bridgehead_N3701102}

The following code illustrates how to add a work order close record using a few different techniques.

## Using Initialize {#bridgehead_N3701114}

This example shows how to create a work order close record using both the initialize and add operations, which is the preferred approach. Note that this technique results in two SOAP requests and two SOAP responses.

## Java {#bridgehead_N28563801}

          `InitializeRef initRef = new InitializeRef(); initRef.setType(InitializeRefType.workOrder); initRef.setInternalId("167");   WorkOrderClose woRecord = (WorkOrderClose) c.initialize(initRef,InitializeType.workOrderClose,null);   c.addRecord(woRecord);` 
        

## SOAP Request (Initialize) {#bridgehead_N28563861}

          `<soapenv:Body>      <initialize xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <initializeRecord>              <ns7:type xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">workOrderClose</ns7:type>              <ns8:reference internalId="167" type="workOrder" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>          </initializeRecord>      </initialize>  </soapenv:Body>` 
        

## SOAP Response (Initialize) {#bridgehead_N28563921}

          `<soapenv:Body>    <initializeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <readResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <record xsi:type="tranInvt:WorkOrderClose" xmlns:tranInvt="urn:inventory_2017_1.transactions.webservices.netsuite.com">             <tranInvt:createdDate>2013-03-07T07:10:00.000-08:00</tranInvt:createdDate>             <tranInvt:lastModifiedDate>2013-03-07T08:25:00.000-08:00</tranInvt:lastModifiedDate>             <tranInvt:tranId>1</tranInvt:tranId>             <tranInvt:item internalId="247" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>JS Assembly Item Y</platformCore:name>             </tranInvt:item>             <tranInvt:orderQuantity>5.0</tranInvt:orderQuantity>             <tranInvt:createdFrom internalId="167" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Work Order #1</platformCore:name>             </tranInvt:createdFrom>             <tranInvt:tranDate>2013-03-07T00:00:00.000-08:00</tranInvt:tranDate>             <tranInvt:postingPeriod internalId="141" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Mar 2013</platformCore:name>             </tranInvt:postingPeriod>             <tranInvt:subsidiary internalId="3" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>SUB  UK</platformCore:name>             </tranInvt:subsidiary>             <tranInvt:location internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Location UK</platformCore:name>             </tranInvt:location>             <tranInvt:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:customField internalId="43" scriptId="custbody_633637_bsubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="165" scriptId="custbody_633637_bload" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="65" scriptId="custbody_633637_asubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>             </tranInvt:customFieldList>          </record>       </readResponse>    </initializeResponse> </soapenv:Body>` 
        

## SOAP Request (Add) {#bridgehead_N28563981}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record xsi:type="ns7:WorkOrderClose" xmlns:ns7="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns7:createdDate xsi:type="xsd:dateTime">2013-03-07T15:10:00.000Z</ns7:createdDate>              <ns7:lastModifiedDate xsi:type="xsd:dateTime">2013-03-07T16:25:00.000Z</ns7:lastModifiedDate>              <ns7:tranId xsi:type="xsd:string">1</ns7:tranId>              <ns7:item internalId="247" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns8:name xsi:type="xsd:string">JS Assembly Item Y</ns8:name>              </ns7:item>              <ns7:orderQuantity xsi:type="xsd:double">5.0</ns7:orderQuantity>              <ns7:createdFrom internalId="167" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns9:name xsi:type="xsd:string">Work Order #1</ns9:name>              </ns7:createdFrom>              <ns7:tranDate xsi:type="xsd:dateTime">2013-03-07T08:00:00.000Z</ns7:tranDate>              <ns7:postingPeriod internalId="141" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns10:name xsi:type="xsd:string">Mar 2013</ns10:name>              </ns7:postingPeriod>              <ns7:subsidiary internalId="3" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns11:name xsi:type="xsd:string">SUB  UK</ns11:name>              </ns7:subsidiary>              <ns7:location internalId="2" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns12:name xsi:type="xsd:string">Location UK</ns12:name>              </ns7:location>              <ns7:customFieldList xsi:type="ns13:CustomFieldList" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns13:customField scriptId="custbody_633637_bsubmit" xsi:type="ns13:BooleanCustomFieldRef">                <ns13:value xsi:type="xsd:boolean">false</ns13:value>                  </ns13:customField>                <ns13:customField scriptId="custbody_633637_bload" xsi:type="ns13:BooleanCustomFieldRef">                   <ns13:value xsi:type="xsd:boolean">false</ns13:value>                  </ns13:customField>             <ns13:customField scriptId="custbody_633637_asubmit" xsi:type="ns13:BooleanCustomFieldRef">                <ns13:value xsi:type="xsd:boolean">false</ns13:value>                  </ns13:customField>           </ns7:customFieldList>       </record>    </add> </soapenv:Body>` 
        

## SOAP Response (Add) {#bridgehead_N3701169}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="270" type="workOrderClose" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

## Using Add {#bridgehead_N3701180}

This example shows how to create a work order close record using the add operation alone.

## Java {#bridgehead_N28564221}

          `RecordRef createdFromRef = new RecordRef(); createdFromRef.setInternalId("167");   RecordRef postingPeriodRef = new RecordRef(); postingPeriodRef.setInternalId("141");   RecordRef departmentRef = new RecordRef(); departmentRef.setInternalId("2");   RecordRef classRef = new RecordRef(); classRef.setInternalId("2");   WorkOrderClose newWOCl = new WorkOrderClose(); newWOCl.setExternalId("WOCl-JS-001-TEST"); newWOCl.setTranId("TEST WOCl #1"); newWOCl.setCreatedFrom(createdFromRef); newWOCl.setPostingPeriod(postingPeriodRef); newWOCl.setDepartment(departmentRef); newWOCl.set_class(classRef); newWOCl.setMemo("Memo text");   c.addRecord(newWOCl);` 
        

## SOAP Request {#bridgehead_N3701203}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record externalId="WOCl-JS-001-TEST" xsi:type="ns6:WorkOrderClose" xmlns:ns6="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns6:tranId xsi:type="xsd:string">TEST WOCl #1</ns6:tranId>              <ns6:createdFrom internalId="167" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:postingPeriod internalId="141" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:memo xsi:type="xsd:string">Memo text</ns6:memo>              <ns6:department internalId="2" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:class internalId="2" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>          </record>      </add>  </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3701214}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="269" externalId="WOCl-JS-001-TEST" type="workOrderClose" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

### Related Topics

-   [Work Order Completion](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3701691.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

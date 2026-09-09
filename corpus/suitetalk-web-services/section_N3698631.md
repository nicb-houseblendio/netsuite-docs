---
id: "section_N3698631"
type: "section"
title: "Work Order Issue"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Work Order Issue"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3698631.html"
anchors: ["bridgehead_N3698689", "bridgehead_N3698939", "bridgehead_N3698976", "bridgehead_N3698988", "bridgehead_N3699031", "bridgehead_N3699067", "bridgehead_N3699091", "bridgehead_N3699113", "bridgehead_N3699125", "bridgehead_N28543961", "bridgehead_N28544021", "bridgehead_N28544081", "bridgehead_N28544141", "bridgehead_N3699184", "bridgehead_N3699195", "bridgehead_N3699207", "bridgehead_N3699219", "bridgehead_N3699229"]
sha256: "18dc1e0e239860ae25af7502aae749dabeda583a8af7c2b53c0dcad5da776489"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Work Order Issue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_29213414016.html).

If the Manufacturing Work In Process (WIP) feature has been enabled, you can use SOAP web services to interact with work order issue records. You can verify whether WIP is enabled by going to Setup > Company > Enable Features, and reviewing the Items & Inventory subtab.

With WIP, instead of creating a single assembly build record to denote that a work order has been addressed, you track progress of the work using three records: work order issue, work order completion, and work order close. This approach lets you manage the assembly process in a more granular way, and to keep the General Ledger up to date as materials move through the different phases of assembly. For more on the benefits of WIP, refer to [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html).

The work order issue record is used to indicate that particular quantities of raw materials, or component items, have been gathered for the production of the assembly item (or items).

In the UI, you can view the form used for creating the work order issue record by choosing _Transactions > Manufacturing > Issue Components_, selecting a Subsidiary (for OneWorld accounts), then clicking the Issue link that corresponds with one of listed work orders. An alternate method is to view the work order and click the Issue Components button. For help filling out the form manually, refer to [Entering Work Order Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html).

The work order issue record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

## Supported Operations {#bridgehead_N3698689}

The following operations can be used with work order issue records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3698939}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [work order issue](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/workorderissue.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3698976}

Refer to the following sections for more details on interacting with work order issue records.

## Prerequisites for Creating a Record {#bridgehead_N3698988}

Before you can create a work order issue record, a work order record must already exist, and the work order must be configured to use WIP (the WIP box on the work order record must be selected). This is true regardless of whether you are creating the work order issue record using initialize and add, or add by itself. If you try to create a work order issue record referencing a work order that has _not_ been configured to use WIP, the system generates an error reading in part, 'One of the following problems exists: You have an invalid work order < _work order ID_ >, the work order does not use WIP, or the work order is already closed.'

You can create and modify work orders by choosing _Transactions > Manufacturing > Enter Work Orders_. You can also interact with work orders using SOAP web services, as described in [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html).

Note also that the assembly item referenced in the work order must be properly set up for WIP. as described in the [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html).

## Using Initialize Versus Add {#bridgehead_N3699031}

You can initialize a work order issue record from a [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html) record. This is the preferred approach, though you can also create the record using the add operation by itself.

The initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

If you are using the add operation by itself, note that you must use the createdFrom field to identify the appropriate work order. If you fail to set a value for this field, the system generates an error reading, 'Transaction can only be created from a work order.'

## Working with the ComponentList Sublist {#bridgehead_N3699067}

The work order issue record includes the componentList sublist, which identifies the component items required by the work order.

When working with the work order issue record, most of the data in the componentList sublist is static - except for quantity. That is, you can update the individual quantities of each of the items listed, but you cannot add or remove items from the list.

In regard to quantity adjustments, note that, for each item, there is a maximum quantity. This maximum is determined by both the assembly item record and the work order record. For example, suppose you have an assembly item record for a widget that calls for 10 nails. If you create a work order calling for six builds of the widget, a total of 60 nails will be needed. Therefore, when you create the work order issue record, you can update the quantity of nails up to a maximum of 60.

Related to this, note that the maximum is cumulative. This rule is significant if you create multiple work order issue records for the same work order, or if you have also created work order completions with backflush (another record that lets you specify that certain quantities of component items have been used). To follow on with the previous example, suppose you create one work order issue record that records the use of 10 nails, and one work order completion with backflush that records the use of 20 nails. An additional work order issue record could denote the use of only 30 nails.

## Using ReplaceAll {#bridgehead_N3699091}

When you set replaceAll to true when working with the componentList sublist, you must specify a value for each record in the sublist. If you fail to reference each record, the system generates an error.

## Sample Code {#bridgehead_N3699113}

The following code illustrates how to add a work order issue record using a few different techniques.

## Using Both Initialize and Add {#bridgehead_N3699125}

This example shows how to create a work order issue record using both the initialize and add operations, which is the preferred approach. Note that this technique results in two sets of SOAP requests and responses.

Although the sample below does not change the quantities of items on the componentList sublist, it would be possible to do so by using set commands between the initialize and add statements.

## Java {#bridgehead_N28543961}

          `InitializeRef initRef = new InitializeRef(); initRef.setType(InitializeRefType.workOrder); initRef.setInternalId("167");   WorkOrderIssue woRecord = (WorkOrderIssue) c.initialize(initRef,InitializeType.workOrderIssue,null);   c.addRecord(woRecord);` 
        

## SOAP Request (Initialize) {#bridgehead_N28544021}

          `<soapenv:Body>       <initialize xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <initializeRecord>              <ns7:type xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">workOrderIssue</ns7:type>              <ns8:reference internalId="167" type="workOrder" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>          </initializeRecord>      </initialize>  </soapenv:Body>` 
        

## SOAP Response (Initialize) {#bridgehead_N28544081}

          `<soapenv:Body>     <initializeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">        <readResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <record xsi:type="tranInvt:WorkOrderIssue" xmlns:tranInvt="urn:inventory_2017_1.transactions.webservices.netsuite.com">             <tranInvt:createdDate>2013-03-07T07:10:00.000-08:00</tranInvt:createdDate>             <tranInvt:lastModifiedDate>2013-03-07T07:43:00.000-08:00</tranInvt:lastModifiedDate>             <tranInvt:tranId>3</tranInvt:tranId>               <tranInvt:item internalId="247" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>JS Assembly Item Y</platformCore:name>             </tranInvt:item>             <tranInvt:createdFrom internalId="167" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Work Order #1</platformCore:name>             </tranInvt:createdFrom>             <tranInvt:tranDate>2013-03-07T00:00:00.000-08:00</tranInvt:tranDate>             <tranInvt:postingPeriod internalId="141" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Mar 2013</platformCore:name>             </tranInvt:postingPeriod>             <tranInvt:subsidiary internalId="3" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>SUB  UK</platformCore:name>             </tranInvt:subsidiary>             <tranInvt:location internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Location UK</platformCore:name>             </tranInvt:location>             <tranInvt:componentList>                <tranInvt:workOrderIssueComponent>                   <tranInvt:item internalId="245" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <tranInvt:quantity>23.0</tranInvt:quantity>                    <tranInvt:lineNumber>5</tranInvt:lineNumber>                </tranInvt:workOrderIssueComponent>                   <tranInvt:workOrderIssueComponent>                   <tranInvt:item internalId="246" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <tranInvt:quantity>27.0</tranInvt:quantity>                   <tranInvt:lineNumber>6</tranInvt:lineNumber>                </tranInvt:workOrderIssueComponent>             </tranInvt:componentList>             <tranInvt:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:customField internalId="65" scriptId="custbody_633637_bsubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="34" scriptId="custbody_633637_bload" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="215" scriptId="custbody_633637_asubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>             </tranInvt:customFieldList>          </record>       </readResponse>    </initializeResponse> </soapenv:Body>` 
        

## SOAP Request (Add) {#bridgehead_N28544141}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record xsi:type="ns7:WorkOrderIssue" xmlns:ns7="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns7:createdDate xsi:type="xsd:dateTime">2013-03-07T15:10:00.000Z</ns7:createdDate>              <ns7:lastModifiedDate xsi:type="xsd:dateTime">2013-03-07T15:43:00.000Z</ns7:lastModifiedDate>              <ns7:tranId xsi:type="xsd:string">3</ns7:tranId>              <ns7:item internalId="247" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns8:name xsi:type="xsd:string">JS Assembly Item Y</ns8:name>              </ns7:item>              <ns7:createdFrom internalId="167" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns9:name xsi:type="xsd:string">Work Order #1</ns9:name>              </ns7:createdFrom>              <ns7:tranDate xsi:type="xsd:dateTime">2013-03-07T08:00:00.000Z</ns7:tranDate>              <ns7:postingPeriod internalId="141" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns10:name xsi:type="xsd:string">Mar 2013</ns10:name>              </ns7:postingPeriod>              <ns7:subsidiary internalId="3" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns11:name xsi:type="xsd:string">SUB  UK</ns11:name>              </ns7:subsidiary>              <ns7:location internalId="2" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns12:name xsi:type="xsd:string">Location UK</ns12:name>              </ns7:location>              <ns7:componentList replaceAll="false" xsi:type="ns7:WorkOrderIssueComponentList">               <ns7:workOrderIssueComponent xsi:type="ns7:WorkOrderIssueComponent">                   <ns7:item internalId="245" xsi:type="ns13:RecordRef" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <ns7:quantity xsi:type="xsd:double">23.0</ns7:quantity>                   <ns7:lineNumber xsi:type="xsd:long">5</ns7:lineNumber>               </ns7:workOrderIssueComponent>               <ns7:workOrderIssueComponent xsi:type="ns7:WorkOrderIssueComponent">                   <ns7:item internalId="246" xsi:type="ns14:RecordRef" xmlns:ns14="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <ns7:quantity xsi:type="xsd:double">27.0</ns7:quantity>                   <ns7:lineNumber xsi:type="xsd:long">6</ns7:lineNumber>               </ns7:workOrderIssueComponent>              </ns7:componentList>              <ns7:customFieldList xsi:type="ns15:CustomFieldList" xmlns:ns15="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns15:customField internalId="65" scriptId="custbody_633637_bsubmit" xsi:type="ns15:BooleanCustomFieldRef">                      <ns15:value xsi:type="xsd:boolean">false</ns15:value>                  </ns15:customField>                  <ns15:customField internalId="215" scriptId="custbody_633637_bload" xsi:type="ns15:BooleanCustomFieldRef">                      <ns15:value xsi:type="xsd:boolean">false</ns15:value>                  </ns15:customField>                  <ns15:customField internalId="23" scriptId="custbody_633637_asubmit" xsi:type="ns15:BooleanCustomFieldRef">                <ns15:value xsi:type="xsd:boolean">false</ns15:value>                  </ns15:customField>              </ns7:customFieldList>          </record>      </add>  </soapenv:Body>` 
        

## SOAP Response (Add) {#bridgehead_N3699184}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>       <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="174" type="workOrderIssue" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

## Using Add {#bridgehead_N3699195}

This example uses the add operation to create the work order issue record. This example also sets values for the quantities of items in the componentList sublist.

## Java {#bridgehead_N3699207}

          `RecordRef createdFromRef = new RecordRef(); createdFromRef.setInternalId("167");   RecordRef postingPeriodRef = new RecordRef(); postingPeriodRef.setInternalId("141");   RecordRef departmentRef = new RecordRef(); departmentRef.setInternalId("2");   RecordRef classRef = new RecordRef(); classRef.setInternalId("2");   RecordRef locationRef = new RecordRef(); locationRef.setInternalId("2");   RecordRef item1Ref = new RecordRef(); item1Ref.setInternalId("245");   RecordRef item2Ref = new RecordRef(); item2Ref.setInternalId("246");   WorkOrderIssue newWOI = new WorkOrderIssue(); newWOI.setExternalId("WOI-JS-002-TEST"); newWOI.setCreatedFrom(createdFromRef); newWOI.setPostingPeriod(postingPeriodRef); newWOI.setDepartment(departmentRef); newWOI.set_class(classRef); newWOI.setLocation(locationRef); newWOI.setMemo("Memo text");   WorkOrderIssueComponent[] componentListArray = { new WorkOrderIssueComponent(), new WorkOrderIssueComponent() }; componentListArray[0].setItem(item1Ref); componentListArray[0].setQuantity(2.0); componentListArray[1].setItem(item2Ref); componentListArray[1].setQuantity(3.0);   WorkOrderIssueComponentList componentList = new WorkOrderIssueComponentList(); componentList.setWorkOrderIssueComponent(componentListArray); componentList.setReplaceAll(false); newWOI.setComponentList(componentList);   c.addRecord(newWOI);` 
        

## SOAP Request {#bridgehead_N3699219}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record externalId="WOI-JS-002-TEST" xsi:type="ns6:WorkOrderIssue" xmlns:ns6="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns6:createdFrom internalId="167" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:postingPeriod internalId="141" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:memo xsi:type="xsd:string">Memo text</ns6:memo>              <ns6:department internalId="2" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:class internalId="2" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:location internalId="2" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:componentList replaceAll="false" xsi:type="ns6:WorkOrderIssueComponentList">                  <ns6:workOrderIssueComponent xsi:type="ns6:WorkOrderIssueComponent">                      <ns6:item internalId="245" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">2.0</ns6:quantity>                  </ns6:workOrderIssueComponent>                  <ns6:workOrderIssueComponent xsi:type="ns6:WorkOrderIssueComponent">                      <ns6:item internalId="246" xsi:type="ns13:RecordRef" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                  </ns6:workOrderIssueComponent>              </ns6:componentList>          </record>      </add>  </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3699229}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>           <baseRef internalId="171" externalId="WOI-JS-002-TEST" type="workOrderIssue" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

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

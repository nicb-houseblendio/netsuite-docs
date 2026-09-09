---
id: "section_N3701691"
type: "section"
title: "Work Order Completion"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Work Order Completion"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3701691.html"
anchors: ["bridgehead_N3701747", "bridgehead_N3702009", "bridgehead_N3702047", "bridgehead_N3702059", "bridgehead_N3702105", "procedure_N3702127", "bridgehead_N3702181", "bridgehead_N3702193", "bridgehead_N3702213", "bridgehead_N3702253", "bridgehead_N3702265", "bridgehead_N28571081", "bridgehead_N28571141", "bridgehead_N28571201", "bridgehead_N28571261", "bridgehead_N3702345", "bridgehead_N3702356", "bridgehead_N28571601", "bridgehead_N28571661", "bridgehead_N3702403"]
sha256: "ee2120fdd3e8a3e5584a418f28e64ad2eb8b20b615d9c57c734f000496b2be3d"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Work Order Completion](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_94213635853.html).

If the Manufacturing Work In Process (WIP) feature has been enabled, you can use SOAP web services to interact with work order completion records. You can verify whether WIP is enabled by going to _Setup > Company > Enable Features_, and reviewing the Items & Inventory subtab.

With WIP, instead of creating a single assembly build record to denote that a work order has been addressed, you track progress of the work using three records: work order issue, work order completion, and work order close. This approach lets you manage the assembly process in a more granular way, and to keep the General Ledger up to date as materials move through the different phases of assembly. For more on the benefits of WIP, refer to [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html).

The work order completion record is used to indicate that assemblies have been built. You can also optionally use this record to record that raw materials - items in the componentList sublist - have been consumed as part of the assembly process. This latter option is called entering a completion with backflush. For example, you might enter a completion with backflush if previous records (such as work order issue) did not record the consumption of all the materials you ended up using.

In the UI, you can view the form used for creating the work order completion record by choosing _Transactions > Manufacturing > Enter Completions_, selecting a Subsidiary (for OneWorld accounts), then clicking the Complete link that corresponds with one of the listed work orders. An alternate method is to view the work order and click one of two buttons: Enter Completions or Enter Completions With Backflush. For help filling out the form manually, refer to [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html).

The work order completion record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

## Supported Operations {#bridgehead_N3701747}

The following operations can be used with work order completion records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3702009}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [work order completion](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/workordercompletion.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3702047}

Refer to the following sections for more details on interacting with work order completion records.

## Prerequisites for Creating a Record {#bridgehead_N3702059}

Before you can create a work order completion record, a work order record must already exist, and the work order must be configured to use WIP (the WIP box on the work order record must be selected). This is true regardless of whether you are creating the work order issue record using initialize and add, or add by itself. If you try to create a work order issue record referencing a work order that has _not_ been configured to use WIP, the system generates an error reading in part, 'One of the following problems exists: You have an invalid work order < _work order ID_ >, the work order does not use WIP, or the work order is already closed.'

You can create work orders by choosing _Transactions > Manufacturing > Enter Work Orders_. You can also interact with work orders using SOAP web services, as described in [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html).

Further, the assembly item referenced in the work order must be properly set up for WIP. For details on this process, see [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html).

Note that it does not matter if a work order issue record already exists for your work order. You can go straight from entering the work order to creating the work order completion record.

## Using Initialize Versus Add {#bridgehead_N3702105}

You can initialize a work order completion record from a [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html) record. This is the preferred approach, though you can also create the record using the add operation by itself.

## Using Both Initialize and Add {#procedure_N3702127}

The initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

Note that when you use the initialize operation, certain required fields are not initialized and must be set manually. These fields vary depending on the work order that you are using, as follows:

-   If the work order uses routing, the startOperation and endOperation fields are both required (but are not initialized). These fields denote which operation tasks were completed.
    
-   If the work order does not use routing, the quantity field is required (but is not initialized). The quantity element denotes the total number of assembly items that were completed in the build process. Note that you cannot update this field to a value greater than the value called for in the work order. Attempting to set the value too high results in an error.
    

In each case, you must manually set the required values in a statement between the initialize and add statements. To see an example, refer to [Using Initialize and Setting isBackflush to False](#bridgehead_N3702265).

## Using Add {#bridgehead_N3702181}

If you are using the add operation by itself, note that you must use the createdFrom field to identify the appropriate work order. If you fail to set a value for this field, the system generates an error reading, 'Transaction can only be created from a work order.'

## Working with the OperationList Sublist {#bridgehead_N3702193}

When routing is used, an additional sublist, operationList, is available. If the original work order does not use routing, the operationList sublist is unavailable.

## Working with the ComponentList Sublist {#bridgehead_N3702213}

When working with the componentList sublist, note that the same general restrictions apply as when you are using the work order issue record. For details, see [Working with the ComponentList Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3698631.html#bridgehead_N3699067).

In addition, note that, with work order completion, you can interact with the componentList sublist _only_ if the isBackflush element is set to true.

Refer also to [Using ReplaceAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3698631.html#bridgehead_N3699091) for details on the validation that occurs when replaceAll is set to true.

## Sample Code {#bridgehead_N3702253}

The following code illustrates how to create a work order completion record using a few different techniques.

## Using Initialize and Setting isBackflush to False {#bridgehead_N3702265}

The preferred strategy of creating a work order completion record is to use the initialize operation. Note that this approach generates two sets of SOAP requests and responses - one for the initialize operation and one for the add operation. This example shows how to use initialize to create a work order completion with isBackflush set to false.

Note that isBackflush is set to false by default. To include quantity values for items on the componentList, you would have to set isBackflush to true and specify the quantity values for the component items. (To see an example that sets isBackflush to true, see [Using Add and Setting isBackflush to True](#bridgehead_N3702356).)

Further, note that in this example, the work order being referenced does not use routing. For this reason, the quantity value is required - and because the value is not initialized, it must be manually set. You should set the quantity value between the initialize and add statements.

## Java {#bridgehead_N28571081}

          `InitializeRef initRef = new InitializeRef(); initRef.setType(InitializeRefType.workOrder); initRef.setInternalId("167");   WorkOrderCompletion woRecord = (WorkOrderCompletion) c.initialize(initRef,InitializeType.workOrderCompletion,null);   woRecord.setQuantity(3.0);   c.addRecord(woRecord);` 
        

## SOAP Request (Initialize) {#bridgehead_N28571141}

          `<soapenv:Body>      <initialize xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <initializeRecord>              <ns7:type xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">workOrderCompletion</ns7:type>              <ns8:reference internalId="167" type="workOrder" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>          </initializeRecord>      </initialize>  </soapenv:Body>` 
        

## SOAP Response (Initialize) {#bridgehead_N28571201}

          `<soapenv:Body>    <initializeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <readResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <record xsi:type="tranInvt:WorkOrderCompletion" xmlns:tranInvt="urn:inventory_2017_1.transactions.webservices.netsuite.com">             <tranInvt:createdDate>2013-03-07T07:10:00.000-08:00</tranInvt:createdDate>             <tranInvt:lastModifiedDate>2013-03-07T08:14:00.000-08:00</tranInvt:lastModifiedDate>             <tranInvt:tranId>2</tranInvt:tranId>             <tranInvt:item internalId="247" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>JS Assembly Item Y</platformCore:name>             </tranInvt:item>             <tranInvt:isBackflush>false</tranInvt:isBackflush>             <tranInvt:orderQuantity>5.0</tranInvt:orderQuantity>             <tranInvt:createdFrom internalId="167" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Work Order #1</platformCore:name>             </tranInvt:createdFrom>             <tranInvt:tranDate>2013-03-07T00:00:00.000-08:00</tranInvt:tranDate>             <tranInvt:postingPeriod internalId="141" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Mar 2013</platformCore:name>             </tranInvt:postingPeriod>             <tranInvt:subsidiary internalId="3" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>SUB  UK</platformCore:name>             </tranInvt:subsidiary>             <tranInvt:location internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:name>Location UK</platformCore:name>       </tranInvt:location>             <tranInvt:componentList>                <tranInvt:workOrderCompletionComponent>                   <tranInvt:item internalId="245" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <tranInvt:quantityPer>5.0</tranInvt:quantityPer>                   <tranInvt:lineNumber>5</tranInvt:lineNumber>                </tranInvt:workOrderCompletionComponent>                   <tranInvt:workOrderCompletionComponent>                   <tranInvt:item internalId="246" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <tranInvt:quantityPer>6.0</tranInvt:quantityPer>                   <tranInvt:lineNumber>6</tranInvt:lineNumber>                </tranInvt:workOrderCompletionComponent>             </tranInvt:componentList>             <tranInvt:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:customField internalId="65" scriptId="custbody_633637_bsubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="215" scriptId="custbody_633637_bload" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>                <platformCore:customField internalId="53" scriptId="custbody_633637_asubmit" xsi:type="platformCore:BooleanCustomFieldRef">                   <platformCore:value>false</platformCore:value>                </platformCore:customField>             </tranInvt:customFieldList>          </record>       </readResponse>    </initializeResponse> </soapenv:Body>` 
        

## SOAP Request (Add) {#bridgehead_N28571261}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record xsi:type="ns7:WorkOrderCompletion" xmlns:ns7="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns7:createdDate xsi:type="xsd:dateTime">2013-03-07T15:10:00.000Z</ns7:createdDate>              <ns7:lastModifiedDate xsi:type="xsd:dateTime">2013-03-07T16:14:00.000Z</ns7:lastModifiedDate>              <ns7:tranId xsi:type="xsd:string">2</ns7:tranId>              <ns7:item internalId="247" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns8:name xsi:type="xsd:string">JS Assembly Item Y</ns8:name>              </ns7:item>              <ns7:quantity xsi:type="xsd:double">3.0</ns7:quantity>              <ns7:isBackflush xsi:type="xsd:boolean">false</ns7:isBackflush>              <ns7:orderQuantity xsi:type="xsd:double">5.0</ns7:orderQuantity>              <ns7:createdFrom internalId="167" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns9:name xsi:type="xsd:string">Work Order #1</ns9:name>              </ns7:createdFrom>              <ns7:tranDate xsi:type="xsd:dateTime">2013-03-07T08:00:00.000Z</ns7:tranDate>              <ns7:postingPeriod internalId="141" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns10:name xsi:type="xsd:string">Mar 2013</ns10:name>              </ns7:postingPeriod>              <ns7:subsidiary internalId="3" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns11:name xsi:type="xsd:string">SUB  UK</ns11:name>              </ns7:subsidiary>              <ns7:location internalId="2" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns12:name xsi:type="xsd:string">Location UK</ns12:name>              </ns7:location>              <ns7:componentList replaceAll="false" xsi:type="ns7:WorkOrderCompletionComponentList">               <ns7:workOrderCompletionComponent xsi:type="ns7:WorkOrderCompletionComponent">                <ns7:item internalId="245" xsi:type="ns13:RecordRef" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns7:quantityPer xsi:type="xsd:double">5.0</ns7:quantityPer>                <ns7:lineNumber xsi:type="xsd:long">5</ns7:lineNumber>               </ns7:workOrderCompletionComponent>               <ns7:workOrderCompletionComponent xsi:type="ns7:WorkOrderCompletionComponent">                <ns7:item internalId="246" xsi:type="ns14:RecordRef" xmlns:ns14="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns7:quantityPer xsi:type="xsd:double">6.0</ns7:quantityPer>                <ns7:lineNumber xsi:type="xsd:long">6</ns7:lineNumber>               </ns7:workOrderCompletionComponent>              </ns7:componentList>              <ns7:customFieldList xsi:type="ns15:CustomFieldList" xmlns:ns15="urn:core_2017_1.platform.webservices.netsuite.com">                  <ns15:customField internalId="65" scriptId="custbody_633637_bsubmit" xsi:type="ns15:BooleanCustomFieldRef">                      <ns15:value xsi:type="xsd:boolean">false</ns15:value>                  </ns15:customField>               <ns15:customField internalId="215" scriptId="custbody_633637_bload" xsi:type="ns15:BooleanCustomFieldRef">                      <ns15:value xsi:type="xsd:boolean">false</ns15:value>                     </ns15:customField>                  <ns15:customField internalId="53" scriptId="custbody_633637_asubmit" xsi:type="ns15:BooleanCustomFieldRef">                      <ns15:value xsi:type="xsd:boolean">false</ns15:value>                  </ns15:customField>              </ns7:customFieldList>          </record>      </add>  </soapenv:Body>` 
        

## SOAP Response (Add) {#bridgehead_N3702345}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="268" type="workOrderCompletion" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

## Using Add and Setting isBackflush to True {#bridgehead_N3702356}

The following example omits the initialize operation - using only the add operation to create the record. In this example, isBackflush is set to true and values are sent for the quantities of items in the componentList sublist.

Note that this example sets a value for the quantity body field. However, if the original work order used a routing, the quantity field would not be updatable.

## Java {#bridgehead_N28571601}

          `RecordRef createdFromRef = new RecordRef(); createdFromRef.setInternalId("167");   RecordRef postingPeriodRef = new RecordRef(); postingPeriodRef.setInternalId("141");   RecordRef departmentRef = new RecordRef(); departmentRef.setInternalId("2");   RecordRef classRef = new RecordRef(); classRef.setInternalId("2");   RecordRef item1Ref = new RecordRef(); item1Ref.setInternalId("245");   RecordRef item2Ref = new RecordRef(); item2Ref.setInternalId("246");   WorkOrderCompletion newWOCo = new WorkOrderCompletion(); newWOCo.setExternalId("WOCo-JS-001-TEST-BFT"); newWOCo.setCreatedFrom(createdFromRef); newWOCo.setQuantity(2.0); newWOCo.setIsBackflush(true); newWOCo.setPostingPeriod(postingPeriodRef); newWOCo.setDepartment(departmentRef); newWOCo.set_class(classRef); newWOCo.setMemo("Add - isBackFlush = T");   WorkOrderCompletionComponent[] componentListArray = { new WorkOrderCompletionComponent(), new WorkOrderCompletionComponent() }; componentListArray[0].setItem(item1Ref); componentListArray[0].setQuantity(3.0); componentListArray[1].setItem(item2Ref); componentListArray[1].setQuantity(4.0);   WorkOrderCompletionComponentList componentList = new WorkOrderCompletionComponentList(); componentList.setWorkOrderCompletionComponent(componentListArray); newWOCo.setComponentList(componentList);   c.addRecord(newWOCo);` 
        

## SOAP Request {#bridgehead_N28571661}

          `<soapenv:Body>      <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record externalId="WOCo-JS-001-TEST-BFT" xsi:type="ns6:WorkOrderCompletion" xmlns:ns6="urn:inventory_2017_1.transactions.webservices.netsuite.com">              <ns6:quantity xsi:type="xsd:double">2.0</ns6:quantity>              <ns6:isBackflush xsi:type="xsd:boolean">true</ns6:isBackflush>              <ns6:createdFrom internalId="167" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:postingPeriod internalId="141" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:memo xsi:type="xsd:string">Add - isBackFlush = T</ns6:memo>              <ns6:department internalId="2" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:class internalId="2" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>              <ns6:componentList replaceAll="false" xsi:type="ns6:WorkOrderCompletionComponentList">                  <ns6:workOrderCompletionComponent xsi:type="ns6:WorkOrderCompletionComponent">                      <ns6:item internalId="245" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                  </ns6:workOrderCompletionComponent>                  <ns6:workOrderCompletionComponent xsi:type="ns6:WorkOrderCompletionComponent">                      <ns6:item internalId="246" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">4.0</ns6:quantity>                  </ns6:workOrderCompletionComponent>              </ns6:componentList>          </record>      </add>  </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3702403}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="267" externalId="WOCo-JS-001-TEST-BFT" type="workOrderCompletion" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

### Related Topics

-   [Work Order Issue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3698631.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3486552"
type: "section"
title: "deleteList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > deleteList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html"
anchors: ["bridgehead_N3486589", "subsect_91133720763", "bridgehead_4485491885", "bridgehead_N3486706", "bridgehead_N3488284", "bridgehead_N3488360", "bridgehead_4484708953", "bridgehead_3705191452", "bridgehead_3705191694"]
sha256: "514c1877974c33a9ccbb86f2fefb9079a16223081e92716b5b2a358d782402bb"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The deleteList operations is used to delete one or more record instances. The record instances can be of various record types. For example, it is possible to delete a customer and a contact within a single request by using this operation.

Note:

An asynchronous equivalent is available for this operation, **asyncDeleteList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Request {#bridgehead_N3486589}

The DeleteListRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record\[\] | RecordRef | An array of recordRef objects that specify the records to be deleted. |
| deletionReason | DeletionReason | Identifies a deletion reason and deletion reason memo. This parameter supports the Use Deletion Reasons feature, which requires users to provide reasons when they delete transactions. However, even when this feature is not enabled, you must use this parameter with every deleteList request. (You can provide a value of `null` in such cases.) For more details, see [Deletion Reason Usage Notes](#bridgehead_4485491885). |

## Usage Notes {#subsect_91133720763}

If the deleteList request contains malformed syntax and the request cannot be completed, the No data was found error message is returned.

## Deletion Reason Usage Notes {#bridgehead_4485491885}

Note the following about the deletionReason parameter:

-   A single deletion reason applies to the entire array of records being deleted. If some of the records are transactions and some are not, then the deletion reason still applies to the transactions. It is ignored for the other records.
    
-   The deletionReason complex type includes two fields: deletionReasonCode and deletionReasonMemo. The deletionReasonCode must identify a deletion reason that is listed at _Setup > Accounting > Accounting Lists_. If the Use Deletion Reasons feature is enabled and you use the deletionReasonCode to identify a code that does not exist, the request fails with an `INVALID_REF_KEY` error.
    
-   Deletion reasons can be saved only for transactions. However, in SOAP web services, you must use the deletionReason parameter even when referencing other record types, and even when the Use Deletion Reasons feature is not enabled. For situations where it is not appropriate to identify a deletion reason, pass in a value of `null`.
    
-   Even when when a deletion reason is required, you can use a value of `null`. In these cases, the system automatically populates the deletion reason fields with default values. These defaults are: `Other` for deletionReasonCode and `This transaction was deleted by script or web service` for deletionReasonMemo.
    
-   The deletionReason complex type is defined in the [core XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd).
    

For more details about the Use Deletion Reasons feature, see [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html).

## Response {#bridgehead_N3486706}

The DeleteListResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response\[\] | WriteResponse | Contains an array of WriteResponse objects, each of which contains details on the status of the delete operation and a reference to the deleted record. |

## Faults {#bridgehead_N3488284}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3488360}

The following examples show various ways of using the deleteList operation.

## C# {#bridgehead_4484708953}

The following example shows how to delete two cash sale transactions. Both transactions have the same deletion reason.

          `private void deleteCashSales() {    RecordRef myCashSale = new RecordRef();    myCashSale.internalId = "1727";    myCashSale.type = RecordType.cashSale;    myCashSale.typeSpecified = true;     RecordRef myCashSale2 = new RecordRef();    myCashSale2.internalId = "1728";    myCashSale2.type = RecordType.cashSale;    myCashSale2.typeSpecified = true;     RecordRef myDeletionReasonCode = new RecordRef();    myDeletionReasonCode.internalId = "2";     DeletionReason myDeletionReason = new DeletionReason();    myDeletionReason.deletionReasonCode = myDeletionReasonCode;    myDeletionReason.deletionReasonMemo = "Per Scott";            RecordRef[] myCashSaleRefs = new RecordRef[2];    myCashSaleRefs[0] = myCashSale;    myCashSaleRefs[1] = myCashSale2;     _service.deleteList(myCashSaleRefs, myDeletionReason);  }` 
        

The following example shows how to delete two records of different types: an employee record and a calender event record. Because it's not possible to set a deletion reason for either of those two types of records, the deletion reason used is null.

          `private void deleteVariousRecords() {    RecordRef myEmployee = new RecordRef();    myEmployee.internalId = "360";    myEmployee.type = RecordType.employee;    myEmployee.typeSpecified = true;     RecordRef myCalendarEvent = new RecordRef();    myCalendarEvent.internalId = "381";    myCalendarEvent.type = RecordType.calendarEvent;    myCalendarEvent.typeSpecified = true;     RecordRef[] myRecords = new RecordRef[2];    myRecords[0] = myEmployee;    myRecords[1] = myCalendarEvent;     _service.deleteList(myRecords, null);  }` 
        

## SOAP Request {#bridgehead_3705191452}

The following SOAP request shows how to delete an employee and calendar event record.

          `<soap:Body>    <deleteList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <baseRef type="employee" internalId="360" xsi:type="q1:RecordRef" xmlns:q1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef type="calendarEvent" internalId="381" xsi:type="q2:RecordRef" xmlns:q2="urn:core_2017_1.platform.webservices.netsuite.com"/>    </deleteList> </soap:Body>` 
        

## SOAP Response {#bridgehead_3705191694}

In the response, the status for each item in the request is returned. If a problem exists with one of the items, creating an error, the other records are still processed.

          `<soapenv:Body>    <deleteListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponseList>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef xsi:type="platformCore:RecordRef" type="employee" internalId="360" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef xsi:type="platformCore:RecordRef" type="calendarEvent" internalId="381" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>       </writeResponseList>    </deleteListResponse> </soapenv:Body>` 
        

### Related Topics

-   [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html)
-   [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

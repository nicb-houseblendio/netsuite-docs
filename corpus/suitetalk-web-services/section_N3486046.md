---
id: "section_N3486046"
type: "section"
title: "delete"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > delete"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html"
anchors: ["bridgehead_N3486058", "bridgehead_4485470467", "bridgehead_N3486174", "bridgehead_N3486289", "bridgehead_N3486372", "bridgehead_4484640141", "bridgehead_3705190086", "bridgehead_3705190306"]
sha256: "a91083a607b9f1efac4b8d69817dc6b3d107e00bc458866a13044ba3c69e78b8"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The delete operation is used to delete an instance of a record. It is similar to the deleteList operation, except that it permits only one record to be deleted per request.

## Request {#bridgehead_N3486058}

The DeleteRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| recordRef | RecordRef | Indentifies the record to be deleted. |
| deletionReason | DeletionReason | Identifies a deletion reason and deletion reason memo. This parameter supports the Use Deletion Reasons feature, which requires users to provide reasons when they delete transactions. However, even when this feature is not enabled, you must use this parameter with every delete request. (You can provide a value of `null` in such cases.) For more details, see [Deletion Reason Usage Notes](#bridgehead_4485470467). |

## Deletion Reason Usage Notes {#bridgehead_4485470467}

Note the following about the deletionReason parameter:

-   The deletionReason complex type includes two fields: deletionReasonCode and deletionReasonMemo. The deletionReasonCode must identify a deletion reason that is listed at _Setup > Accounting > Accounting Lists_. If the Use Deletion Reasons feature is enabled and you use the deletionReasonCode to identify a code that does not exist, the request fails with an `INVALID_REF_KEY` error.
    
-   Deletion reasons can be saved only for transactions. However, in SOAP web services, you must use the deletionReason parameter even when referencing other record types, and even when the Use Deletion Reasons feature is not enabled. For situations where it is not appropriate to identify a deletion reason, pass in a value of `null`.
    
-   Even when when a deletion reason is required, you can use a value of `null`. In these cases, the system automatically populates the deletion reason fields with default values. These defaults are: `Other` for deletionReasonCode and `This transaction was deleted by script or web service` for deletionReasonMemo.
    
-   The deletionReason complex type is defined in the [core XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd).
    

For more details about the Use Deletion Reasons feature, see [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html).

## Response {#bridgehead_N3486174}

The DeleteResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse | Contains details on the status of the delete operation and a reference to the deleted record. |

## Faults {#bridgehead_N3486289}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

Note:

If you attempt to delete a record that does not exist, the system returns an INVALID\_KEY\_OR\_REF error.

## Sample Code {#bridgehead_N3486372}

The following example shows how to delete a cash sale transaction.

## C# {#bridgehead_4484640141}

          `private void deleteCashSale() {    RecordRef myCashSale = new RecordRef();    myCashSale.internalId = "1745";    myCashSale.type = RecordType.cashSale;    myCashSale.typeSpecified = true;     RecordRef myDeletionReasonCode = new RecordRef();    myDeletionReasonCode.internalId = "3";     DeletionReason myDeletionReason = new DeletionReason();    myDeletionReason.deletionReasonCode = myDeletionReasonCode;    myDeletionReason.deletionReasonMemo = "Per John in Accounting";     _service.delete(myCashSale, myDeletionReason);  }` 
        

## SOAP Request {#bridgehead_3705190086}

          `<soap:Body>    <delete xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <baseRef type="cashSale" internalId="1745" xsi:type="q1:RecordRef" xmlns:q1="urn:core_2017_1.platform.webservices.netsuite.com"/>          <deletionReason>             <deletionReasonCode internalId="3" xmlns="urn:core_2017_1.platform.webservices.netsuite.com"/>             <deletionReasonMemo xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Per John in Accounting</deletionReasonMemo>          </deletionReason>    </delete> </soap:Body>` 
        

## SOAP Response {#bridgehead_3705190306}

          `<soapenv:Body>    <deleteResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef xsi:type="platformCore:RecordRef" type="cashSale" internalId="1745" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </deleteResponse> </soapenv:Body>` 
        

### Related Topics

-   [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html)
-   [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

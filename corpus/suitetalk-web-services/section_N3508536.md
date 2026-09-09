---
id: "section_N3508536"
type: "section"
title: "initialize / initializeList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > initialize / initializeList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html"
anchors: ["bridgehead_N3512044", "bridgehead_N3512063", "bridgehead_N3512214", "bridgehead_N3512365", "bridgehead_N3512441", "bridgehead_N27184821", "bridgehead_N27184881", "bridgehead_N27184941", "bridgehead_N27185001"]
sha256: "3f49d8139dfa70b077eee21bd5ea629d44b8b0bd074916d26eb6dbf665842a82"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Use the initialize operation to emulate the UI workflow by prepopulating fields on transaction line items with values from a related record. Your SOAP web services application can then modify only the values it needs to before submitting the record.

For example, in the UI clicking Bill from a Sales Order record loads an Invoice record where fields are populated with values from the Sales Order. When loading an invoice record in SOAP web services, you can reference the related Sales Order record to initialize fields with values from that sales order.

Note:

An asynchronous equivalent is available for the initializeList operation, **asyncInitializeList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

The following table lists all the transaction types that can be used with the initialize operation and the valid reference types they can use.

| (Target Record) Transaction Type | Initialize Reference | Notes |
| --- | --- | --- |
| Assembly Unbuild | Assembly Build |  |
| Cash Refund | Cash Sale |  |
| Cash Refund | Return Authorization |  |
| Cash Sale | Customer | Populates Billable tabs |
| Cash Sale | Estimate |  |
| Cash Sale | Opportunity |  |
| Cash Sale | Sales Order |  |
| Credit Memo | Customer |  |
| Credit Memo | Invoice |  |
| Credit Memo | Return Authorization |  |
| Customer Deposit | Sales Order |  |
| Customer Payment | Customer | Use the arAccount parameter to specify the accounts receivable (AR) account in a Customer to Customer Payment initialization. (This parameter is define in InitializeAuxRefType.) |
| Customer Payment | Invoice |  |
| Customer Refund | Credit Memo |  |
| Customer Refund | Customer |  |
| Deposit Application | Customer Deposit |  |
| Estimate | Opportunity |  |
| Invoice | Customer | Defaults billable time, expense, and items |
| Invoice | Estimate |  |
| Invoice | Opportunity |  |
| Invoice | Sales Order | Defaults the line items as well as billable time, expense, and items |
| Item Fulfillment | Intercompany Transfer Order |  |
| Item Fulfillment | Sales Order | Defaults the line items for fulfillment |
| Item Fulfillment | Transfer Order | The line field on a transfer order does not have to correspond to the orderLine field on a newly created item fulfillment. |
| Item Fulfillment | Vendor Return Authorization |  |
| Item Receipt | Intercompany Transfer Order |  |
| Item Receipt | Purchase Order | Initializing an item receipt from a **dropship** purchase order is not supported. The preferred workflow is to initialize an item fulfillment from the sales order that has the dropship item. The accounting impact will be the same and more desirable because inventory levels will not be affected. |
| Item Receipt | Return Authorization |  |
| Item Receipt | Transfer Order |  |
| Purchase Order | Requisition |  |
| Return Authorization | Cash Sale |  |
| Return Authorization | Invoice |  |
| Return Authorization | Sales Order |  |
| Sales Order | Estimate |  |
| Sales Order | Opportunity |  |
| Vendor Bill | Purchase Order | You can initialize or link a single purchase order to a vendor bill, or a list of purchase orders to a vendor bill. Note that when linking multiple purchase orders to a single vendor bill, all purchase orders must be for the same vendor. When you initialize a vendor bill from a purchase order, the purchase order gets transformed but any attached files are not transferred to the vendor bill. For more information, see [Linking Purchase Orders to a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3687718.html#bridgehead_N3688254). When you initialize a vendor bill, there are two possibilities for the value of the account field on the vendor bill.
-   If you have not populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the account most recently used on a vendor bill.
-   If you have populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the same field value.

 |
| Vendor Bill | Vendor | Use the apAccount parameter to specify the accounts payable (AP) account in a Vendor to Vendor Bill initialization. (This parameter is define in InitializeAuxRefType.) When you initialize a vendor bill, there are two possibilities for the value of the account field on the vendor bill.

-   If you have not populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the account most recently used on a vendor bill.
-   If you have populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the same field value.

 |
| Vendor Credit | Vendor |  |
| Vendor Credit | Vendor Bill |  |
| Vendor Credit | Vendor Return Authorization |  |
| Vendor Payment | Employee |  |
| Vendor Payment | Vendor |  |
| Vendor Payment | Vendor Bill |  |
| Vendor Return Authorization | Vendor |  |
| Vendor Return Authorization | Vendor Bill |  |
| Work Order Close | Work Order | The work order must be configured to use WIP. |
| Work Order Completion | Work Order | The work order must be configured to use WIP. |
| Work Order Issue | Work Order | The work order must be configured to use WIP. |

## Ignore Read-Only Preference {#bridgehead_N3512044}

To submit an initialized record without having to remove read-only fields populated during the initialization, set the Ignore Read-Only header preference to TRUE.

Important:

When this preference is set to TRUE, read-only fields are ignored during the SOAP web services request. The fields still cannot be set.

## Request {#bridgehead_N3512063}

The InitializeRequest type is used for this request. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| initializeRecord | InitializeRecord |  |

The InitializeRecord type takes the following fields:

-   type
    
-   reference
    
-   auxReference
    
-   referenceList
    

## Response {#bridgehead_N3512214}

The InitializeResponse type is used for the response. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| record | Record | The record type of the resulting initialization. |

## Faults {#bridgehead_N3512365}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3512441}

## SOAP Request (initialize) {#bridgehead_N27184821}

          `<soapenv:Body> <platformMsgs:initialize xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:platformCoreTyp="urn:types.core_2017_1.platform.webservices.netsuite.com" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com" xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">    <platformMsgs:initializeRecord>       <platformCore:type>invoice</platformCore:type>       <platformCore:reference internalId="1513" type="salesOrder">          <platformCore:name>1511</platformCore:name>       </platformCore:reference>    </platformMsgs:initializeRecord> </platformMsgs:initialize> </soapenv:Body>` 
        

## SOAP Request (initializeList) {#bridgehead_N27184881}

          `<initializeList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">   <initializeRecord>     <ns1:type        xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com">customerPayment     </ns1:type>     <ns2:reference internalId="176" type="customer"          xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>   </initializeRecord>      <initializeRecord>         <ns3:type xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">          invoice</ns3:type>             <ns4:reference internalId="176" type="customer"              xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com"/>       </initializeRecord>   </initializeList>` 
        

## Java (initializeList) {#bridgehead_N27184941}

          `InitializeRef iRef1 = new InitializeRef(); iRef1.setInternalId("176"); iRef1.setType(InitializeRefType.customer);   InitializeRecord ir1 = new InitializeRecord(); ir1.setReference(iRef1); ir1.setType(InitializeType.customerPayment);   InitializeRecord ir2 = new InitializeRecord(); ir2.setReference(iRef1); ir2.setType(InitializeType.invoice);   sessMgr.getPort().getNetSuitePortTypePort().initializeList(new InitializeRecord[]{ir1, ir2});` 
        

## C# (initialize) {#bridgehead_N27185001}

          `private void Initialize()         {             this.login(true);                        InitializeRef ref1 = new InitializeRef();             ref1.type = InitializeRefType.salesOrder;                  //internal id of the sales order to be converted to cash sale             ref1.internalId = "792";              ref1.typeSpecified = true;                         InitializeRecord rec = new InitializeRecord();             rec.type = InitializeType.cashSale;             rec.reference = ref1;                          ReadResponse read1 = _service.initialize(rec);                 }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

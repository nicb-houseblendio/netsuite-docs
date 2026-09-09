---
id: "section_N3481360"
type: "section"
title: "addList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > addList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html"
anchors: ["bridgehead_N3481468", "bridgehead_N3481583", "bridgehead_N3481699", "bridgehead_N3481774", "bridgehead_3705185066", "bridgehead_3705185383", "bridgehead_3705185634"]
sha256: "944515b788f5200a0912433f23b8e0530570bd1af9b252179f01dae532f419f7"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The addList operation is used to add one or more new instances of a record to NetSuite. If there are multiple records, they can either be of the same record type or different record types. For example, it's possible to add a customer and a contact within a single request using this operation. However, each record entered must have a unique signature. Adding two records with the same signature results in a SOAP fault. The signature consists of parameters required to identify a record as unique.

For example, in the case of entities, a record is uniquely identified by its name, its type and its parent hierarchy. So you could have two records with the same entityId (or name) belonging to two different record types as follows:

Customer (the type):

John Smith

MyCompany: John Smith

Contact

John Smith

But a second record such as the following would be invalid:

Contact

John Smith

Note:

An asynchronous equivalent is available for this operation, **asyncAddList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

Note that to prevent duplicate records, you should use the alternate [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) and [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html) operations when adding records to NetSuite.

## Request {#bridgehead_N3481468}

The AddListRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record\[\] | Record | Contains an array of record objects. The record type is an abstract type so an instance of a type that extends record must be used-such as Customer or Event. |

## Response {#bridgehead_N3481583}

The AddListResponse type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response\[\] | WriteResponse | Contains an array of WriteResponse objects, each of which contains details on the status of that add operation and a reference to that created record. |

## Faults {#bridgehead_N3481699}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3481774}

## SOAP Request {#bridgehead_3705185066}

In the following example, two customer records are added. When using the addList operation, you can submit two different record types in the same request.

          `<soap:Body> <platformMsgs:addList>         <platformMsgs:record xsi:type="listRel:Customer">                 <listRel:entityId>Shutter Fly</listRel:entityId>                 <listRel:companyName>Shutter Fly, Inc</listRel:companyName>                 <listRel:unsubscribe>false</listRel:unsubscribe>         </platformMsgs:record>         <platformMsgs:record xsi:type="listRel:Customer">                 <listRel:entityId>GNC</listRel:entityId>                 <listRel:companyName>GNC Corp</listRel:companyName>                 <listRel:unsubscribe>false</listRel:unsubscribe>         </platformMsgs:record> </platformMsgs:addList> </soap:Body>` 
        

## SOAP Response {#bridgehead_3705185383}

In the response, notice that the internal ID for each record added is returned.

          `<soapenv:Body> <addListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponseList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <writeResponse>       <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="980" type="customer" xsi:type="ns2:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse>    <writeResponse>       <ns3:status isSuccess="true" xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="981" type="customer" xsi:type="ns4:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse> </writeResponseList> </addListResponse> </soapenv:Body>` 
        

## Java Sample {#bridgehead_3705185634}

          `public void addListCustomer() throws RemoteException {                 this.login(true);                                  Customer cust1 = new Customer();                 cust1.setEntityId("Shutter Fly");                 cust1.setCompanyName("Shutter Fly, Inc");                 cust1.setUnsubscribe(false);                                  Customer cust2 = new Customer();                 cust2.setEntityId("GNC");                 cust2.setCompanyName("GNC Corp");                 cust2.setUnsubscribe(false);                                  Customer[] customers = new Customer[2];                 customers[0] = cust1;                 customers[1] = cust2;                                  WriteResponseList responseList = _port.addList(customers);         }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

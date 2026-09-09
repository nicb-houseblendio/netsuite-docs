---
id: "section_N3499748"
type: "section"
title: "getList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html"
anchors: ["bridgehead_N3499789", "bridgehead_N3499904", "bridgehead_N3500055", "bridgehead_N3500124", "bridgehead_N27094021", "bridgehead_N27094101", "bridgehead_N27094161", "bridgehead_N27094221"]
sha256: "5fce2445e8e930e8f604f0ecdc80d0052ab0ac56a82f54da7e281a11d95ec515"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The getList operation is used to retrieve a list of one or more records by providing the unique ids that identify those records.

If there are multiple ids provided, they can either belong to the same record type or different record types. For example, it is possible to retrieve a customer and a contact within a single request using this operation.

If some of the provided ids are invalid, the request is still processed for the valid ids and the response will contain a warning that indicates that some of the ids were invalid.

Note:

An asynchronous equivalent is available for this operation, **asyncGetList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Request {#bridgehead_N3499789}

The getListRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| recordRef | RecordRef | An array of recordRef objects that specify the ids of the records to be retrieved. |

## Response {#bridgehead_N3499904}

The getListResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| recordList | Record\[\] | A list of records that correspond to the specified ids. The records returned need to be of a type that extends the abstract type Record. |

## Faults {#bridgehead_N3500055}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3500124}

## SOAP Request {#bridgehead_N27094021}

In the following example, two records are retrieved - one customer record and one employee record. Note that you must provide the internal ID of the specify instance of the record and the record type for the getList.

          `<soap:Body> <platformMsgs:getList>    <platformMsgs:baseRef internalId="983" type="customer" xsi:type="platformCore:RecordRef"/>    <platformMsgs:baseRef internalId="-5" type="employee" xsi:type="platformCore:RecordRef"/> </platformMsgs:getList> </soap:Body>` 
        

## SOAP Response {#bridgehead_N27094101}

          `<soapenv:Body> <getListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <readResponseList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <readResponse>       <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <record internalId="983" xsi:type="ns2:Customer"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns2="urn:relationships_2017_1.lists.webservices.netsuite.com">          <ns2:entityId>Shutter Fly</ns2:entityId>          <ns2:isInactive>false</ns2:isInactive>          <ns2:companyName>Shutter Fly, Inc</ns2:companyName>          .          ...[more fields]          .          <ns2:customFieldList>             <ns6:customField internalId="265" scriptId="custentity_map"              xsi:type="ns6:StringCustomFieldRef"              xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">                   <ns6:value>http://maps.google.com</ns6:value>             </ns6:customField>          </ns2:customFieldList>       </record>    </readResponse>    <readResponse>       <ns8:status isSuccess="true" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>       <record internalId="-5" xsi:type="ns9:Employee"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns9="urn:employees_2017_1.lists.webservices.netsuite.com">          <ns9:entityId>A Wolfe</ns9:entityId>          <ns9:isInactive>false</ns9:isInactive>          .          ...[more fields]          .       </record>    </readResponse> </readResponseList> </getListResponse>  </soapenv:Body>` 
        

## C# {#bridgehead_N27094161}

          `private int getCustomerList() {    // This operation requires a valid session    this.login( true );        // Prompt for list of nsKeys and place in an array    _out.write( "\nnsKeys for records to retrieved (separated by commas): " );    String reqKeys = _out.readLn();    string [] nsKeys = reqKeys.Split( new Char[] {','} );        return getCustomerList( nsKeys, false ); }` 
        

## Java {#bridgehead_N27094221}

          `public int getCustomerList() throws RemoteException, ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault, ExceededRecordCountFault {    // This operation requires a valid session    this.login(true);        // Prompt for list of nsKeys and place in an array    _console    .write("\nnsKeys for records to retrieved (separated by commas): ");    String reqKeys = _console.readLn();    String[] nsKeys = reqKeys.split(",");        return getCustomerList(nsKeys, false); }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

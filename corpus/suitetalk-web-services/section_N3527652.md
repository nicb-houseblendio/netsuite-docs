---
id: "section_N3527652"
type: "section"
title: "updateList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > updateList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html"
anchors: ["bridgehead_N3527700", "bridgehead_N3527837", "bridgehead_N3530801", "bridgehead_N3530876", "bridgehead_N27321281", "bridgehead_N27321361", "bridgehead_N27321421", "bridgehead_N27321481"]
sha256: "0b6fe12aab2ce4b84967a512ee559035344de4da6db292fd37ae0db3e39b5d3b"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The updateList operation is used to update one or more instances of a record type in NetSuite.

If there are multiple records, they can either be of the same record type or different record types. For example, it's possible to update a customer and a contact within a single request using this operation.

Only the fields that have been populated in each submitted record are updated in the system. If a field has not been populated, it is not updated in the system and it retains its previous value. If a field is set to an empty string, the previous value of the field is replaced with an empty string.

Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of a particular type must all be from the same external application.

Important:

Calculated and hidden fields in records are always updated by the system unless your service explicitly overrides the system values. For more information, refer to [Hidden Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439416.html#bridgehead_N3439516).

Note:

As of the 2011.2 endpoint, when a record is updated and the values that are sent are the same as the existing record values, the record is not reset (nothing happens). In previous endpoints, sometimes records were reset in these cases.

## Request {#bridgehead_N3527700}

The UpdateListRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record\[\] | Record | Contains an array of record objects. The record type is an abstract type so an instance of a type that extends record must be used-such as Customer or Event. |

Note:

An asynchronous equivalent is available for this operation, **asyncUpdateList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Response {#bridgehead_N3527837}

The UpdateListResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response\[\] | WriteResponse | Contains an array of WriteResponse objects, each of which contains details on the status of that update operation and a reference to the created record. |

## Faults {#bridgehead_N3530801}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3530876}

## SOAP Request {#bridgehead_N27321281}

In the following example, two customer records are updated. The first has the single field companyName updated, whereas the second updates two fields: entityID and companyName. The internalID for each record must be provided and the type of record (Customer) to be updated.

          `<soap:Body> <platformMsgs:updateList>    <platformMsgs:record internalId="980" xsi:type="listRel:Customer">       <listRel:companyName>Shutter Fly Corporation</listRel:companyName>    </platformMsgs:record>    <platformMsgs:record internalId="981" xsi:type="listRel:Customer">       <listRel:entityId>GNCC</listRel:entityId>       <listRel:companyName>GNCC Corp</listRel:companyName>    </platformMsgs:record> </platformMsgs:updateList> </soap:Body>` 
        

## SOAP Response {#bridgehead_N27321361}

          `<soapenv:Body> <updateListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponseList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <writeResponse>       <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="980" type="customer" xsi:type="ns2:RecordRef"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse>    <writeResponse>       <ns3:status isSuccess="true" xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="981" type="customer" xsi:type="ns4:RecordRef"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse> </writeResponseList> </updateListResponse> </soapenv:Body>` 
        

## C# {#bridgehead_N27321421}

          `private void updateCustomerList() {    // This operation requires a valid session    this.login( true );        // Prompt for list of nsKeys and place in an array    _out.write( "\nEnter nsKeys for customer records to be updated (separated by commas): " );    String reqKeys = _out.readLn();    string [] nsKeys = reqKeys.Split( new Char[] {','} );        // Create an array of Record objects to hold the customers    Record[] records = new Record[nsKeys.Length];        // For each submitted nsKey, populate a customer object    for ( int i=0; i<nsKeys.Length; i++)    {       Customer customer = new Customer();              // Update name       customer.entityId = "XYZ Inc " + i;       customer.companyName = "XYZ, Inc. " + i;              customer.internalId = nsKeys[i].Trim();       records[i] = customer;    }        // Invoke updateList() operation to update customers    WriteResponse[] responses = _service.updateList( records );        // Process responses for all successful updates    _out.info( "\nThe following customers were updated successfully:" );    bool hasFailures = false;    for ( int i=0; i<responses.Length; i++ )    {       if ( (responses[i] != null) && (responses[i].status.isSuccess) )       {          _out.info( "\nCustomer[" + i + "]:" );          _out.info(          "key=" + ((RecordRef) responses[i].baseRef).internalId +          "\nentityId=" + ((Customer) records[i]).entityId +          "\ncompanyName=" + ((Customer) records[i]).companyName );       }       else       {          hasFailures = true;       }    }        // Process responses for all unsuccessful updates    if ( hasFailures )    {       _out.info( "\nThe following customers were not updated:\n" );       for ( int i=0; i<responses.Length; i++ )       {          if ( (responses[i] != null) && (!responses[i].status.isSuccess) )          {             _out.info( "Customer[" + i + "]:" );             _out.info( "key=" + ((RecordRef) responses[i].baseRef).internalId );             _out.errorForRecord( getStatusDetails( responses[i].status ) );          }       }    } }` 
        

## Java {#bridgehead_N27321481}

          `public void updateCustomerList() throws RemoteException, ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault, ExceededRecordCountFault {    // This operation requires a valid session    this.login(true);        // Prompt for list of nsKeys and place in an array    _console    .write("\nEnter nsKeys for customer records to be updated (separated by commas): ");    String reqKeys = _console.readLn();    String[] nsKeys = reqKeys.split(",");        // Create an array of Record objects to hold the customers    Record[] records = new Record[nsKeys.length];        // For each submitted nsKey, populate a customer object    for (int i = 0; i < nsKeys.length; i++) {       Customer customer = new Customer();              // Update name       customer.setEntityId("XYZ Inc " + i);       customer.setCompanyName("XYZ, Inc. " + i);              customer.setInternalId(nsKeys[i].trim());       records[i] = customer;    }        // Invoke updateList() operation to update customers    WriteResponseList responseList = _port.updateList(records);        // Process responses for all successful updates    WriteResponse[] responses = responseList.getWriteResponse();    boolean hasFailures = false;    _console.info("\nThe following customers were updated successfully:");    for (int i = 0; i < responses.length; i++) {       if ((responses[i] != null)       && (responses[i].getStatus().isIsSuccess())) {          _console.info("\nCustomer[" + i + "]:");          _console.info("key="          + ((RecordRef) responses[i].getBaseRef()).getInternalId()          + "\nentityId="          + ((Customer) records[i]).getEntityId()          + "\ncompanyName="          + ((Customer) records[i]).getCompanyName());       } else {          hasFailures = true;       }    }        // Process responses for all unsuccessful updates    if (hasFailures) {       _console.info("\nThe following customers were not updated:\n");       for (int i = 0; i < responses.length; i++) {          if ((responses[i] != null)          && (!responses[i].getStatus().isIsSuccess())) {             _console.info("Customer[" + i + "]:");             _console.info("key="             + ((RecordRef) responses[i].getBaseRef()).getInternalId());             _console.errorForRecord(getStatusDetails(responses[i]             .getStatus()));          }       }    } }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

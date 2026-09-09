---
id: "section_N3533243"
type: "section"
title: "upsertList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > upsertList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html"
anchors: ["procedure_N3533274", "bridgehead_N3533325", "bridgehead_N3533461", "bridgehead_N3533577", "bridgehead_N3533689", "bridgehead_N27356621", "bridgehead_N27356681", "bridgehead_N27356741", "bridgehead_N27356801"]
sha256: "5b32d5fe2cc1ab2dadc12893b05b2637b62e70c3f5116e293e6ed437512fb7d2"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The upsertList operation is used to add or update one or more instances of a record type in NetSuite.

If there are multiple records, they can either be of the same record type or different record types. For example, it's possible to add or update a customer and a contact within a single request using this operation.

The upsertList operation is similar to both the addList and updateList operations, but upsert can be run without first determining whether records exist in NetSuite. Records are identified by their external ID and their record type. If a record of the specified type with a matching external ID exists in the system, it is updated. If it does not exist, a new record is created.

Because external ID is required for this operation, upsertList is supported only for records that support the external ID field. Also, this operation prohibits the passing of internal ID values.

Note:

To prevent duplicate records, you should use external IDs and the upsert and upsertList operations to add records to NetSuite.

## Limitations on upsertList {#procedure_N3533274}

-   Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of a particular type must all be from the same external application.
    
-   UpsertList cannot complete updates during an [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) operation, when a record is transformed into a record of another type. In this case, upsertList only adds and does not update records.
    
-   Updates through the upsertList operation are also subject to the same limitations as updates through the updateList operation. For details of these limitations, see [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html).
    

## Request {#bridgehead_N3533325}

The UpsertListRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record\[\] | Record | Contains an array of record objects. The record type is an abstract type so an instance of a type that extends record must be used-such as Customer or Event. |

Note:

An asynchronous equivalent is available for this operation, **asyncUpsertList**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Response {#bridgehead_N3533461}

The UpsertListResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response\[\] | WriteResponse | Contains an array of WriteResponse objects, each of which contains details on the status of that upsert operation and a reference to the created or updated record. |

## Faults {#bridgehead_N3533577}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

This operation returns the following run-time error if the passed record type does not support the external ID field:

          `INVALID_RCRD_TYPE:  <record_type> does not support external ID and cannot be used with upsert` 
        

This operation returns the following run-time error if passed data includes internal ID:

          `USER_ERROR:  You cannot set internalId with upsert.` 
        

This operation returns the following run-time error if passed data does not include external ID:

          `USER_ERROR:  This operation requies a value for externalId.` 
        

For more information about error codes, see [Error Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539978.html).

## Sample Code {#bridgehead_N3533689}

## SOAP Request {#bridgehead_N27356621}

          `<soap:Body>          <upsertList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xmlns:q1="urn:relationships_2017_1.lists.webservices.netsuite.com" xsi:type="q1:Customer" externalId="ext1">                <q1:entityId>XYZ Inc 0</q1:entityId>                <q1:companyName>XYZ, Inc. 0</q1:companyName>             </record>             <record xmlns:q2="urn:relationships_2017_1.lists.webservices.netsuite.com" xsi:type="q2:Customer" externalId="ext2">                <q2:entityId>XYZ Inc 1</q2:entityId>                <q2:companyName>XYZ, Inc. 1</q2:companyName>             </record>          </upsertList>       </soap:Body>` 
        

## SOAP Response {#bridgehead_N27356681}

          `<soapenv:Body>          <upsertListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponseList>                <writeResponse>                   <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <baseRef internalId="970" externalId="ext1" type="customer" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                </writeResponse>                <writeResponse>                   <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <baseRef internalId="974" externalId="ext2" type="customer" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                </writeResponse>             </writeResponseList>          </upsertListResponse>       </soapenv:Body>` 
        

## C# {#bridgehead_N27356741}

          `private void upsertCustomerList()         {               // This operation requires a valid session               this.login( true );                            // Prompt for list of externalIds and place in an array               _out.write( "\nEnter externalIds for customer records to be updated (separated by commas): " );               String reqKeys = _out.readLn();               string [] nsKeys = reqKeys.Split( new Char[] {','} );                            // Create an array of Record objects to hold the customers               Record[] records = new Record[nsKeys.Length];                 // For each submitted nsKey, populate a customer object                  for ( int i=0; i<nsKeys.Length; i++)                   {                     Customer customer = new Customer();                                        // Update name                     customer.entityId = "XYZ Inc " + i;                     customer.companyName = "XYZ, Inc. " + i;                                        customer.externalId = nsKeys[i].Trim();                     records[i] = customer;               }                            // Invoke upsertList() operation to create or update customers               WriteResponse[] responses = _service.upsertList( records );                            // Process responses for all successful updates                    _out.info( "\nThe following customers were updated or created successfully:" );                 bool hasFailures = false;               for ( int i=0; i<responses.Length; i++ )               {                     if ( (responses[i] != null) && (responses[i].status.isSuccess) )                     {                           _out.info( "\nCustomer[" + i + "]:");                           _out.info( "internalId=" + ((RecordRef) responses[i].baseRef).internalId + " externalId="+((RecordRef) responses[i].baseRef).externalId +                           "\nentityId=" + ((Customer) records[i]).entityId +                           "\ncompanyName=" + ((Customer) records[i]).companyName );                     }                     else                     {                           hasFailures = true;                     }               }                 // Process responses for all unsuccessful updates               if ( hasFailures )                   {                     _out.info( "\nThe following customers were not updated:\n" );                     for ( int i=0; i<responses.Length; i++ )                     {                           if ( (responses[i] != null) && (!responses[i].status.isSuccess) )                           {                                 _out.info( "Customer[" + i + "]:" );                                 _out.info( "key=" + ((RecordRef) responses[i].baseRef).internalId );                                _out.errorForRecord( getStatusDetails(responses[i].status ) );                           }                     }               }         }` 
        

## Java {#bridgehead_N27356801}

          `public void upsertCustomerList() throws RemoteException,ExceededUsageLimitFault,                         UnexpectedErrorFault,InvalidSessionFault,ExceededRecordCountFault             {                         // This operation requires a valid session                         this.login(true);                           // Prompt for list of externalIds and place in an array                         _console.write("\nEnter externalIds for customer records to be updated (separated by commas): ");                         String reqKeys = _console.readLn();                         String[] nsKeys = reqKeys.split(",");                           // Create an array of Record objects to hold the customers                         Record[] records = new Record[nsKeys.length];                           // For each submitted nsKey, populate a customer object                         for (int i = 0; i < nsKeys.length; i++)                         {                                     Customer customer = new Customer();                                       // Update name                                     customer.setEntityId("XYZ Inc " + i);                                     customer.setCompanyName("XYZ, Inc. " + i);                                     customer.setExternalId(nsKeys[i].trim());                                       records[i] = customer;                         }                           // Invoke upsertList() operation to create or update customers                         WriteResponseList responseList = _port.upsertList(records);                           // Process responses for all successful upserts                         WriteResponse[] responses = responseList.getWriteResponse();                           boolean hasFailures = false;                         _console.info("\nThe following customers were processed successfully:");                           for (int i = 0; i < responses.length; i++)                         {                                     if ((responses[i] != null) && (responses[i].getStatus().isIsSuccess()))                                     {                                                 _console.info("\nCustomer[" + i + "]:");                                                _console.info("key=" + ((RecordRef) responses[i].getBaseRef()).getInternalId()                                                             + "\nexternalId=" + ((RecordRef) responses[i].getBaseRef()).getExternalId()                                                             + "\nentityId="           + ((Customer) records[i]).getEntityId()                                                             + "\ncompanyName=" + ((Customer) records[i]).getCompanyName());                                     }                                     else                                     {                                                 hasFailures = true;                                     }                         }                           // Process responses for all unsuccessful updates                         if (hasFailures)                         {                                     _console.info("\nThe following customers were not updated:\n");                                     for (int i = 0; i < responses.length; i++)                                     {                                                 if ((responses[i] != null) && (!responses[i].getStatus().isIsSuccess()))                                                 {                                                             _console.info("Customer[" + i + "]:");                                                             _console.info("key=" + ((RecordRef) responses[i].getBaseRef()).getInternalId());                                                             _console.errorForRecord(getStatusDetails(responses[i].getStatus()));                                                 }                                     }                         }               }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

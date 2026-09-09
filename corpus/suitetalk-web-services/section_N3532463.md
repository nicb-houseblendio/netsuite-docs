---
id: "section_N3532463"
type: "section"
title: "upsert"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > upsert"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html"
anchors: ["procedure_N3532490", "bridgehead_N3532541", "bridgehead_N3532656", "bridgehead_N3532767", "bridgehead_N3532898", "bridgehead_N27351601", "bridgehead_N27351661", "bridgehead_N27351721", "bridgehead_N27351781"]
sha256: "98b81b86623a265de4121bec0d3d8a8307a9a184c553ed76a8274d06c4972510"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The upsert operation is used to add a new instance or to update an instance of a record in NetSuite. It is similar to the upsertList operation, which allows users to add or update more than one record at a time.

The upsert operation is similar to both the add and update operations, but upsert can be run without first determining whether a record exists in NetSuite. A record is identified by its external ID and its record type. If a record of the specified type with a matching external ID exists in the system, it is updated. If it does not exist, a new record is created.

Because external ID is required for this operation, upsert is supported only for records that support the external ID field. Also, this operation prohibits the passing of internal ID values.

Note:

To prevent duplicate records, you should use external IDs and the upsert and upsertList operations to add records to NetSuite.

## Limitations on upsert {#procedure_N3532490}

-   Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of a particular type must all be from the same external application.
    
-   Upsert cannot complete updates during an [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) operation, when a record is transformed into a record of another type. In this case, upsert only adds and does not update records.
    
-   Updates through the upsert operation are also subject to the same limitations as updates through the update operation. For details of these limitations, see [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html).
    

## Request {#bridgehead_N3532541}

The UpsertRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record | Record | Contains an array of record objects. The record type is an abstract type so an instance of a type that extends record must be used-such as Customer or Event. |

## Response {#bridgehead_N3532656}

The UpsertResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse | Contains details on the status of the operation and a reference to thecreated or updated record. |

## Faults {#bridgehead_N3532767}

-   This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information.
    
    -   InvalidSessionFault
        
    -   InvalidCredentialsFault
        
    -   ExceededRequestLimitFault
        
    -   ExceededUsageLimitFault
        
    -   ExceededRecordCountFault
        
    -   ExceededRequestSizeFault
        
    -   UnexpectedErrorFault
        
-   This operation returns the following run-time error if the passed record type does not support the external ID field:
    
                  `INVALID_RCRD_TYPE:  <record_type> does not support external ID and cannot be used with upsert` 
                
    
-   This operation returns the following run-time error if passed data includes internal ID:
    
                  `USER_ERROR:  You cannot set internalId with upsert.` 
                
    
-   This operation returns the following run-time error if passed data does not include external ID:
    
                  `USER_ERROR:  This operation requies a value for externalId.` 
                
    
    For more information about error codes, see [Error Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539978.html).
    

## Sample Code {#bridgehead_N3532898}

## SOAP Request {#bridgehead_N27351601}

          `<soap:Body>             <upsert xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record xmlns:q1="urn:relationships_2017_1.lists.webservices.netsuite.com" xsi:type="q1:Customer" externalId="THISISMYEXTID">                   <q1:entityId>XYZ 2 Inc</q1:entityId>                   <q1:companyName>XYZ 2, Inc.</q1:companyName>                   <q1:email>bsanders@xyz.com</q1:email>                </record>             </upsert>          </soap:Body>` 
        

## SOAP Response {#bridgehead_N27351661}

          `<soapenv:Body>             <upsertResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <writeResponse>                   <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <baseRef internalId="973" externalId="THISISMYEXTID" type="customer" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                </writeResponse>             </upsertResponse>          </soapenv:Body>` 
        

## C# {#bridgehead_N27351721}

          `private void upsertCustomer()         {               // This operation requires a valid session               this.login( true );                            Customer customer = new Customer();                            // Get externalId for upsert                     _out.write( "\nEnter externalId for customer record to be created or updated : " );               customer.externalId = _out.readLn().ToUpper();                            // Set name and email               customer.entityId = "XYZ 2 Inc";               customer.companyName = "XYZ 2, Inc.";               customer.email = "bsanders@xyz.com";                            // Invoke upsert() operation               WriteResponse response = _service.upsert( customer );                            // Process the response               if (response.status.isSuccess )                  {                     _out.info(                     "\nThe upsert operation was successful :" +                     "\ninternalId=" + ((RecordRef) response.baseRef).internalId +                     "\nexternalId=" + ((RecordRef) response.baseRef).externalId +                     "\nentityId=" + customer.entityId +                     "\ncompanyName=" + customer.companyName);               } else {                     _out.error( getStatusDetails( response.status ) );               }         }` 
        

## Java {#bridgehead_N27351781}

          `public void upsertCustomer() throws RemoteException,ExceededUsageLimitFault,             UnexpectedErrorFault, InvalidSessionFault,ExceededRecordCountFault       {             // This operation requires a valid session             this.login(true);             Customer customer = new Customer();               // Get extenalId for add or update             _console.write("\nEnter externalId for customer record to be updated : ");             customer.setExternalId(_console.readLn());               // Set name and email             customer.setEntityId("XYZ 2 Inc");             customer.setCompanyName("XYZ 2, Inc.");             customer.setEmail("bsanders@xyz.com");               // Invoke upsert() operation             WriteResponse response = _port.upsert(customer);               // Process the response             if (response.getStatus().isIsSuccess())             {                   _console.info("\nThe following customer was created/updated successfully:"                         + "\nkey=" + ((RecordRef) response.getBaseRef()).getInternalId()                         + "\nexternalId=" + ((RecordRef) response.getBaseRef()).getExternalId()                         + "\nentityId=" + customer.getEntityId()                         + "\ncompanyName=" + customer.getCompanyName()                         + "\nemail=" + customer.getEmail());             }             else             {                   _console.error(getStatusDetails(response.getStatus()));             }       }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3488543"
type: "section"
title: "get"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > get"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html"
anchors: ["bridgehead_N3488555", "bridgehead_N3488670", "bridgehead_N3488822", "bridgehead_1535369694", "bridgehead_1535373715", "bridgehead_3705192642", "bridgehead_3705192937", "bridgehead_3705193212", "bridgehead_3705193414"]
sha256: "d9bddf0eb31f1bc826d3183ee0f6313f089f22b8aa6effa981b6d4566ec82fd1"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The get operation is used to retrieve a record by providing the unique id that identifies that record.

## Request {#bridgehead_N3488555}

The getRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| recordRef | RecordRef | A recordRef object that specifies the id of the record to be retrieved. |

## Response {#bridgehead_N3488670}

The getResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| record | Record | A record that represents the specified id. The record returned needs to be a type that extends the abstract type Record. |

## Faults {#bridgehead_N3488822}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Usage Notes for Custom Fields Generated from Custom Segments {#bridgehead_1535369694}

The get operation supports the usage of unified scripts IDs of custom segments. If the unified script ID is used on a custom segment, it is returned, if the legacy one is used, it is returned.

As of 2019.1, any new custom segments that you create automatically use the unified ID.

## SOAP Response with Unified Script ID Used on the Custom Segment {#bridgehead_1535373715}

          `<soapenv:Body>          <getResponse xmlns="urn:messages_2018_2.platform.webservices.netsuite.com">             <readResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2018_2.platform.webservices.netsuite.com"/>                <record internalId="107" xsi:type="listRel:Customer" xmlns:listRel="urn:relationships_2018_2.lists.webservices.netsuite.com">                   <listRel:customForm internalId="3" xmlns:platformCore="urn:core_2018_2.platform.webservices.netsuite.com">                      <platformCore:name>Customer_Preferred=T_Store=F</platformCore:name>                   </listRel:customForm>                   <listRel:entityId>Tim Harris</listRel:entityId>        …[more fields]…                       <platformCore:customField internalId="58" scriptId="cseg_633637_beforeload" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                   </listRel:customFieldList>                </record>             </readResponse>          </getResponse>       </soapenv:Body>` 
        

## SOAP Request - Return Customer Record {#bridgehead_3705192642}

In this example, a single customer record is retrieved. Note that the internal ID for the specific instance of the record and the record type (customer) must be specified.

          `<soapenv:Body>            <get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <baseRef internalId="107" type="customer" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>            </get>        </soapenv:Body>` 
        

## SOAP Response {#bridgehead_3705192937}

          `<soapenv:Body>          <getResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <readResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <record internalId="107" xsi:type="listRel:Customer" xmlns:listRel="urn:relationships_2017_1.lists.webservices.netsuite.com">                   <listRel:customForm internalId="3" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Customer_Preferred=T_Store=F</platformCore:name>                   </listRel:customForm>                   <listRel:entityId>Tim Harris</listRel:entityId>                   <listRel:isPerson>false</listRel:isPerson>                   <listRel:companyName>Glenrock General Hospital</listRel:companyName>                   <listRel:entityStatus internalId="13" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>CUSTOMER-Closed Won</platformCore:name>                   </listRel:entityStatus>                   <listRel:phone>555-394-3830</listRel:phone>                   <listRel:email>tim@example.com</listRel:email>                              ...[more fields]...                                  <listRel:isInactive>false</listRel:isInactive>                   <listRel:dateCreated>2017-09-04T15:59:15.000-07:00</listRel:dateCreated>                   <listRel:emailPreference>_default</listRel:emailPreference>                   <listRel:sendEmail>false</listRel:sendEmail>                   <listRel:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:customField internalId="59" scriptId="custentity_633637_asubmit" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                      <platformCore:customField internalId="58" scriptId="custentity_633637_bload" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                   </listRel:customFieldList>                </record>             </readResponse>          </getResponse>       </soapenv:Body>` 
        

## C# {#bridgehead_3705193212}

          `private void getCustomer() {    // This operation requires a valid session    this.login( true );        // Prompt for the nsKey    _out.write( "\nnsKey for record to be retrieved: " );    String nsKey = _out.readLn();        // Invoke the get() operation to retrieve the record    RecordRef recordRef = new RecordRef();    recordRef.internalId = nsKey;    recordRef.type = RecordType.customer;    recordRef.typeSpecified = true;        ReadResponse response = _service.get( recordRef );        // Process response from get() operation    _out.info( "\nRecord returned from get() operation: " );    if ( !response.status.isSuccess )    {       _out.info(       "ERROR: " +       getStatusDetails( response.status ) );    }    else    {       Customer customer = (Customer) response.record;       _out.info(       "\nnsKey=" + customer.internalId + ", " +       "\nentityId=" + customer.entityId +       (customer.companyName==null ? "" : ("\ncompanyName=" + customer.companyName)) +       (customer.stage==null ? "" : ("\nstage=" + customer.stage)) +       (customer.email==null ? "" : ("\nemail=" + customer.email)) +       (customer.phone==null ? "" : ("\nphone=" + customer.phone)) +       "\nisInactive=" + customer.isInactive +       (!customer.dateCreatedSpecified ? "" : ("\ndateCreated=" +        customer.dateCreated.ToShortDateString())) );    } }` 
        

## Java {#bridgehead_3705193414}

          `public void getCustomer() throws RemoteException, ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault, ExceededRecordCountFault {    // This operation requires a valid session    this.login(true);        // Prompt for the nsKey    _console.write("\nnsKey for record to be retrieved: ");    String nsKey = _console.readLn();        // Invoke the get() operation to retrieve the record    RecordRef recordRef = new RecordRef();    recordRef.setInternalId(nsKey);    recordRef.setType(RecordType.customer);        ReadResponse response = _port.get(recordRef);        // Process response from get() operation    _console.info("\nRecord returned from get() operation: ");    if (!response.getStatus().isIsSuccess()) {       _console.info("ERROR: " + getStatusDetails(response.getStatus()));    } else {       Customer customer = (Customer) response.getRecord();       _console       .info("\nnsKey="       + customer.getInternalId()       + ", "       + "\nentityId="       + customer.getEntityId()       + (customer.getCompanyName() == null ? ""       : ("\ncompanyName=" + customer       .getCompanyName()))       + (customer.getStage() == null ? ""       : ("\nstage=" + customer.getStage()))       + (customer.getEmail() == null ? ""       : ("\nemail=" + customer.getEmail()))       + (customer.getPhone() == null ? ""       : ("\nphone=" + customer.getPhone()))       + "\nisInactive="       + customer.getIsInactive()       + (customer.getDateCreated() != null ? ""       : ("\ndateCreated=" + customer       .getDateCreated().toString())));    } }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3480855"
type: "section"
title: "add"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > add"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html"
anchors: ["bridgehead_N3480874", "bridgehead_N3480989", "bridgehead_N3481101", "bridgehead_N3481177", "bridgehead_3705183801", "bridgehead_3705184071", "bridgehead_3705184350", "bridgehead_3705184657"]
sha256: "db88e2740e755b7d6b8c69d7105c08bf73cd098c5a2afcda528700604db1db89"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The add operation is used to add a new instance of a record in NetSuite. It is similar to the addList operation except that it allows only one record to be added at a time. Note that to prevent duplicate records, you should use the alternate [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) and [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html) operations along with external IDs to add records to NetSuite.

Note:

Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of each type must all be from the same external application.

## Request {#bridgehead_N3480874}

The AddRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record | Record | The record type is an abstract type so an instance of a type that extends record must be used - such as Customer or Event. |

## Response {#bridgehead_N3480989}

The AddResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse | Contains details on the status of the operation and a reference to the created record. |

## Faults {#bridgehead_N3481101}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3481177}

## SOAP Request {#bridgehead_3705183801}

In this example, a single customer record is added.

Note:

For information about adding custom fields to records, see the code sample in [Entity Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3772873.html).

          `<soap:Body> <platformMsgs:add>         <platformMsgs:record xsi:type="listRel:Customer">                 <listRel:companyName>Shutter Fly, Inc</listRel:companyName>                 <listRel:unsubscribe>false</listRel:unsubscribe>         </platformMsgs:record> </platformMsgs:add> </soap:Body>` 
        

## SOAP Response {#bridgehead_3705184071}

In the response, notice that the internal ID for the record added is returned.

          `<soapenv:Body> <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="979" type="customer" xsi:type="ns2:RecordRef"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/> </writeResponse> </addResponse> </soapenv:Body>` 
        

## C# {#bridgehead_3705184350}

          `private void addCustomer() {    // This operation requires a valid session    this.login( true );        Customer customer = new Customer();        // Set entityId, company name, and email    if ( "true".Equals( _dataCollection["promptForFieldValues"] ) )    {       _out.writeLn(       "\nPlease enter the following customer information. " +       "Note that some fields have already been populated. " );       _out.write( "Entity name: " );       customer.entityId = _out.readLn();       _out.write( "Company name: " );       customer.companyName = _out.readLn();       _out.write( "E-mail: " );       customer.email = _out.readLn();       _out.write( "Sales Rep key: " );       RecordRef salesRep = new RecordRef();       salesRep.internalId = _out.readLn();       //salesRep.type = RecordType.contact;       //salesRep.typeSpecified = true;       customer.salesRep = salesRep;    }    else    {       customer.entityId = "XYZ Inc";       customer.companyName = "XYZ, Inc.";       customer.email = "bsanders@yahoo.com";    }        // Set email preference    customer.emailPreference = CustomerEmailPreference._hTML;    customer.emailPreferenceSpecified = true;        // Set entity status. The nsKey can be obtained from Setup > SFA > Customer Statuses.    // The default status is "Closed Won" which has an nsKey of 13    RecordRef status = new RecordRef();    if ( "true".Equals( _dataCollection["promptForFieldValues"] ) )    {       _out.write( "Entity status nsKey (press enter for default value of Closed Won): " );       String statusKey = _out.readLn();       if ( statusKey.Equals( "" ) )       {          status.internalId = "13";       }       else       {          status.internalId = statusKey;       }    }    else    {       status.internalId = "13";    }        customer.entityStatus = status;        // Populate the address list for this customer. You can add as many    // adresses as you like.    CustomerAddressbook address = new CustomerAddressbook();    address.defaultShipping = true;    address.defaultShippingSpecified = true;    address.defaultBilling = false;    address.defaultBillingSpecified = true;    address.label = "Shipping Address";    address.addressee = "William Sanders";    address.attention = "William Sanders";    address.addr1 = "4765 Sunset Blvd";    address.city = "San Francisco";    address.state = "CA";    address.zip = "94131";    address.country = Country._unitedStates;        // Attach the CustomerAddressbookList to the customer    CustomerAddressbookList addressList = new CustomerAddressbookList();    CustomerAddressbook[] addresses = new CustomerAddressbook[1];    addresses[0] = address;    addressList.addressbook = addresses;    customer.addressbookList = addressList;        // Invoke add() operation    WriteResponse response = _service.add( customer );        // Print the document id from the SOAP header    //_out.info(    //"\nThe add() operation with document id " + _service.documentInfo.nsID + " was processed " );        // Process the response    if ( response.status.isSuccess )    {       _out.info(       "\nThe following customer was added successfully:" +       "\nkey=" + ((RecordRef) response.baseRef).internalId +       "\nentityId=" + customer.entityId +       "\ncompanyName=" + customer.companyName +       "\nemail=" + customer.email +       "\nstatusKey=" + customer.entityStatus.internalId +       "\naddressbookList[0].label=" + customer.addressbookList.addressbook[0].label );              // Create a second customer that's a sub-customer of the first customer       /*       Customer subCustomer = new Customer();              subCustomer.entityId = "XYZ Japan";              // Set the parent customer       recordRef = new RecordRef();       recordRef.internalId = ((RecordRef) response.baseRef).internalId;       //recordRef.internalId = "125";       subCustomer.parent = recordRef;              // Invoke add() operation       response = _service.add( subCustomer );              // Process the response       //"\nThe add() operation with job id " + _service.sessionInfo.jobID + " was processed " );       if ( !response.status.isSuccess )       {          _out.info( "\nThe customer was not added:" );          _out.error( getStatusDetails( response.status ) );       }       else       {          _out.info(          "\nThe following customer was added successfully:" +          "\nkey=" + ((RecordRef) response.baseRef).internalId +          "\nentityId=" + customer.entityId +          "\ncompanyName=" + customer.companyName);       }       */    }    else    {       _out.error( "The customer was not added:", true );       _out.error( getStatusDetails( response.status ) );    } }` 
        

## Java {#bridgehead_3705184657}

          `public void addCustomer() throws RemoteException, ExceededRecordCountFault, ExceededUsageLimitFault, InsufficientPermissionFault, InvalidSessionFault {    // This operation requires a valid session    this.login(true);        Customer customer = new Customer();        // Set entityId, company name, and email    if ("true".equals(_properties.getProperty("promptForFieldValues"))) {       _console       .writeLn("\nPlease enter the following customer information. "       + "Note that some fields have already been populated. ");       _console.write("Entity name: ");       customer.setEntityId(_console.readLn());       _console.write("Company name: ");       customer.setCompanyName(_console.readLn());       _console.write("E-mail: ");       customer.setEmail(_console.readLn());    } else {       customer.setEntityId("XYZ Inc");       customer.setCompanyName("XYZ, Inc.");       customer.setEmail("bsanders@yahoo.com");    }        // Set email preference.    customer.setEmailPreference(CustomerEmailPreference._hTML);        // Set entity status. The nsKey can be obtained from Setup > SFA >    // Customer Statuses.    // The default status is "Closed Won" which has an nsKey of 13    RecordRef status = new RecordRef();    if ("true".equals(_properties.getProperty("promptForFieldValues"))) {       _console.write("Entity status nsKey (press enter for default value of Closed Won): ");       String statusKey = _console.readLn();       if (statusKey.equals("")) {          status.setInternalId("13");       } else {          status.setInternalId(statusKey);       }    } else {       status.setInternalId("13");    }        customer.setEntityStatus(status);        // Populate the address list for this customer. You can add as many    // adresses as you like.    CustomerAddressbook address = new CustomerAddressbook();    address.setDefaultShipping(Boolean.TRUE);    address.setDefaultBilling(Boolean.FALSE);    address.setLabel("Shipping Address");    address.setAddressee("William Sanders");    address.setAttention("William Sanders");    address.setAddr1("4765 Sunset Blvd");    address.setCity("San Francisco");    address.setState('CA');    address.setZip("94131");    address.setCountry(Country._unitedStates);        // Attach the CustomerAddressbookList to the customer    CustomerAddressbookList addressList = new CustomerAddressbookList();    CustomerAddressbook[] addresses = new CustomerAddressbook[1];    addresses[0] = address;    addressList.setAddressbook(addresses);    customer.setAddressbookList(addressList);        // Invoke add() operation    WriteResponse response = _port.add(customer);        // Print the document id from the SOAP header    // _console.info(    // "\nThe add() operation with document id " + _port.documentInfo.nsID +    // " was processed " );        // Process the response    if (response.getStatus().isIsSuccess()) {       _console.info("\nThe following customer was added successfully:"       + "\nkey="       + ((RecordRef) response.getBaseRef()).getInternalId()       + "\nentityId="       + customer.getEntityId()       + "\ncompanyName="       + customer.getCompanyName()       + "\nemail="       + customer.getEmail()       + "\nstatusKey="       + customer.getEntityStatus().getInternalId()       + "\naddressbookList[0].label="       + customer.getAddressbookList().getAddressbook(0)       .getLabel());    } else {       _console.error("The customer was not added:", true);       _console.error(getStatusDetails(response.getStatus()));    } }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

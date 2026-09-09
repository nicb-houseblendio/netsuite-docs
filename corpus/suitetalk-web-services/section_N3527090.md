---
id: "section_N3527090"
type: "section"
title: "update"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > update"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html"
anchors: ["bridgehead_N3527149", "bridgehead_N3527264", "bridgehead_N3527376", "bridgehead_N3527452", "bridgehead_N27316651", "bridgehead_N27316731", "bridgehead_N27316791", "bridgehead_N27316851", "bridgehead_N3527507"]
sha256: "7d9d5d7f690f485fe601e7b6373a26ca0d18a79d3d278d7cb67cf6ea97d4b4da"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The update operation is used to update an instance of a record in NetSuite. It is similar to the updateList operation, which allows users to update more than one record at a time.

Only the fields that have been populated in each submitted record are updated in the system. If a field has NOT been populated, it is not updated in the system and it retains its previous value. If a field is set to an empty string, the previous value of the field is replaced with an empty string. Therefore, when updating records, you should get the desired record, instantiate a new record of the same type, populate only the fields that require an update and then submit the updated record. This ensures that only the fields requiring an update are written on submission.

Important:

Calculated and hidden fields in records are always updated by the system unless your service explicitly overrides the system values. For more information, see [Hidden Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439416.html#bridgehead_N3439516). Also, custom fields can only be set to NULL by submitting the field in nullFieldList. For more information, see [CustomFieldList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438152.html).

To ensure that the most recent data for a specific record is being modified, when a Web service request is received, the values for that record are retrieved at the time of the Update request rather than with the initial Get of the associated record. The record is then updated by the values submitted in the request. It is possible that between the time of the retrieval of the record field values and the submission of the updated fields that the record is altered from another source (for example from a UI submission). In this case an error message is returned to indicate that the fields have been modified since your service retrieved the record.

Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of a particular type must all be from the same external application.

Note:

When a record is updated and the values that are sent are the same as the existing record values, the record is not reset (nothing happens). In previous endpoints, sometimes records were reset in these cases.

## Request {#bridgehead_N3527149}

The UpdateRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record | Record | Contains an array of record objects. The record type is an abstract type so an instance of a type that extends record must be used-such as Customer or Event. |

## Response {#bridgehead_N3527264}

The UpdateResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse | Contains details on the status of the operation and a reference to the updated record. |

## Faults {#bridgehead_N3527376}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3527452}

## SOAP Request {#bridgehead_N27316651}

In the following example, a customer's companyName is updated. The internal ID for the customer must be provided in the request.

          `<soap:Body> <platformMsgs:update>    <platformMsgs:record internalId="980" xsi:type="listRel:Customer">       <listRel:companyName>Shutter Fly Corporation</listRel:companyName>    </platformMsgs:record> </platformMsgs:update> </soap:Body>` 
        

## SOAP Response {#bridgehead_N27316731}

          `<soapenv:Body> <updateResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="980" type="customer" xsi:type="ns2:RecordRef"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/> </writeResponse> </updateResponse> </soapenv:Body>` 
        

## C# {#bridgehead_N27316791}

          `private void updateCustomer() {    // This operation requires a valid session    this.login( true );        Customer customer = new Customer();        // Get nsKey for update    _out.write( "\nEnter nsKey for customer record to be updated : " );    customer.internalId = _out.readLn().ToUpper();        // Set name and email    customer.entityId = "XYZ 2 Inc";    customer.companyName = "XYZ 2, Inc.";    customer.email = "bsanders@xyz.com";        // Populate the address. Updating a list through WS results in the    // entire contents of the previous list being replaced by the new    // list.    CustomerAddressbook address = new CustomerAddressbook();    address.defaultBilling = true;    address.defaultBillingSpecified = true;    address.defaultBilling = false;    address.defaultBillingSpecified = true;    address.label = "Billing Address";    address.addr1 = "4765 Sunset Blvd";    address.city = "San Mateo";    address.state = "CA";    address.country = Country._unitedStates;        // Attach the address to the customer    CustomerAddressbookList addressList = new CustomerAddressbookList();    CustomerAddressbook[] addresses = new CustomerAddressbook[1];    addresses[0] = address;    addressList.addressbook = addresses;    customer.addressbookList = addressList;        // Invoke add() operation    WriteResponse response = _service.update( customer );        // Process the response    if ( response.status.isSuccess )    {       _out.info(       "\nThe following customer was updated successfully:" +       "\nkey=" + ((RecordRef) response.baseRef).internalId +       "\nentityId=" + customer.entityId +       "\ncompanyName=" + customer.companyName +       "\nemail=" + customer.email +       "\naddressbookList[0].label=" + customer.addressbookList.addressbook[0].label );    }    else    {       _out.error( getStatusDetails( response.status ) );    } }` 
        

## Java {#bridgehead_N27316851}

          `public void updateCustomer() throws RemoteException, ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault, ExceededRecordCountFault {    // This operation requires a valid session    this.login(true);        Customer customer = new Customer();        // Get nsKey for update    _console.write("\nEnter nsKey for customer record to be updated : ");    customer.setInternalId(_console.readLn().toUpperCase());        // Set name and email    customer.setEntityId("XYZ 2 Inc");    customer.setCompanyName("XYZ 2, Inc.");    customer.setEmail("bsanders@xyz.com");        // Populate the address. Updating a list through WS results in the    // entire contents of the previous list being replaced by the new    // list.    CustomerAddressbook address = new CustomerAddressbook();    address.setDefaultBilling(Boolean.TRUE);    address.setDefaultShipping(Boolean.FALSE);    address.setLabel("Billing Address");    address.setAddr1("4765 Sunset Blvd");    address.setCity("San Mateo");    address.setState('CA');    address.setCountry(Country._unitedStates);        // Attach the address to the customer    CustomerAddressbookList addressList = new CustomerAddressbookList();    CustomerAddressbook[] addresses = new CustomerAddressbook[1];    addresses[0] = address;    addressList.setAddressbook(addresses);    customer.setAddressbookList(addressList);        // Invoke add() operation    WriteResponse response = _port.update(customer);        // Process the response    if (response.getStatus().isIsSuccess()) {       _console.info("\nThe following customer was updated successfully:"       + "\nkey="       + ((RecordRef) response.getBaseRef()).getInternalId()       + "\nentityId="       + customer.getEntityId()       + "\ncompanyName="       + customer.getCompanyName()       + "\nemail="       + customer.getEmail()       + "\naddressbookList[0].label="       + customer.getAddressbookList().getAddressbook(0)       .getLabel());    } else {       _console.error(getStatusDetails(response.getStatus()));    } }` 
        

## Updating Record Lists {#bridgehead_N3527507}

When updating a list of records (a sublist) within a business record you CANNOT update a specific item in the list. Instead you must interact with the sublist as a whole. For details, see [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

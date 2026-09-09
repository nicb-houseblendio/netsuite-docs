---
id: "section_N3498308"
type: "section"
title: "getItemAvailability"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getItemAvailability"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3498308.html"
anchors: ["bridgehead_N3498335", "bridgehead_N3498452", "bridgehead_N3498599", "bridgehead_N3498752", "bridgehead_N3499349", "bridgehead_N3499496", "bridgehead_N3499572", "bridgehead_N27089561", "bridgehead_N27089621", "bridgehead_N27089681", "bridgehead_N27089741"]
sha256: "cbdc1cbad0c306b96cbbe859fb7c7712d9330bd8b2801e5cc050d2507c1697d3"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The getItemAvailability operation can be used to retrieve the inventory availability for a specific list of items.

You can filter the returned list using a lastQtyAvailableChange filter. If set, only items with quantity available changes recorded as of this date are returned.

If the Multi-Location Inventory feature is enabled, this operation returns results for all locations. For locations that do not have any items available, only location IDs and names are listed in results.

Warning:

This operation supports up to 10,000 records. If this limit is exceeded, an error is returned.

## Request {#bridgehead_N3498335}

The GetItemAvailabilityRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| itemAvailabilityFilter | ItemAvailabilityFilter | You can filter the returned itemAvailability using this filter. |

## ItemAvailabilityFilter {#bridgehead_N3498452}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| item | RecordRefList | References an exiting item record in NetSuite. |
| lastQtyAvailableChange | dateTime | If set, only items with quantity available changes recorded as of the specified date are returned. |

## Response {#bridgehead_N3498599}

The GetItemAvailabilityResult type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| itemAvailabilityList | List | Returns a list of available items. |

## ItemAvailabilityList {#bridgehead_N3498752}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| item | RecordRef | References an existing item record. |
| lastQtyAvailableChange | dateTime | If set, only items with quantity available changes recorded as of this date are returned. |
| locationId | RecordRef | References a location in a user defined list at Lists > Accounting > Locations. |
| quantityOnHand | double | The number of units of an item in stock. |
| onHandValueMli | double |  |
| reorderPoint | double | The stock level at which a new order for the item needs to be placed |
| preferredStockLevel | double | The preferred quantity of this item maintained in inventory for a specific location. |
| quantityOnOrder | double | The number of units of an item pending receipt from a vendor. |
| quantityCommitted | double | The number of units of an item reserved by unfulfilled sales orders. |
| quantityBackOrdered | double | The number of units of an item reserved by unfulfilled sales orders. |
| quantityAvailable | double | The number of units in stock that have not been committed to fulfill sales. |

## ItemAvailabilityFilter {#bridgehead_N3499349}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| item | RecordRefList |  |
| lastQtyAvailableChange | dateTime |  |

## Faults {#bridgehead_N3499496}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3499572}

## SOAP Request (for C# sample) {#bridgehead_N27089561}

          `<soap:Body> <platformMsgs:getItemAvailability>    <platformMsgs:itemAvailabilityFilter>       <platformCore:item>          <platformCore:recordRef internalId="390" type="inventoryItem">             <platformCore:name/>          </platformCore:recordRef>       </platformCore:item>       <platformCore:lastQtyAvailableChange/>    </platformMsgs:itemAvailabilityFilter> </platformMsgs:getItemAvailability> </soap:Body>` 
        

## SOAP Response (for C# sample) {#bridgehead_N27089621}

          `<soapenv:Body> <getItemAvailabilityResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <getItemAvailabilityResult        xmlns="urn:core_2017_1.platform.webservices.netsuite.com">       <status isSuccess="true"/>       <itemAvailabilityList>          <itemAvailability>             <item internalId="390" type="inventoryItem">                <name>testItem</name>             </item>             <locationId internalId="1" type="location">                <name>East Coast</name>             </locationId>             <quantityOnHand>20.0</quantityOnHand>             <onHandValueMli>0.0</onHandValueMli>             <quantityCommitted>0.0</quantityCommitted>             <quantityAvailable>20.0</quantityAvailable>          </itemAvailability>          <itemAvailability>             <item internalId="390" type="inventoryItem">                <name>testItem</name>             </item>             <locationId internalId="2" type="location">                <name>West Coast</name>             </locationId>          </itemAvailability>       </itemAvailabilityList>    </getItemAvailabilityResult> </getItemAvailabilityResponse> </soapenv:Body>` 
        

## C# Sample {#bridgehead_N27089681}

          `private void getItemAvailability()         {             this.login(true);               RecordRef item1 = new RecordRef();             item1.internalId = "59";             item1.type = RecordType.inventoryItem;             item1.typeSpecified = true;               RecordRef[] recordrefs = new RecordRef[1];             recordrefs[0] = item1;               ItemAvailabilityFilter filter = new ItemAvailabilityFilter();             filter.item = recordrefs;             GetItemAvailabilityResult res = _service.getItemAvailability(filter);                              }` 
        

## Java Sample {#bridgehead_N27089741}

          `public void getItemAvailability() throws RemoteException {                 this.login(true);                                  RecordRef item1 = new RecordRef();                 item1.setInternalId("25");                 item1.setType(RecordType.inventoryItem);                                  RecordRef item2 = new RecordRef();                 item2.setInternalId("76");                 item2.setType(RecordType.giftCertificateItem);                                  RecordRef[] recordRefArray = new RecordRef[2];                 recordRefArray[0] = item1;                 recordRefArray[1] = item2;                                  RecordRefList itemRefList = new RecordRefList();                 itemRefList.setRecordRef(recordRefArray);                                  ItemAvailabilityFilter itemAvailability = new ItemAvailabilityFilter();                 itemAvailability.setItem(itemRefList);                                  GetItemAvailabilityResult response = _port.getItemAvailability(itemAvailability);         }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

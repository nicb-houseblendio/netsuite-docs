---
id: "section_N3503649"
type: "section"
title: "getSavedSearch"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getSavedSearch"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html"
anchors: ["bridgehead_N3503685", "bridgehead_N3503800", "bridgehead_N3503984", "bridgehead_N3504059", "bridgehead_N27139961", "bridgehead_N27140021", "bridgehead_N27139841", "bridgehead_N27139901"]
sha256: "13b0f85821bc8ab432e836ddf4680b0666df2cdcfd426d2a132416d0b778f811"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

This operation allows users to retrieve a list of existing saved search IDs on a per-record-type basis (for example, all saved search IDs for every Customer saved search). Note that after you retrieve the list of saved search IDs, you may need to look in the NetSuite UI to see the criteria defined for the saved search. To go to the list of saved searches in the NetSuite UI, go to _Lists > Search > Saved Searches_.

This API takes a search record type as a request argument and returns a list of record references of the saved search. For each saved search, the response includes the internalId, scriptId, and name.

For use cases explaining why you would want to get a list of saved search IDs and then reference a specific ID in your code, see [Reference Existing Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html#bridgehead_N3517038).

Note:

There is no async equivalent for this operation.

## Request {#bridgehead_N3503685}

The GetSavedSearchRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| record | GetSavedSearchRecord |  |

## Response {#bridgehead_N3503800}

The GetSavedSearchResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| totalRecords | xsd:int | The total number of records for this search. Depending on the pageSize value, some or all the records may be returned in this response |
| recordRefList | Record\[\] | A list of records that correspond to the specified ids. The records returned need to be of a type that extends the abstract type Record. |

## Faults {#bridgehead_N3503984}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3504059}

## C# {#bridgehead_N27139961}

          `GetSavedSearchRecord record = new GetSavedSearchRecord(); record.searchTypeSpecified = true; record.searchType = SearchRecordType.transaction;  _service.getSavedSearch(record); ;` 
        

## Java {#bridgehead_N27140021}

          `public void getSavedSearches() throws RemoteException{   this.login(true);      GetSavedSearchRecord record = new GetSavedSearchRecord();   record.setSearchType(SearchRecordType.transaction);                    GetSavedSearchResult result = _port.getSavedSearch(record); }` 
        

## SOAP Request {#bridgehead_N27139841}

          `<soap:Body>         <getSavedSearch xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record searchType="transaction"/>         </getSavedSearch>     </soap:Body>` 
        

## SOAP Response {#bridgehead_N27139901}

          `<soapenv:Body>    <getSavedSearchResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <platformCore:getSavedSearchResult xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">          <platformCore:status isSuccess="true"/>       <platformCore:totalRecords>5</platformCore:totalRecords>       <platformCore:recordRefList>          <platformCore:recordRef xsi:type="platformCore:CustomizationRef" internalId="26" scriptId="customsearch26">             <platformCore:name>Custom Transaction Search</platformCore:name>           </platformCore:recordRef>             <platformCore:recordRef xsi:type="platformCore:CustomizationRef" internalId="27" scriptId="customsearch27">                <platformCore:name>CC Transaction Search</platformCore:name>             </platformCore:recordRef>             <platformCore:recordRef xsi:type="platformCore:CustomizationRef" internalId="42" scriptId="customsearch42">                 <platformCore:name>Returned Items</platformCore:name>          </platformCore:recordRef>          <platformCore:recordRef xsi:type="platformCore:CustomizationRef" internalId="44" scriptId="customsearch44">                <platformCore:name>Ordered More than One Item</platformCore:name>          </platformCore:recordRef>             <platformCore:recordRef xsi:type="platformCore:CustomizationRef" internalId="46" scriptId="customsearch46">                <platformCore:name>Spending Account Average</platformCore:name>                </platformCore:recordRef>          </platformCore:recordRefList>       </platformCore:getSavedSearchResult>    </getSavedSearchResponse> </soapenv:Body>` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

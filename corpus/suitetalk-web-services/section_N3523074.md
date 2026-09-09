---
id: "section_N3523074"
type: "section"
title: "searchMoreWithId"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > searchMoreWithId"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html"
anchors: ["bridgehead_1509528108", "bridgehead_N3523191", "bridgehead_N3523343", "bridgehead_N3523710", "bridgehead_N3523786", "bridgehead_N27289821", "bridgehead_N27289881", "bridgehead_N27289941", "bridgehead_N27290011", "bridgehead_N27290081"]
sha256: "98486df14d9fa851837b5b865754723b09bed6a3dbf1b8bf765d9fae7f69ca90"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Users who authenticate to NetSuite by providing their credentials in the SOAP header of their requests **must** use searchMoreWithId to retrieve search results that span multiple pages.

The searchMoreWithId operation allows you to reference a specific search result set by its searchId, a parameter included in all search results. As with searchMore, you must set the pageIndex value to specify which page in the search to return.

## Usage Notes {#bridgehead_1509528108}

Consider the following information when you use the searchMoreWithId operation.

-   When you paginate through the search results, the searchMoreWithId operation triggers a new search for the page specified by the pageIndex value. If records included in the search result set are updated while you go through the result pages, and they do not match the earlier search criteria anymore, they will be omitted from the results displayed on that page you specified. To avoid this, you need to ensure that records are not modified while you are calling a search operation.
    
-   Search IDs expire if they have not been used within 15 minutes after their creation. Passing an expired or invalid searchId will return search results with a 'failed' status and StatusDetailCode=INVALID\_JOB\_ID.
    
-   There is no async equivalent for this operation.
    
-   For information about achieving the best search performance, see [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html).
    

## Request {#bridgehead_N3523191}

The SearchMoreWithIdRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| searchId | string | The search result ID. |
| pageIndex | int | An index that specifies which page in the search to return. |

## Response {#bridgehead_N3523343}

The SearchMoreWithIdResponse type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this search. All applicable errors or warnings will be listed within this type. |
| totalRecords | xsd:int | The total number of records for this search. Depending on the pageSize value, some or all the records may be returned in this response |
| pageSize | xsd:int | The page size for this search. |
| totalPages | xsd:int | The total number of pages that are part of this search. |
| pageIndex | xsd:int | The page index for the current set of results. |
| searchId | string | Returns a specific search based on its search ID. |
| recordList | Record\[\] | A list of records that meet the criteria for this search. The records returned need to be of a type that extends the abstract type of record. |
| searchRowList | SearchRowList | A list of return columns that meet the criteria for this search. |

## Faults {#bridgehead_N3523710}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3523786}

The following samples show the SOAP for the initial search as well as the SOAP for subsequent searchMoreWithId operation used to specify the next page of the search. The ID returned in the initial search is specified as the searchId when executing searchMoreWithId.

Note:

Prefix-to-namespace mappings have been omitted for readability.

## SOAP Request for Initial Search {#bridgehead_N27289821}

          `<soapenv:Envelope>     <soapenv:Header>         <platformMsgs:searchPreferences>             <platformMsgs:bodyFieldsOnly>true</platformMsgs:bodyFieldsOnly>             <platformMsgs:pageSize>100</platformMsgs:pageSize>         </platformMsgs:searchPreferences>         <platformMsgs:passport>             <platformCore:email>jdoe@netsuite.com</platformCore:email>             <platformCore:password><SOAP web services password></platformCore:password>             <platformCore:account>000034</platformCore:account>             <platformCore:role internalId="37"/>         </platformMsgs:passport>     </soapenv:Header>     <soapenv:Body>         <platformMsgs:search>             <searchRecord xsi:type="platformCommon:ContactSearchBasic">                 <platformCommon:city operator="is" xsi:type="platformCore:SearchStringField">                     <platformCore:searchValue xsi:type="xsd:string">San Francisco</platformCore:searchValue>                 </platformCommon:city>             </searchRecord>         </platformMsgs:search>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response for Initial Search {#bridgehead_N27289881}

          `<soapenv:Envelope>     <soapenv:Header>         <platformMsgs:documentInfo>             <platformMsgs:nsId>WEBSERVICES_528736_07012008543995006307049233_d53ef4d2273b15<       platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <platformMsgs:searchResponse>           <platformCore:searchResult>           <platformCore:status isSuccess="true"/>           <platformCore:totalRecords>231</platformCore:totalRecords>           <platformCore:pageSize>100</platformCore:pageSize>           <platformCore:totalPages>3</platformCore:totalPages>           <platformCore:pageIndex>1</platformCore:pageIndex>             <platformCore: searchId > WEBSERVICES_528736_07012008543995006307049233_d53ef4d2273b15       <platformCore: searchId >            <platformCore:recordList>            <platformCore:recordList>                  <platformCore:record internalId="4" externalId="entity-4" xsi:type="listRel:Contact">                       <listRel:entityId>john</listRel:entityId>                       <listRel:firstName>John</listRel:firstName>                         .....                     </platformCore:record>                 </platformCore:recordList>             </platformCore:searchResult>         </searchMoreWithIdResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Request for Getting the Next Page Using searchMoreWithId {#bridgehead_N27289941}

          `<soapenv:Envelope>     <soapenv:Header>         <platformMsgs:searchPreferences>             <platformMsgs:bodyFieldsOnly>true</platformMsgs:bodyFieldsOnly>             <platformMsgs:pageSize>100</platformMsgs:pageSize>         </platformMsgs:searchPreferences>         <platformMsgs:passport>             <platformCore:email>jdoe@netsuite.com</platformCore:email>             <platformCore:password><SOAP web services password></platformCore:password>             <platformCore:account>000034</platformCore:account>             <platformCore:role internalId="37"/>         </platformMsgs:passport>     </soapenv:Header>     <soapenv:Body>         <platformMsgs:searchMoreWithId>             <searchId>WEBSERVICES_528736_07012008543995006307049233_d53ef4d2273b15</searchId>             <pageIndex>2</pageIndex>         </platformMsgs:searchMoreWithId>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response for Getting the Next Page Using searchMoreWithId {#bridgehead_N27290011}

          `<soapenv:Envelope>     <soapenv:Header>         <platformMsgs:documentInfo>             <platformMsgs:nsId>WEBSERVICES_528736_07012008543995006307049233_d53ef4d2273b15</platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <platformMsgs:searchMoreWithIdResponse>             <platformCore:searchResult>          <platformCore:status isSuccess="true"/>          <platformCore:totalRecords>231</platformCore:totalRecords>          <platformCore:pageSize>100</platformCore:pageSize>          <platformCore:totalPages>3</platformCore:totalPages>          <platformCore:pageIndex>1</platformCore:pageIndex>         <platformCore: searchId > WEBSERVICES_528736_07012008543995006307049233_d53ef4d2273b15              </platformCore: searchId >                 <platformCore:recordList>                     <platformCore:record internalId="5" externalId="entity-5" xsi:type="listRel:Contact">                         <listRel:entityId>mike</listRel:entityId>                         <listRel:firstName>Mike</listRel:firstName>                         .....                     </platformCore:record>                 </platformCore:recordList>             </platformCore:searchResult>         </platformMsgs:searchMoreWithIdResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

## Java {#bridgehead_N27290081}

          `public List<Contact> searchContactsByCity(NetSuitePortType port, String city) throws Exception {     SearchResult searchResult = null;         // search result for each page     Record [] contacts = null;                    // contacts for each page     List<Contact> consolidatedResults = new ArrayList<Contact>();   // to return       // build search criteria     ContactSearchBasic contactSearch = new ContactSearchBasic();     contactSearch.setCity(new SearchStringField(city, SearchStringFieldOperator.is));       // run the search     searchResult = port.search(contactSearch);       if( searchResult.getTotalRecords() > 0 )     {         // retain the search ID  to get more pages         String sSearchId = searchResult.getSearchId();           // process first page         contacts = searchResult.getRecordList().getRecord();         for (Record contact : contacts)             consolidatedResults.add((Contact)contact);           // process remaining pages using search ID         int iNumPages = searchResult.getTotalPages();         for ( int i=2; i<=iNumPages; i++)         {             // get the page             searchResult = port.searchMoreWithId(sSearchId, i);               // process the page             contacts = searchResult.getRecordList().getRecord();             for (Record contact : contacts)                 consolidatedResults.add((Contact)contact);         }     }     return consolidatedResults; }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)
-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

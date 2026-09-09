---
id: "section_N3518731"
type: "section"
title: "Understanding Sorting in Advanced Search"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Understanding Sorting in Advanced Search"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html"
anchors: ["bridgehead_N3519137", "bridgehead_N3519252", "bridgehead_N3519619"]
sha256: "7340079ed8e21b66de0c49281df36153e639b08f3ef71d53865d0b2b068625ad"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

In SOAP web services, when you return a saved search that has sorting criteria specified in the saved search, the records are returned according to the specified _sorted by_ order. To see the _sorted by_ criteria that has been applied to a saved search, you can look at the saved search criteria in the UI.

Note:

When performing a search using SOAP web services, there is no way to specify the sort order of the returned results in the request itself.

In an ad-hoc SOAP web services search (a search in which sorted by criteria have not been set), you should be aware of the implicit sorted by order in which records are returned. This order is based on record type. Record types and the default sort by order for each record type are listed in the following table:

Note:

For a list of all records associated with each type, see [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html).

| Record Type | Default 'Sorted by' Order |
| --- | --- |
| Entities | Name (the name of the entity) |
| Actvities | Event (the title of the Event) |
| Marketing | Campaign ID Note: Promotion Code searches are sorted and returned by promotion code name. |
| Transactions | Date Created |
| Support | Number Note: Topic searches are sorted and returned by topic title. |
| File Cabinet | Name (the name of the file or folder) |
| Items | Name (the name of the item) |
| Communications (includes the Note and the Message records) | Note - sorted/returned by Author Message - sorted/returned by Message Internal ID |
| Website | Name |
| Lists | Name Note: Gift Certificate searches are sorted and returned by Name (From). |

## Request {#bridgehead_N3519137}

The SearchRequest type is used for the request. It contains the following field.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| searchRecord | SearchRecord | The SearchRecord type is an abstract type. An instance of a type that extends SearchRecord must be used-such as CustomerSearchBasic or EventSearchBasic. |

## Response {#bridgehead_N3519252}

The SearchResponse type is used for the response. It contains the following fields.

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

## Faults {#bridgehead_N3519619}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

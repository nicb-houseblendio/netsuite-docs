---
id: "section_N3514306"
type: "section"
title: "search"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html"
anchors: []
sha256: "3e739f7acff0a8e84605a0e2e4576839e1b8815297440dbc5ef564c8d7f5ef97"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The _search_ operation is used to run a search on a specific record type based on a set of criteria. You can search by defining search filter fields on the record, joined fields on an associated record, search return columns, or joined search return columns from an associated record. The results of the search can be complete records, or a select set of fields specified through search return columns.

Note that you can also use the _search_ operation to return an existing saved search. You cannot use the search operation to retrieve state values. You must use the [getAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html) operation to retrieve all state values in the system. The getAll operation will return **all** states, not the legal ones for your default country. Also note that the country and state must match on the address.

Important:

The search preferences you set in the SearchPreferences object affect the search request and response. See [SOAP Web Services Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3422061.html) for details.

Use the _search_ operation to run the following types of searches:

-   **Basic search** - Perform a search on a record type based on search filter fields that are specific to that type. See [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html).
    
-   **Joined search** - Perform a search on a record type based on search filter fields on an associated record type. See [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
    
-   **Advanced search** - Perform a search on a record type in which you specify search filter fields **and/or** search return columns or joined search columns. Using advanced search, you can also return an existing saved search. See [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html).
    

Note:

An asynchronous equivalent is available for the search operation, **asyncSearch**. For information about asynchronous request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

Not all transaction types are supported by SOAP web services searches. For the list of unsupported transactions, see [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html).

Also see the following sections for information about setting additional search filtering values and searching for custom fields:

-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
    
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
    
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
    
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
    
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
    
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
    

Important:

To go directly to search-related code samples, see [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)
-   [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

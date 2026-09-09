---
id: "section_N3522048"
type: "section"
title: "Searching for a Multi-select Custom Field"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Searching for a Multi-select Custom Field"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html"
anchors: ["bridgehead_N27268201", "bridgehead_N3522075"]
sha256: "94e41e2701b4055ce513a5b35db24c71edd2f81cc8c9ab8c22a57c3e857156de"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

In the following code sample, the results for the custom transaction field custcolcolumnname are returned.

## Java {#bridgehead_N27268201}

          `// transaction search by custom column field    TransactionSearchBasic transactionSearch = new TransactionSearchBasic();        SearchCustomFieldList searchCustomFieldList = new SearchCustomFieldList();    transactionSearch.setCustomFieldList(searchCustomFieldList);        // make the multiselectsearch    SearchMultiSelectCustomField searchMultiSelectCustomField = new SearchMultiSelectCustomField();        ListOrRecordRef listOrRecordRef = new ListOrRecordRef();    listOrRecordRef.setInternalId("3"); // the internal id of the custom list value    listOrRecordRef.setType("1"); // your custom list typeId        searchCustomFieldList.setCustomField(new SearchCustomField[]{searchMultiSelectCustomField});        // make the search expression    searchMultiSelectCustomField.setscriptId("custcolcolumnname"); //the name of the tx custom column    searchMultiSelectCustomField.setOperator(SearchMultiSelectFieldOperator.anyOf);        searchMultiSelectCustomField.setSearchValue(new ListOrRecordRef[] {listOrRecordRef});        SearchResult sr = _port.search(transactionSearch);` 
        

## C# {#bridgehead_N3522075}

          `private void searchForMultiSelectCustomField()           {             if (_isAuthenticated)             {                 _out.info("\nExecuting  search ..... \n");                 // transaction search by custom column field                 TransactionSearch transactionSearch = new TransactionSearch();                 TransactionSearchBasic transactionSearchBasic = new TransactionSearchBasic();                   //Java - the SearchCustomFieldList is not used.                  //SearchCustomFieldList searchCustomFieldList = new SearchCustomFieldList();                 //transactionSearch.setCustomFieldList(searchCustomFieldList);                 SearchMultiSelectCustomField searchMultiSelectCustomField = new             SearchMultiSelectCustomField();                   // make the search expression                //the name of the transaction custom column          searchMultiSelectCustomField.scriptId = "custbody_multi_select";                  searchMultiSelectCustomField.@operator = SearchMultiSelectFieldOperator.anyOf;                 searchMultiSelectCustomField.operatorSpecified = true;                 //custom list called colors with typei id  1, values blue - internalid 1, green - id2 etc                 //we are looking for transactions which have transaction body field           //of type multi select set to color blue                 ListOrRecordRef listOrRecordRef = new ListOrRecordRef();                 listOrRecordRef.internalId = "3";                 listOrRecordRef.typeId = "1";                   searchMultiSelectCustomField.searchValue = new ListOrRecordRef[] { listOrRecordRef };                 SearchCustomField[] searchCustomFieldList = new SearchCustomField[] {       searchMultiSelectCustomField };                   //Java                 //searchCustomFieldList.setCustomField(new SearchCustomField[]{searchMultiSelectCustomField});                 transactionSearchBasic.customFieldList = searchCustomFieldList;                 transactionSearch.basic = transactionSearchBasic;                 SearchResult searchRes = _service.search(transactionSearch);                 _out.info("\nSearch Result contains " + searchRes.totalRecords + " record(s) \n");             }             else             {                 _out.info(                     "\nCannot call  search operation  because there is no active session. " +                     "You must be first logged on before attempting to call saved search.\n");             }         }` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

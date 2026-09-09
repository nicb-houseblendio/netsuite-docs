---
id: "section_N3516862"
type: "section"
title: "Advanced Searches in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Advanced Searches in SOAP Web Services"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html"
anchors: ["bridgehead_N3517038", "bridgehead_N3517089", "bridgehead_N3517135", "bridgehead_4044945128", "bridgehead_N3517276", "bridgehead_N3517316", "bridgehead_N3517407", "bridgehead_N3517650", "bridgehead_N3517659", "bridgehead_N3517807", "bridgehead_N3517868"]
sha256: "dd522479ebc1465dcf2a084c8f348f01095c843d92e427fd51a32e0db6c99e4c"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Advanced searching in SOAP web services provides users with the ability to:

-   Perform a search that references an existing saved search. See [Reference Existing Saved Searches](#bridgehead_N3517038).
    
-   Perform a search that references an existing saved search, and then overrides existing search return columns with new search return columns. See [Specify Search Criteria and Search Return Columns](#bridgehead_N3517276).
    
-   Perform a search that references an existing saved search, and then provides additional search filter criteria (on top of the criteria already specified in the saved search). See [Specify Search Criteria and Search Return Columns](#bridgehead_N3517276).
    
-   Perform a search that specifies search criteria and search result columns. See [Specify Search Criteria and Search Return Columns](#bridgehead_N3517276).
    

The SOAP web services API includes advanced search objects for all records that have an existing search interface. To see which objects are used to run advanced searches, see [SOAP Objects used in Advanced Searches](#bridgehead_N3517407)

For advanced search code samples, see [Advanced Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520104).

In case you encounter duplicate or missing search results, ensure your search references an existing saved search in which the results are sorted by Internal ID. For more information about defining the sorting of the results, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).

The following is an XSD snippet of the listRel XSD. This sample provides a high-level overview of advanced search objects and their relationship to the basic search object < _Record_ > **Search**. In this sample, the objects Customer **SearchAdvanced**, Customer **SearchRow**, and Customer **SearchRowBasic** (not shown in sample) are considered to be advanced search objects in the SOAP web services API.

![An overview of advanced search objects.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/searchConceptsExplained.png)

Note:

For additional SOAP and code samples related to searches, see [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html), [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html), and [Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4177763939.html).

## Reference Existing Saved Searches {#bridgehead_N3517038}

Advanced search in SOAP web services lets you reference an existing saved search. Returning saved searches provides you with access to data that otherwise could not be returned in SOAP web services. For example, advanced search lets you return saved searches that include formula filters (in the search criteria) or expressions.

When working with saved searches, consider two questions from SOAP web services users:

-   [Reasons to Reference an Existing Saved Search](#bridgehead_N3517089)
    
-   [How to Reference an Existing Saved Search](#bridgehead_N3517135)
    

## Reasons to Reference an Existing Saved Search {#bridgehead_N3517089}

The following use cases illustrate possible scenarios for referencing a saved search:

-   You want to return only a subset of data from a record (in other words, data that is specified through the saved search's return columns).
    
-   Your integration application processes a set of records that are identified in a saved search. Periodically, users change the criteria of the search. By referencing a saved search ID, your code can reference their saved search. Developers do not have to change and re-test code every time the search criteria changes.
    
-   You have a complex search that compiles data from many different records. You can create a saved search in the NetSuite UI, and then reference this search in SOAP web services rather than try to code the search in SOAP web services.
    
-   You want to reference an existing saved search based on Leads, for example. You can return all the data provided in this search, and then define additional criteria for the search response. For example, you can return a Leads saved search and then provide additional criteria that returns the leads from this search created with today's date. In other words, if you reference a saved search and add any filter criteria to the search request, the additional criteria will be conjunctive with the saved search criteria.
    

## How to Reference an Existing Saved Search {#bridgehead_N3517135}

First you must obtain the saved search ID. You can do so through the UI by going to Lists > Search > Saved Searches. The saved search ID appears in the ID column.

You can also use the [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) operation to programmatically retrieve a list of saved search IDs for a specific record type. Note that this operation does nothing more than return a list of saved search IDs on a per-record-type basis (for example, all saved search IDs for the customer record type).

You can then use the search() operation, along with the < _Record_ > **SearchAdvanced** object to return the details of the saved search. The following is a example that shows how to instantiate the CustomerSearchAdvanced object and specify a savedSearchId to return.

          `// create search object CustomerSearchAdvanced customerSearch = new CustomerSearchAdvanced();   //set saved search id customerSearch.savedSearchId="100";   // perform the search NetSuiteService nss = new NetSuiteService();  SearchResult result = nss.search(customerSearch);` 
        

For more detailed samples, see [Advanced Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520104).

## Usage Notes {#bridgehead_4044945128}

-   Only one saved search can be referenced as part of the search call.
    
-   If you reference a saved search that contains search functions, you _will_ get the results back. However, you cannot _create_ an advanced search that uses search functions. Creating a search in SOAP web services that uses search functions is not currently supported.
    
-   If you reference a saved search for which you do not have permission, the exception is ignored and fields have no value (are not in the SOAP response at all).
    
-   If you reference a saved search that contains summary results, you will get the following error:
    
    We cannot return search columns for summary saved search < _saved search ID_ >
    

## Specify Search Criteria and Search Return Columns {#bridgehead_N3517276}

Similar to a basic search, an advanced search allows you search against a specific record type using the fields on that record as search filters. In addition, you can **also** specify a set of search return columns or joined columns to return.

This kind of advanced search is useful for retrieving only the record data you need rather than the contents of an entire record.

Advanced searches work well, for example, for users who may have a mobile client that needs to display only the name, phone number, and email address of their sales rep contact. Rather than returning all of the data on a contact record, users can create an advanced search that pulls only the relevant information. They are no longer required to download the entire record.

For advanced search code samples that show how to specify both search criteria and search return columns, see [Advanced Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520104).

## Search Return Columns {#bridgehead_N3517316}

The following figures show the UI equivalent of an advanced search that includes search return columns.

1.  First, specify the basic search criteria on the Criteria subtab (in this example all customers that have a company name starting with the letter A).
    
    ![An advanced search that includes search return columns.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/UISearchResultColumn3.png)
2.  Next, click the Results subtab to define the search return columns. When your search is executed, your search response will return only the company name, phone, and contact name of all customers whose company starts with the letter A.
    
    ![The results tab of a search in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/UISearchResultColumns5.png)

The following figure shows the results of the search. Only the relevant data are returned.

![The results of a search in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/UISearchResultColumns4.png)

## SOAP Objects used in Advanced Searches {#bridgehead_N3517407}

The following summarizes the objects used in different types of advanced searches. For additional details, see [Advanced Search Objects Explained](#bridgehead_N3517650) and [Advanced Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520104).

-   To perform a search that specifies search filter criteria and search result columns, use:
    
    1.  < _Record_ > **Search**
        
    2.  < _Record_ > **SearchBasic**
        
    3.  < _Record_ > **SearchRow**
        
    4.  < _Record_ > **SearchRowBasic**
        
-   To perform a search that references an existing saved search, use:
    
    < _Record_ > **SearchAdvanced**
    
-   To perform a search that references an existing saved search, and then overrides existing search return columns with new search return columns, use:
    
    1.  < _Record_ > **SearchAdvanced**
        
    2.  < _Record_ > **SearchRow**
        
    3.  < _Record_ > **SearchRowBasic**
        
-   To perform a search that references an existing saved search, and then provides additional search filter criteria (that is in _addition_ to the criteria already specified in the saved search), use:
    
    1.  < _Record_ > **SearchAdvanced**
        
    2.  < _Record_ > **Search**
        
    3.  < _Record_ > **SearchBasic**
        

## Advanced Search Objects Explained {#bridgehead_N3517650}

## The < Record >SearchAdvanced object contains: {#bridgehead_N3517659}

-   a _criteria_ element - references the < _Record_ > **Search** object through which you specify standard search field criteria. (See [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html) for details on the < _Record_ >Search object.)
    
-   _a columns_ element - references the < _Record_ > **SearchRow** object through which you specify a set of search result columns to return in the response.
    
-   a _savedSearchId_ attribute - references the saved search internal ID (for example, 57, 99, 63).
    

Note:

If the Show Internal ID preference is enabled in your NetSuite account, the saved search internal ID appears in the **Internal ID** column in a saved search list. Programmatically, you can use [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) to obtain a list of saved search internal IDs for a specific record type.

-   a _savedSearchScriptId_ attribute - references a custom saved search ID (for example, customsearch\_mySpecialSearch).
    

Note:

If the Show Internal ID preference is enabled in your NetSuite account, the saved search ID appears in the **ID** column in a saved search list.

Important:

You cannot use [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) to return a list of custom saved search IDs; only the system-defined internal IDs (57, 99, 63, etc.) will be returned.

The XSD sample below shows the CustomerSearchAdvanced object:

          `<complexType name=" CustomerSearchAdvanced ">    <complexContent>       <extension base="platformCore:SearchRecord">          <sequence>             <element name=" criteria " type="listRel:CustomerSearch" minOccurs="0"/>             <element name=" columns " type="listRel:CustomerSearchRow" minOccurs="0"/>             </sequence>             <attribute name=" savedSearchId " type="xsd:string"/>             <attribute name=" savedSearchScriptId " type="xsd:string"/>          </extension>` 
        

## The < Record >SearchRow object contains: {#bridgehead_N3517807}

-   a _basic_ element - references the < _Record_ > **SearchRowBasic** object, which specifies available search return columns and column joins for _that_ record type.
    
-   <xxx>Join elements - references the < _Record_ > **SearchRowBasic** object, which specifies search return columns and column joins for the _associated_ record type.
    

The XSD below shows a snippet of the CustomerSearchRow object:

          `<complexType name=" CustomerSearchRow ">    <complexContent>       <extension base="platformCore:SearchRow">            <sequence>              <element name=" basic " type="platformCommon:CustomerSearchRowBasic"                minOccurs="0"/>              <element name=" callJoin " type="platformCommon:PhoneCallSearchRowBasic"             minOccurs="0"/>              <element name=" campaignResponseJoin "type="platformCommon:CampaignSearchRowBasic"             minOccurs="0"/>          <element name=" caseJoin " type="platformCommon:SupportCaseSearchRowBasic"             minOccurs="0"/>             ......           </sequence>       </extension>    </complexContent> </complexType>` 
        

## The < Record >SearchRowBasic object contains: {#bridgehead_N3517868}

-   search result column elements - use to define specific column names in your response.
    

The next snippet shows the CustomerSearchRowBasic object, which, like ALL < _Record_ > **SearchRowBasic** objects, resides in the platformCommon XSD. This object lists all available search return columns for the Customer record.

          `<complexType name=" CustomerSearchRowBasic ">         <sequence>             <element name=" accountNumber " type="platformCore: SearchColumnStringField " minOccurs="0"       maxOccurs="unbounded"/>             <element name=" address " type="platformCore: SearchColumnStringField " minOccurs="0"       maxOccurs="unbounded"/>             <element name=" addressee " type="platformCore: SearchColumnStringField " minOccurs="0"       maxOccurs="unbounded"/>             <element name=" addressLabel " type="platformCore: SearchColumnStringField " minOccurs="0"       maxOccurs="unbounded"/>            ...          </sequence>     </complexType>` 
        

Note that all search return columns reference SearchColumn< _xxx_ >Field objects. See [Search Column Custom XML Schema Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html#bridgehead_N3468333) for definitions of each search column object.

Important:

When executing an advanced search, you can set the SearchPreferences. _returnSearchColumns_ preference to TRUE to ensure that only search return columns are returned in a search. An error is thrown if _returnSearchColumns_ is set to TRUE and you have not specified search return columns in your request. (Note that you will **not** receive an error if you are using advanced search functionality to return a **saved search** that already includes search return columns.)

Note:

Also note that in an advanced search, the _bodyFieldsOnly_ preference is ignored.

The default value for _returnSearchColumns_ is TRUE.

          `<complexType name="SearchPreferences">  <sequence>   <element name="bodyFieldsOnly" minOccurs="0" type="xsd:boolean" default="true"/>   <element name=" returnSearchColumns " minOccurs="0" type="xsd:boolean"       default="true"/>   <element name="pageSize" minOccurs="0" type="xsd:int"/>  </sequence> </complexType>` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

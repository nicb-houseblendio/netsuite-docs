---
id: "section_N3518157"
type: "section"
title: "Setting the anyof, mine, or myteam Filtering Values"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Setting the anyof, mine, or myteam Filtering Values"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html"
anchors: ["bridgehead_N3518334", "bridgehead_3819309268"]
sha256: "f0d52c52dbd9f90323d2ab56584904f93ff18f296f2bec5c106bd64d84cf4ff4"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

In SOAP web services, you can further define your search using the following filtering values:

| Filter | Note |
| --- | --- |
| @NONE@ | Equates to _anyof_ (see [Filtering Lists that Contain Null Values](#bridgehead_N3518334)) or _unassigned_ depending on the field. |
| @CURRENT@ | Equates to _mine_. For example, use this filter to return all of your own events. |
| @HIERARCHY@ | Equates to _my team_. For example, use this filter on a salesRep field for customer records. If you have previously defined the members of your sales team, using the @HIERARCHY@ filter will return only the customers that have worked with members of your sales team. |

The following provides a SOAP sample for finding _my_ events.

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <searchRecord xsi:type="ns1:CalendarEventSearchBasic"    xmlns:ns1="urn:common_2017_1.platform.webservices.netsuite.com">       <ns1:attendee operator="anyOf" xsi:type="ns2:SearchMultiSelectField"    xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">          <ns2:searchValue internalId="@CURRENT@" xsi:type="ns2:RecordRef"/>       </ns1:attendee>   </searchRecord>   </search>` 
        

## Filtering Lists that Contain Null Values {#bridgehead_N3518334}

For select lists or multi selects which can have a null value, the UI supports the search criteria on these list type fields as 'None Of' '-None-', which essentially means not 'Any Of' all list options. Such a search would result in all records which do NOT have this list type field as null. To accomplish this 'None Of' '-None-' search you need to set the internalId of the search key to '@None@'.

## Example {#bridgehead_3819309268}

To search for Customers which have a Partner associated with them in NetSuite, the SOAP would look as below for the 'Partner field not null' part:

          `<ns3:partner operator="noneOf"> <ns8:searchValue internalId="@NONE@" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/> </ns3:partner> <ns3:customFieldList>` 
        

Java code to generate this SOAP would be:

          `// Adding search criteria where Partner is not null RecordRef[] noPartner = new RecordRef[1]; noPartner[0] = new RecordRef(); noPartner[0].setInternalId("@NONE@"); SearchMultiSelectField partner = new SearchMultiSelectField(); partner.setOperator(SearchMultiSelectFieldOperator.noneOf); partner.setSearchValue(noPartner); custSearch.setPartner(partner);` 
        

C# code to generate this SOAP would be:

          `// Adding search criteria where Partner is not null  RecordRef[] noPartner = new RecordRef[1];  noPartner[0] = new RecordRef();  noPartner[0].internalId = "@NONE@";  SearchMultiSelectField partner = new SearchMultiSelectField();  partner.@operator = SearchMultiSelectFieldOperator.noneOf;  partner.searchValue = noPartner;  custSearch.partner = partner;` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

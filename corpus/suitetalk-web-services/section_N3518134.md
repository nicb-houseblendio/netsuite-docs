---
id: "section_N3518134"
type: "section"
title: "Setting Valid Search Values"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Setting Valid Search Values"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html"
anchors: []
sha256: "14180dd463d27e250279222e9edc9bcb351e420b6db3527b0487223ea9edefcb"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Prior to the 2008.2 endpoint, if you performed a search that included an invalid search enum filter value, you would generally still get records returned in your search. For example, if you performed a search for all customers with the Country enum search value set to "United States" (rather than the supported enum value \_unitedStates), you would still get results from your search. Although the value "United States" was not recognized, you continued to get customer records. Note, however, the search results returned ALL customers in the system, since the value 'United States' was invalid.

Starting with the 2008.2 endpoint, instead of ignoring any invalid search enum values, and still returning search results, NetSuite now returns 0 records and a no-match warning. Therefore, when setting search values, be sure to use the values defined in the schema.

The following is an example of what is now returned if invalid values are specified:

          `<platformCore:searchResult xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformCore:status isSuccess="true"> <platformCore:statusDetail type="WARN"> <platformCore:code>WARNING</platformCore:code> <platformCore:message>The field country's enum value <United States> is invalid for this search.</platformCore:message> </platformCore:statusDetail> </platformCore:status> <platformCore:totalRecords>0</platformCore:totalRecords> <platformCore:totalPages>0</platformCore:totalPages> <platformCore:searchId>WEBSERVICES_MSTRWLF_10212008563721605896842316_60315faa132ad</platformCore:searchId> <platformCore:searchRowList/>` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

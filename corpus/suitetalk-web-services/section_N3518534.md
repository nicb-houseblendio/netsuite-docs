---
id: "section_N3518534"
type: "section"
title: "Searching by lastModifiedDate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Searching by lastModifiedDate"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html"
anchors: ["bridgehead_N27253171", "bridgehead_N27253271"]
sha256: "eb7fe2bc11e0996ea29fdf1d39b33c7e056efae91197768395eaac45f4716f73"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

This sample shows how to create a customer, and then search for the customer that was created based on a specific time frame. In this case, the sample uses the lastModifiedDate field to search 'within' a couple of seconds before the customer was created and then a minute after. The search returns the record that was previously created.

## Java {#bridgehead_N27253171}

          `Customer c = (Customer) new TestCustomer().createMinimalRecord(); Calendar timeFrom = Calendar.getInstance(); WriteResponse wr = sessMgr.getPort().add(c); outputResult(wr.getStatus().isIsSuccess());   Calendar timeTo = Calendar.getInstance(); timeTo.setTimeInMillis(timeTo.getTimeInMillis() + 60000);   CustomerSearch cs = new CustomerSearch(); CustomerSearchBasic csb = new CustomerSearchBasic(); SearchDateField sdf = new SearchDateField(); sdf.setOperator(SearchDateFieldOperator.within); sdf.setSearchValue(timeFrom); sdf.setSearchValue2(timeTo); csb.setLastModifiedDate(sdf);   cs.setBasic(csb);   SearchResult sr = sessMgr.getWrappedPort().search(cs, this);` 
        

## SOAP {#bridgehead_N27253271}

          `<searchRecord xsi:type="ns1:CustomerSearch"     xmlns:ns1="urn:relationships_2017_1.lists.webservices.netsuite.com">                <ns1:basic xsi:type="ns2:CustomerSearchBasic"    xmlns:ns2="urn:common_2017_1.platform.webservices.netsuite.com">                   <ns2:lastModifiedDate operator="within" xsi:type="ns3:SearchDateField"    xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">                      <ns3:searchValue xsi:type="xsd:dateTime">2007-02-10T00:16:17.750Z</ns3:searchValue>                      <ns3:searchValue2 xsi:type="xsd:dateTime">2007-02-10T00:17:53.015Z</ns3:searchValue2>                   </ns2:lastModifiedDate>                </ns1:basic>             </searchRecord>` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

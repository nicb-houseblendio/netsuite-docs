---
id: "section_N3516345"
type: "section"
title: "Joined Searches in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Joined Searches in SOAP Web Services"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html"
anchors: ["bridgehead_N3516410", "bridgehead_N3516482", "bridgehead_N3516550", "bridgehead_N3516664"]
sha256: "a4d7ee60eae8d8bb10de4e370ddfaa537754ed953c0bef899a41eddbb296bdd7"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

See the following topics to learn how to run a joined search in NetSuite using SOAP web services:

-   [Joined Searches](#bridgehead_N3516410)
    
-   [SOAP Objects Used in a Joined Search](#bridgehead_N3516482)
    
-   [Joined Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520026)
    

## Joined Searches {#bridgehead_N3516410}

A joined search allows you search against a specific record type using the fields on an associated record as search filters. In the UI, you can identify which associated records provide joined filter criteria by first navigating to a record's search interface. For example, for the Customer search interface, go to _Lists > Relationships > Customers > Search_.

Check the Use Advanced Search box and wait for the page to update. Then scroll through the Filter dropdown list. Joined search records are indicated by the record name followed by an ellipsis (....). Search fields from any of the records listed (that are also currently exposed in SOAP web services) can be included in the search criteria.

![An example of a joined search in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/joinedSearch.png)

Note:

For a list of SOAP web services-supported records, see [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html).

## SOAP Objects Used in a Joined Search {#bridgehead_N3516482}

To perform a joined search in which you use search filter criteria from an associated record, use:

1.  < _Record_ > **Search**
    
2.  < _Record_ > **SearchBasic**
    

For more details, see [Joined Search Objects Explained](#bridgehead_N3516550) and [Joined Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520026).

## Joined Search Objects Explained {#bridgehead_N3516550}

In SOAP web services, all search joins are listed in the < _Record_ > **Search** object. For example, to find available search joins for the Contact or Employee record, see the [ContactSearch](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) and [EmployeeSearch](https://webservices.netsuite.com/xsd/lists/v2025_2_0/employees.xsd) XSDs, respectively.

The snippet below shows the CustomerSearch object, which includes < _xxx_ > **Join** elements. These elements reference search criteria available from other SOAP-supported records.

          `<complexType name=" CustomerSearch ">         <complexContent>             <extension base="platformCore:SearchRecord">                 <sequence>                     <element name="basic" type="platformCommon:CustomerSearchBasic" minOccurs="0"/>                     <element name=" callJoin " type="platformCommon: PhoneCallSearchBasic " minOccurs="0"/>                     <element name=" campaignResponseJoin " type="platformCommon: CampaignSearchBasic "          minOccurs="0"/>                     <element name=" caseJoin " type="platformCommon: SupportCaseSearchBasic " minOccurs="0"/>       .....                        </sequence>             </extension>         </complexContent>     </complexType>` 
        

In this case, all search filter criteria from the PhoneCallSearchBasic, CampaignSearchBasic, and SupportCaseSearchBasic objects are available to the Customer record as joined search filters. Note that all < _Record_ > **SearchBasic** objects in NetSuite SOAP web services are defined in the [platformCommon](https://webservices.netsuite.com/xsd/platform/v2025_2_0/common.xsd) XSD.

For a code sample of a joined search, see [Joined Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520026).

Important:

Only fields on **SOAP-supported** records can be specified as filter criteria for a joined search request. For a list of SOAP-supported records, see [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html).

## Returning an Associated Joined List of Records {#bridgehead_N3516664}

Using a combination of joined search and the internalId list on each record, you can retrieve a list of records for an associated list of records. For example, you can retrieve a list of contacts for a specific list of customers. To do this, you must first retrieve the desired list of internalIds for the record you need to retrieve by, and then submit that list in a joined search query to retrieve the associated list.

See [Joined Search Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3520026) for an example of a joined search which uses a list of records.

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Search-Related Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

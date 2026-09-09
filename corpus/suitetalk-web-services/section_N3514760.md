---
id: "section_N3514760"
type: "section"
title: "Basic Searches in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Basic Searches in SOAP Web Services"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html"
anchors: ["bridgehead_N3514825", "bridgehead_N3514890", "bridgehead_N3514958", "bridgehead_1536825462"]
sha256: "d935f78d1fd51e7038a48d6d5e31689cdbc0782b99e47aa2b81c35e771535ada"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

See the following topics to learn how to run a basic search in NetSuite using SOAP web services:

-   [Basic Searches](#bridgehead_N3514825)
    
-   [SOAP Objects Used in a Basic Search](#bridgehead_N3514890)
    
-   [Basic Search Code Sample](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3519940)
    

## Basic Searches {#bridgehead_N3514825}

A basic search lets you search records of a specific type using the fields on that record as search filters. The following figure shows the UI equivalent of a basic Customer search. Start by going to Lists > Relationships > Customers > Search, and ensure that the Use Advanced Search box is not checked. You can specify one or more field values to use as filters for search results.

![A basic customer search in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/SimpleSearch.png)

In a basic search, field criteria are the **only** values you set. You cannot specify search return columns. In SOAP web services, specifying search return columns is the equivalent of performing an advanced search. (See [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html) for details.)

In the example of a basic Customer search (see previous figure), the results returned include the record ID of every customer that has the Category field set to _From Advertisement_ and the Status field set to _Customer-Closed Won_. Note that **ALL** the other data associated with these specific customer records are returned as well. Therefore, in SOAP web services a basic search tends to increase the search response time.

## SOAP Objects Used in a Basic Search {#bridgehead_N3514890}

To perform a basic search in which you specify search filter criteria only, use:

1.  < _Record_ > **Search**
    
2.  < _Record_ > **SearchBasic**
    

For more details, see [Basic Search Objects Explained](#bridgehead_N3514958) and [Basic Search Code Sample](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3519940).

## Basic Search Objects Explained {#bridgehead_N3514958}

In SOAP web services, any record that supports search has a corresponding < _Record_ > **Search** object, which contains a _basic_ element. The _basic_ element references a < _Record_ > **SearchBasic** object, which defines all available search criteria (filter fields) specific to that record type.

The XSD snippet below shows the CustomerSearch object. The _basic_ element references the CustomerSearchBasic object, which defines all available search criteria for the Customer record.

          `<complexType name=" CustomerSearch ">         <complexContent>             <extension base="platformCore:SearchRecord">                 <sequence>                     <element name=" basic " type="platformCommon: CustomerSearchBasic " minOccurs="0"/>                     <element name="callJoin" type="platformCommon:PhoneCallSearchBasic" minOccurs="0"/>                     <element name="campaignResponseJoin" type="platformCommon:CampaignSearchBasic"          minOccurs="0"/>                  .....                        </sequence>             </extension>         </complexContent>     </complexType>` 
        

Note:

< _Record_ > **Search** objects reside in the same XSD as their corresponding record objects. In this case, both the Customer and CustomerSearch objects reside in the [listRel](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD. Also note that the CustomerSearch object, like all < _Record_ > **Search** objects, provide available search joins for that record type. For information about joined searches, see [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html).

This snippet shows the CustomerSearchBasic object. All < _Record_ > **SearchBasic** objects are defined in the [platformCommon](https://webservices.netsuite.com/xsd/platform/v2025_2_0/common.xsd) XSD. This sample shows four of the available fields (accountNumber, address, addressee, addressLabel) that can be used as search criteria on the Customer record.

          `<complexType name=" CustomerSearchBasic ">       <complexContent>    <extension base="platformCore:SearchRecord">       <sequence>         <element name=" accountNumber " type="platformCore:SearchStringField" minOccurs="0" />          <element name=" address " type="platformCore:SearchStringField" minOccurs="0" />         <element name=" addressee " type="platformCore:SearchStringField" minOccurs="0" />          <element name=" addressLabel " type="platformCore:SearchStringField" minOccurs="0" />                 ...      </sequence>          </extension>    </complexContent> </complexType>` 
        

Important:

< _Record_ > **SearchBasic** does not work for subrecords.

For a code sample of a basic search, see [Basic Search Code Sample](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html#bridgehead_N3519940).

## Basic Search Behavior with User Event Scripts and Workflows {#bridgehead_1536825462}

If the bodyFieldsOnly preference is set to false, a basic search triggers user event scripts and workflows. To avoid triggering user event scripts and workflows while using basic search, do one of the following:

-   Set the bodyFieldsOnly preference to true. For information about this preference, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).
    
-   Set the runServerSuiteScriptAndWorkflowTriggers preference to false. For information about this preference, see [runServerSuiteScriptAndWorkflowTriggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_4629750371).
    

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
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

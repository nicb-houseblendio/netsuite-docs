---
id: "section_N2628302"
type: "section"
title: "Declare Attribute Tags for Tags Within Tags"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Declare Attribute Tags for Tags Within Tags"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html"
anchors: ["bridgehead_N2628325", "procedure_N2628362"]
sha256: "43eb3bc39ee830758b9a9ffc3b05766f70e248fa178a96db4fb08f4196f68eb2"
---

You must use the declareAttribute tag when you add an attribute tag in a field and use a site template to show that field on your website. The NetSuite tag replacement engine needs the declareAttribute tag to show embedded tags.

Behind the scenes, the NetSuite tag replacement engine scans each page twice to find the attributes in your custom HTML and ensure that they show up correctly on your web pages. On the first scan, it finds the attributes used in each tag but skips over the embedded tags. On the second pass, it replaces all the tags on the page, including embedded ones. Use the declareAttribute tag to point to embedded tags.

## Using declareAttribute Tags {#bridgehead_N2628325}

You can use declareAttribute tags in item/category templates or Hosted web pages.

For example, you may create an item drilldown template that contains an attribute tag for the detailed description field on an item record:

          `<%=getCurrentAttribute('item','storedetaileddescription')%>` 
        

The HTML in the detailed description field may contain an attribute tag for the item name:

          `<%=getCurrentAttribute('item','storedisplayname')%>` 
        

To display all the information in the detailed description field from the item record, you must use the declareAttribute tag for the item name in front of the Attribute tag for the detailed description field. For example:

          `<%=declareCurrentAttribute('item','storedisplayname')%><%=getCurrentAttribute('item', 'storedetaileddescription')%>.` 
        

Use the appropriate declareAttribute tag listed below to ensure the embedded tag is rendered properly in your site. Note that the declareAttribute tag takes the same parameters as its corresponding Attribute tag.

## Syntax: {#procedure_N2628362}

-   **declareAttribute**
    
                  `<%=declareAttribute('item',7,'storedisplayname')%><%=getAttribute('item','storedetaileddescription')%>.` 
                
    
-   **declareCurrentAttribute**
    
                  `<%=declareCurrentAttribute('item','storedisplayname')%><%=getCurrentAttribute('item',    'storedetaileddescription')%>.` 
                
    
-   **declareRecordAttribute**
    

          `<%=declareRecordAttribute('24',34,'custrecord80')%><%=getRecordAttribute('24',34,'custrecord85')%>` 
        

### Related Topics

-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)
-   [Using the Server-Side Include Tag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html)
-   [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html)
-   [Tags for Information Unavailable on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634674.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

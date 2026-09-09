---
id: "section_N2616759"
type: "section"
title: "Creating Attribute Tags for Custom Records and Custom Fields"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Custom Records and Custom Fields"
parent: "section_N2615537"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html"
anchors: ["bridgehead_N2616779", "bridgehead_N2616869"]
sha256: "0a0bafb84e7e6a31f4cf2638ee32852722556be3928617d6aaab1b296679dbaf"
---

You can display information from custom records and custom fields on your website by using attribute tags in item/category templates and in the HTML you write for your site themes in Site Builder.

## Creating Attribute Tags for Custom Fields {#bridgehead_N2616779}

Display information from custom fields on item and customer records by using the custom field ID as the attribute.

For example, to include information from an item custom field with ID custitem1, you can use the following attribute tag:

          `<%=getCurrentAttribute('item','custitem1')%>` 
        

You can find the ID for a field in the following places:

-   **attribute** - Go to _Customization > Lists, Records, & Fields > Record Types_. Click the name of the record type. The attribute is listed on the Fields subtab, in the ID column.
    
-   Custom fields on customer records - Go to _Customization > Lists, Records, & Fields > Entity Fields_.
    

## Creating RecordAttribute Tags for Custom Records {#bridgehead_N2616869}

Display information from custom fields on custom records using the custom record type ID, the ID for the custom record, and the custom field on the record as the attribute.

To display information from a custom record, use the following syntax for the tag:

          `<%=getRecordAttribute('recordTypeID',id,'attribute')%>` 
        

-   **recordTypeID** - Open a custom record of the type you want to use. On the Custom record Type page, note the value for **Internal ID**. The number referenced here is the recordTypeID for all custom records of this type.
    
-   **id** - Open the list of records for the custom record type you want to use. The ID for each unique record is listed in the **ID Column**.
    
-   **attribute** - Go to _Customization > Lists, Records, & Fields > Record Types_. Click the name of the record type. The attribute is listed on the Fields subtab, in the ID column.
    

### Related Topics

-   [Using Attribute Tags in Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616422.html)
-   [Using Web Site Tags in Hosted Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)
-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

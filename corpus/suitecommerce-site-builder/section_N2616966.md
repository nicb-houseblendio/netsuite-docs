---
id: "section_N2616966"
type: "section"
title: "Creating Attribute Tags for Standard Records"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records"
parent: "section_N2615537"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html"
anchors: ["procedure_N2616990", "bridgehead_3823930919", "bridgehead_3823946940", "bridgehead_3823947633", "bridgehead_3830784665"]
sha256: "8c49d454857b6f3937c928345ed701c278b04dfb4ec182ad58403c3df15e061e"
---

Attribute tags are typically made up of two components - record type and attribute.

The attribute can be any information available on a NetSuite record or a field on a record that contains the information. For a list of record types and their corresponding tag components, see [Using recordType in Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html#bridgehead_N2615664).

## Sample Attribute Tags {#procedure_N2616990}

Attribute tags are commonly used for displaying the default value in a field on a certain record type, such as item records or customer records. You can also display a value in a field on a specific record, or specify the information for display. Use the information below to create attribute tags for your own website.

-   [Displaying the Default Value from a Field on a Record](#bridgehead_3823930919)
    
-   [Displaying Information from a Specific Record](#bridgehead_3823946940)
    
-   [Specifying Information for Display](#bridgehead_3823947633)
    

## Displaying the Default Value from a Field on a Record {#bridgehead_3823930919}

You can use an attribute tag to display information from the current applicable record. This can be an item being viewed in the web store or data from the customer record assigned to the same customer currently logged in. Note the following syntax:

          `<%=getCurrentAttribute('recordType','attribute','defaultValue')%>` 
        

-   The following tag shows the store display name of the item being viewed in the site:
    
                  `<%=getCurrentAttribute('item','storedisplayname')%>` 
                
    
-   The following tag displays the name of the customer currently logged in:
    
                  `<%=getCurrentAttribute('customer','entityID','Guest')%>` 
                
    

Note:

Customers must be logged in to display personalized information. NetSuite recommends using default values for all customer tags.

## Displaying Information from a Specific Record {#bridgehead_3823946940}

Use an internal ID in the tag to refer to a specific record of any type that supports current attribute tags. In this way, you can display values from fields on specific records regardless of the page being viewed on the website. Note the following syntax:

          `<%=getAttribute('recordType',id,'attribute')%>` 
        

The internal ID is found in the URL of the record page in your account. For more information, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)

For example, to display the value in the Store Display Name field on item ID 7, use this attribute tag:

          `<%=getAttribute('item',7,'storedisplayname')%>` 
        

## Specifying Information for Display {#bridgehead_3823947633}

You can add the nlignorefamily parameter to an Attribute tag to omit data from the record 'family.' The nlignorefamily flag skips data from record types other than the one specified in the tag. For example, when you're working with customer records, you can exclude data from other related records, like partner records.

In the sample attribute tag below, an empty string is returned if a customer record doesn't exist. If the nlignorefamily flag isn't there, a partner email or an email from another related record is shown.

          `<%=getCurrentAttribute('customer','email', '', 'nlignorefamily')%>` 
        

Note that you can change the third parameter in the sample, from an empty string to any string you want to display when a customer record does not exist.

You can use the nlescapehtml parameter to specify that you want a response formatted for HTML. For example:

          `<%=getCurrentAttribute('request','querystring','','nlescapehtml')%>` 
        

Note:

When using request attributes in you r attribute tags, also use nlescapehtml to avoid cross-site scripting vulnerabilities.

## Records that Support Attribute Tags {#bridgehead_3830784665}

Use the links below to see a complete list of attributes for each record type:

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
    
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
    
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
    
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
    
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
    
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
    
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
    
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
    
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
    

### Related Topics

-   [Using Attribute Tags in Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616422.html)
-   [Using Web Site Tags in Hosted Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html)
-   [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html)
-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

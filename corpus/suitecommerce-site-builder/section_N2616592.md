---
id: "section_N2616592"
type: "section"
title: "Using Web Site Tags in Hosted Files"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Using Web Site Tags in Hosted Files"
parent: "section_N2615537"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html"
anchors: []
sha256: "00e698578b1c966c16cc152ba5de3e5ad40f692bd5124501c7eb0f9558d63986"
---

You can use the NetSuite Web Site Tags to build custom pages for your site that have a similar look and feel to other non-custom areas of your site. You can also display information from item and customer records in your NetSuite account on your website. Note that Web Site Tags are not supported in SuiteCommerce Advanced.

Use the following format to insert information from a record in your account:

          `<%=getAttribute('recordtype',id,'attribute')%>` 
        

For example, you can use the code sample below to display an item in your HTML website. Note that the internal ID for the item record must be referenced in the Attribute tag:

          `<h2><%=getAttribute('item',10,'itemid')%><%=getAttribute('item',10,'stockstatusmessagehtml')%></h2> <br><br><%=getAttribute('item',10,'storedetaileddescription')%> <br><br> Only<%=getAttribute('item',10,'salespricehtml')%> <br><br><br> <table> <td><%=getAttribute('item',10,'addtocarthtml')%></td> <td><%=getAttribute('item',10,'storedisplayimagehtml')%></td> </table>` 
        

The internal ID is found in the URL of the record page in your account. For more information, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)

See [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html) to view a chart including the record types attributes you can use.

Important:

Web site tags are not substituted in hosted files greater than 2 MB in size.

### Related Topics

-   [Using Attribute Tags in Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616422.html)
-   [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)
-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

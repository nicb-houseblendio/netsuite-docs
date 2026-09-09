---
id: "section_N2629027"
type: "section"
title: "Using the Server-Side Include Tag"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Using the Server-Side Include Tag"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html"
anchors: ["procedure_N2629069"]
sha256: "5e9d5d6835d470d62b8164d3bed521a9dd4880644104d9ae8090519bfe1b6e87"
---

You can use the server-side Include tag in your item or category templates and in HTML pages hosted in your NetSuite file cabinet.

The server-side Include tag helps you reuse common HTML code across your site, like a page header, footer, or navigation menu. When it's time to update that code, you don't have to change every template and HTML file. Update the file used in the Include tag.

Using Include tags, instead of repeating blocks of HTML can help your website pages load faster. For more information, see [Best Practices for Website Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2461527.html).

For example, if several pages on your site use the same HTML for a related items list template you customized, just upload a text or HTML file with the code to the right folder to your NetSuite file cabinet. Then use the Server-Side Include tag in the item drilldown template to pull in the HTML in the hosted file. When you need to update the HTML for your related items list, edit the hosted file.file.

Important:

Web Site tags are not supported in SuiteCommerce Advanced websites.

#### To use the Server-Side Include tag: {#procedure_N2629069}

1.  Create a text or HTML file for the code you call in other site pages.
    
2.  Upload this file to the appropriate folder in your NetSuite File Cabinet.
    
3.  Now, you are ready to create your Server-Side Include tag. This is the syntax:
    
                    `<%=include('URL')%>` 
                  
    
    Replace `URL` with the site-relative URL of your HTML or text file. This must be a quoted string. This field is case sensitive. For example:
    
                    `<%=include('/list.html')%>` 
                  
    
4.  Place this tag in the hosted pages of your site, or in an item/category template where you want the common piece of HTML code to appear.
    

Note:

Currently, you cannot use Server-Side Include tags in site theme templates.

### Related Topics

-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)
-   [Declare Attribute Tags for Tags Within Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html)
-   [Defining Custom Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html)
-   [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html)
-   [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

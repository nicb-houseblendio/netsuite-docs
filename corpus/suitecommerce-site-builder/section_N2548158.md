---
id: "section_N2548158"
type: "section"
title: "Creating Customer-Facing Messages from Scriptable Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Creating Customer-Facing Messages from Scriptable Cart"
parent: "chapter_N2545000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html"
anchors: ["procedure_N2548418"]
sha256: "73d9d5f898d9957913e2677b63afe531a6ac3507a9127fbf9129fd3d5ab20cc4"
---

Use Web Site Tags with Scriptable Cart to create messages that display in your web store. The content for your message is captured in a custom field, or any field on your Scriptable Template sales order, and then displayed on your site wherever you use Scriptable Cart Message Tags.

| Scriptable Cart Message Tag | Notes |
| --- | --- |
| <%=getField( **fieldname** )%> | 
-   Replace **fieldname** with the ID of a custom field or any field on your Scriptable Template sales order.
-   Include this tag in custom HTML and in scripts to create messages that display on website pages.

 |
| <%=setField( **fieldname, value** )%> | 

-   Replace **fieldname** with the ID of a custom field or any field on your Scriptable Template sales order.
-   Use the **value** parameter to designate a value for the custom field where appropriate.
-   Use the setField() tag with the getField() tag in custom HTML and in scripts to create popups and alerts.

 |
| <%=getCartLineField( **fieldname** )%> | 

-   Replace **fieldname** with the ID of a custom field.
-   Can only be used in the **Cart Line Message** field in site themes.

 |

You can combine these tags to communicate with your customers using either page-level or cart-level messages. The `getField()` and `setField()` tags display messages on any page of your site. The `getCartLineField()` tag displays a message on the cart page, or on a specific line in the shopping cart.

You can also customize an error message triggered by a failure in the validateLine event. For more information, see [Custom Error Messages for ValidateLine Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549673.html).

#### To create a Scriptable Cart message, follow these general steps: {#procedure_N2548418}

1.  Create a custom field for displaying your message, or for page-level messages, choose an existing field from your Scriptable Template sales order.
    
2.  Customize your Scriptable Template sales order form to include the custom field for the message. Or, if you choose to use an existing field, note the field's internal ID.
    
3.  Write the script you will use to generate the message, including Scriptable Cart message tags.
    
4.  Attach your script to the sales order form attached to the scriptable cart.
    
5.  Add HTML along with Scriptable Cart message tags to the appropriate fields in NetSuite based on the type of message you plan to display on your site.
    

### Related Topics

-   [Page-Level Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548584.html)
-   [Cart Line Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549413.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

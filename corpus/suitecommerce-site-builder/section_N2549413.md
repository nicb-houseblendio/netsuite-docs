---
id: "section_N2549413"
type: "section"
title: "Cart Line Messages"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Creating Customer-Facing Messages from Scriptable Cart > Cart Line Messages"
parent: "section_N2548158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549413.html"
anchors: ["procedure_N2549468"]
sha256: "2b502dc07c40b8c8e043ff18b6987407d72dd5f5b5e6f4bbf692152b8f7b88a3"
---

Use the `getCartLineField()` tag in the `Cart Line Message` field on a Site Theme template to display a message on any line of an order in the shopping cart.

Note:

The cart line message always displays under the description field in the shopping cart. Consider using color attributes and other HTML techniques to differentiate the message from the typical descriptive text associated with an item in the cart.

The site theme template applies your message to all lines in the cart. However, you can modify your script to create different messages on different lines of the cart. To do this, use your script to set values in the custom field associated with the `getCartLineField()` tag. The per-line customization occurs on the script level, not on the template level.

#### To create a message that displays inline on the shopping cart: {#procedure_N2549468}

1.  Create a custom field for your message.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Column Fields > New.
        
    2.  Enter values in the following fields:
        
        -   **ID** - Enter a short and descriptive name for the ID.
            
            You will use this ID in a Scriptable Cart message tag, for example:
            
                                    `<%=getCartLineField('custcol_msg1')%>` 
                                  
            
        -   **Type** - Select Free-Form Text.
            
        -   On the **Applies To** subtab, check the **Sale** box, and clear the **Web Store** box. The custom field is not intended to display on forms in the website, so that shoppers cannot change the values you set.
            
        -   Clear the **Store Value** field.
            
    3.  Click **Save**.
        
2.  Go to _Commerce > Site Builder > Appearance > Themes_. Click **Edit** next to the site theme on your website.
    
3.  Enter the `getCartLineField()` tag in the **Cart Line Message** field on the **Tabs & Buttons** subtab.
    
    Here, you can also add custom HTML to make your message consistent with the look and feel of your website.
    
4.  Click **Save**.
    
5.  Update your Scriptable Template to use the sales order form with the custom fields you created for Scriptable Cart messaging.
    

### Related Topics

-   [Page-Level Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548584.html)
-   [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html)
-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

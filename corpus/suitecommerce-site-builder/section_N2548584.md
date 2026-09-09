---
id: "section_N2548584"
type: "section"
title: "Page-Level Messages"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Creating Customer-Facing Messages from Scriptable Cart > Page-Level Messages"
parent: "section_N2548158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548584.html"
anchors: ["bridgehead_N2548677", "procedure_N2548713", "bridgehead_N2548881", "procedure_N2548914", "bridgehead_N2549107", "procedure_N2549133"]
sha256: "6f16a13b9496775a7546480f3f16370ca792c40dfdc6e29e92c650d686c1e89b"
---

Use the `getField()` tag to display a message on any page of your site, including item pages, the shopping cart, and all pages in the checkout process. Show any content you want, such as a graphic or a customized popup. You can even use this tag to open another browser window.

Note:

You can create a custom field for your Scriptable Cart message, or use any field that exists on your Scriptable Template sales order. In both cases, you must pass the field's internal ID in the getField() tag. To find the internal ID of an existing field, see [Finding Internal IDs of Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416043804.html)

Read the basic examples below to get you started:

-   [Creating a Basic Page-Level Message](#bridgehead_N2548677)
    
-   [Creating a Popup Message](#bridgehead_N2548881)
    
-   [Creating Messages for Checkout Pages](#bridgehead_N2549107)
    

## Creating a Basic Page-Level Message {#bridgehead_N2548677}

You can write HTML to position a page-level message on any website page.

The script attached to the cart determines the content of the message. The steps below describe how to create a message that will remain on the page.

#### To create a page-level message using Scriptable Cart: {#procedure_N2548713}

1.  Determine whether you need to create a custom field for your Scriptable Cart message, or use a field that exists on your Scriptable Template sales order.
    
    -   If you choose to use a field that exists on your Scripting Template sales order, note the field's internal ID, and go to Step 3.
        
    -   If you choose to create a Custom field for your message, go to Step 2.
        
2.  Go to Customization > Lists, Records, & Fields > Transaction Body Fields > New.
    
    Enter values in the following fields:
    
    -   **Label** - Name the custom field.
        
    -   **ID** - Enter a short and descriptive name for the ID.
        
        You will use this ID in a Scriptable Cart message tag. This sample tag displays the message in bold text:
        
                            `<b><%=getField('custbody_bannermsg')=%></b>` 
                          
        
    -   **Type** - Select Free-Form Text.
        
    -   On the **Applies To** subtab, check the **Sale** box, and clear the **Web Store** box. The custom field is not intended to display on forms in the website, so that shoppers cannot change the values you set.
        
    -   Clear the **Store Value** field.
        
3.  Go to Customization > Forms > Transaction Forms. Customize a sales order form to include the custom field you created in Step 1.
    
4.  Write the script you will use to generate the message.
    
    Note:
    
    If you already have a script that is working properly in Scriptable Cart, save a backup version.
    
5.  Use the tag in custom HTML where you want the message to display.
    
    -   To display the message on multiple site pages, add it to a site theme, or an item/category template.
        
    -   To display the message on a specific page, add the tag in one of the description fields on a tab or category record.
        
6.  Save your changes.
    
7.  Update your Scriptable Template to use the sales order form with the custom fields you created for Scriptable Cart messaging. To update your Scriptable Template, go to the Web Site Setup page, and select the sales order form as a **Scripting Template**.
    

The code sample below displays a page-level message. You can add it to the **Greeting** field on a tab record to display a message on a specific page in your website. Advanced web developers can use HTML techniques to change the look and feel.

          `<center><tr> <td width="100%" valign=top> <table border=0 cellspacing=0 cellpadding=5><tr> <td> <img src='/images/icons/store/icon_exclamation2c.gif' width=12 height=12 border=0> </td> <td> <%=getField("custbody_bannermsg")%>  </td></tr> </center>   <script> var txt = '<%=getField("custbody_bannermsg")%>';  if (!txt) {     // Hide element if no banner is there     document.getElementById('banner').style.visibility = "hidden"; } </script>` 
        

## Creating a Popup Message {#bridgehead_N2548881}

To display a message only one time, such as a popup or an alert message, use both the `getField()` and `setField()` tags together.

#### To create a basic popup: {#procedure_N2548914}

1.  Determine whether you need to create a custom field for your Scriptable Cart message, or use a field that exists on your Scriptable Template sales order.
    
    If you choose to use a field that exists on your Scripting Template sales order, note the field's internal ID, and go to Step 3.
    
    If you choose to create a Custom field for your message, do the following:
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Body Fields > New.
        
    2.  Enter values in the following fields:
        
        -   **Label** - Name the custom field.
            
        -   **ID** - Enter a short and descriptive name for the ID.
            
            You will use this ID in a Scriptable Cart message tag, for example:
            
                                    `<%=getField('custbody_popupmsg')%>` 
                                  
            
        -   **Type** - Select Free-Form Text.
            
        -   On the **Applies To** subtab, check the **Sale** box, and clear the **Web Store** box. The custom field is not intended to display on forms in the website, so that shoppers cannot change the values you set.
            
        -   Clear the **Store Value** field.
            
    3.  Click **Save**.
        
2.  Go to Customization > Forms > Transaction Forms. Customize a sales order form to include the custom field you created in Step 1.
    
3.  Write the script you will use to generate the message.
    
    Note:
    
    If you already have a script that is working properly in Scriptable Cart, save a backup version.
    
4.  Go to _Commerce > Site Builder > Appearance > Themes_.
    
5.  Click **Edit** next to a theme.
    
6.  On the **General** subtab, in the **<body> tag attributes** field, enter the following:
    
                    `onload="page_init(); showPopup();"` 
                  
    
    Note:
    
    `page_init();` is a NetSuite function.
    
    To create a popup, you must use the `BODY onload` attribute in a site theme to wait until the entire page loads before showing the popup. Otherwise writing a simple alert script, such as: `<script> alert('...'); </script>`, will result in your popup message displaying before the browser finishes rendering the rest of the page.
    
7.  Add the script to any of the fields in the Theme template.
    
    Note that the `getField()` tag retrieves content from the custom field, while the `setField()` tag clears the message content. The JavaScript below prevents the alert box from displaying continuously.
    
                    `<script>    function showPopup()    {       var msg = '<%=getField("custbody_popupmsg")%>';        if (msg)              {    alert(msg);    }      }    <%=setField( 'custbody_popupmsg ', '')%>     </script>` 
                  
    
8.  Click **Save**.
    
9.  Update your Scriptable Template to use the sales order form with the custom fields you created for Scriptable Cart messaging.
    

## Creating Messages for Checkout Pages {#bridgehead_N2549107}

Use the `getField()` tag to display a message on checkout pages.

For example, you can communicate specific shipping instructions to customers placing orders online. Create a message on the page where a shopper on your site chooses a shipping method for an order.

#### To create messaging for the shipping methods page using Scriptable Cart: {#procedure_N2549133}

1.  Determine whether you need to create a custom field for your Scriptable Cart message, or use a field that exists on your Scriptable Template sales order.
    
    -   If you choose to use a field that exists on your Scripting Template sales order, note the field's internal ID, and go to Step 3.
        
    -   If you choose to create a Custom field for your message, go to Step 2.
        
2.  Create a custom field for your message.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Column Fields > New.
        
    2.  Enter values in the following fields:
        
        -   **ID** - Enter a short and descriptive name for the ID.
            
            You will use this ID in a Scriptable Cart message tag, for example:
            
                                    `<%=getField('custbody_shipinfo')%>` 
                                  
            
        -   **Type** - Select Free-Form Text.
            
        -   On the **Applies To** subtab, check the **Sale** box, and clear the **Web Store** box. The custom field is not intended to display on forms in the website, so that shoppers cannot change the values you set.
            
        -   Clear the **Store Value** field.
            
    3.  Click **Save**.
        
3.  Go to Customization > Forms > Transaction Forms. Customize a sales order form to include the custom field you created in Step 1.
    
4.  Write the script you will use to generate the message.
    
    Note:
    
    If you already have a script that is working properly in Scriptable Cart, save a backup version.
    
5.  Go to _Commerce > Site Builder > Content > Customize Text_.
    
6.  Click the **Headings** subtab.
    
7.  Find **Shipping Method** on this page.
    
    Note:
    
    There are two **Shipping Method** headings on this page. The first one is the heading that appears in bold at the top of the page. The second is the heading that appears at the top of the bulleted list of shipping options.
    
8.  Add the `getField()` tag to the field in the Customization column.
    
9.  Click **Save**.
    
10.  Ensure that you update your scriptable template to use the sales order form with the custom fields you created for Scriptable Cart messaging.
     

The message you create will display on the Shipping Methods page based on the logic in your script.

### Related Topics

-   [Cart Line Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549413.html)
-   [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html)
-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1231841"
type: "section"
title: "Sending Order Fulfillment Email"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Order Fulfillment Confirmation Email > Sending Order Fulfillment Email"
parent: "section_N1231778"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231841.html"
anchors: ["procedure_N1231862", "bridgehead_N1231973", "procedure_N1232012"]
sha256: "60f37f7f29f2a8f40fdc6df390f77bc8a7a4e158f840f81ba6712aea455a9dbd"
---

You can configure NetSuite to send an order fulfillment confirmation email message for orders placed over the phone or with sales reps.

#### To send the order fulfillment email: {#procedure_N1231862}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Order Management** subtab.
    
3.  Under **Fulfillment**, check the **Send Order Fulfilled Confirmation Emails** box.
    
4.  Click **Save**.
    

When you process an order, NetSuite sends an email message to the customer email address on the sales order, indicating the total quantity shipped.

-   If you use the Advanced Shipping feature, the email message is sent when the order is fulfilled.
    
-   If you do not use the Advanced Shipping feature, the email message is sent when the order is billed.
    
-   If you use the Pick, Pack, and Ship feature, the email message is sent when the order is shipped.
    

The email address in the From field of the confirmation email depends on the email settings of your NetSuite account. It can be set to one of the following:

-   The company return email address.
    
-   The subsidiary return email address.
    
-   The email address of the user logged in to NetSuite. Users can also set a different email address in their preferences for all email sent from NetSuite, for example, "orders@example.com".
    

See [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html) for more information about company email settings.

Note:

If you check the **Use Web Site Template For Fulfillment Emails** box, the text specified on the Custom Web Site Text page is used for fulfillment email messages, sent for sales orders entered from the Transactions tab in NetSuite. However, fulfillment email messages, sent for web store order, do not use this text. It is no longer possible to use the same email template for fulfilment emails for orders from both sources. For information about customizing and sending fulfillment email for web store orders, see [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html).

## Customizing Order Fulfillment Email Text {#bridgehead_N1231973}

You can customize the text of the order fulfillment confirmation email message for each language available to you in the system. Depending on whether or not the Advanced Site Customization feature is enabled in your account, NetSuite uses the custom text from the Custom Web Site Text page or the Customize Fulfillment Email page respectively. See [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2601007.html#bridgehead_N2601145) for more information about the Advanced Site Customization feature.

#### To customize the order fulfillment email text: {#procedure_N1232012}

1.  Open the customization page according to the features enabled in your account.
    
    -   If the Advanced Site Customization feature is enabled, and you have a Commerce web store, go to _Commerce > Content Management > Content > Customize Text_. If you have a Site Builder website, go to _Commerce > Site Builder > Content > Customize Text_.
        
    -   If the Advanced Site Customization feature is enabled, go to Setup > Accounting > Preferences > Customize Fulfillment Email (Administrator).
        
2.  Select the language you want to customize.
    
3.  If you are on the Custom Web Site Text page, look for the custom text row that corresponds to sales order fulfilled text. If you are on the Customize Fulfillment Email page, there is only one custom text row.
    
4.  In the **Customization** column, enter the text you want to use.
    
    The Default Text column displays the HTML source code for the fulfillment email message. The blank fields in the Customization column are for the customized version of your fulfillment email message.
    
    If you are familiar with editing HTML and CSS, you can also copy the HTML from the **Default Text** column to the **Customization** column and then change the customized text to suit your business needs.
    
5.  Click **Save**.
    
    Customers now receive your customized email message when their orders are fulfilled.
    

You can use attribute tags to display information from the sales order (such as the customer name and the sales order number) in the fulfillment confirmation email message. For more information, see [Attribute Tags for Use in Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4428732431.html). Attribute tags function in the fulfillment email message regardless of whether you use the Web Store or Advanced Site Customization features.

### Related Topics

-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2601007.html#bridgehead_N2601145)
-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2609254"
type: "section"
title: "Customizing Website Text"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Using Web Site Text Groups > Customizing Website Text"
parent: "section_N2609031"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609254.html"
anchors: ["procedure_N2609293"]
sha256: "9f1a01d73fec37bd22343d6d812f760ba92aed3c2ade7e28e376aee0dcfe89b6"
---

You can customize the system-generated text that appears in your website. This includes text in error messages and buttons. It also includes headings and fields displayed during the web store checkout process. Customizing the text on your website lets you communicate more effectively with your customers.

You can also create different groups of custom text for use on multiple sites. For more information, see [Using Web Site Text Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609031.html).

#### To customize the text in your website: {#procedure_N2609293}

1.  If you have a Commerce (SC/ SCA/ SCMA/ SCIS) site, go to _Commerce > Content Management > Content > Customize Text > New_. If you have a Site Builder site, go to _Commerce > Site Builder > Content Management > Customize Text > New_.
    
2.  If you use the Multi-Language feature, select the language for which you want to customize the text. An administrator can select multiple languages for your site at _Setup > Company > General Preferences > Languages_.
    
3.  The Customize Web Site Text page is divided into subtabs for each block of text that appears in your website.
    
    -   **Headings** - Change the headings on pages in the checkout process.
        
    -   **Field Labels** - Customize the labels for entry fields on your web store. For example, you can change the 'Address 1' field label on the Address page in the web store, to 'Street Address.'
        
    -   **Alerts** - Customize alerts displayed in the web store. For example, you can customize the alert that is displayed when a shopper selects a product in a color that is out of stock.
        
    -   **List Options** - Customize the default option on select lists. This affects items on your web store with list options such as matrix items.
        
        For example, when a shopper selects a color or size for a product, you can change the NetSuite default list option from 'Select' to 'Choose One.'
        
    -   **Buttons** - Change the text on buttons in the web store. For example, you can customize the label on each of the buttons on the shopping cart page.
        
    -   **Error Messages** - Customize error messages displayed on your web store. For example, you can change the error message displayed when a customer enters an invalid coupon or gift certificate code.
        
        Note:
        
        Customized error messages will not be displayed on websites using Site Builder Reference Checkout version 2.05 and earlier. The default error message will be displayed.
        
    -   **Messages** - Customize other labels and messages displayed in the web store. For example, you can customize the cookie compliance message, the website disclaimer, footer messages etc.
        
4.  Click on a subtab to choose a type of website text to customize.
    
    The **Default Text** column displays the HTML source code for each block of text that appears in the web store. The blank fields in the **Customization** column are for your customized changes to the existing HTML. The **Description** column provides more information about each field.
    
5.  Copy the HTML in the **Default Text** column, make your changes, and then paste your customized HTML in the **Customization** column.
    
6.  Click Save.
    

To view your updated site after you save your changes, go to _Commerce > Websites > Preview Website_.

### Related Topics

-   [Attribute Tags for Use in Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4428732431.html)
-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html)
-   [Site Builder Items, Forms, & Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2582621.html)
-   [Web Site Language Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2567348.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

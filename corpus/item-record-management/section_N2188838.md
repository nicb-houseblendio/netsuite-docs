---
id: "section_N2188838"
type: "section"
title: "Customizing Price List Forms"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Generating Price Lists > Customizing Price List Forms"
parent: "section_N2185787"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html"
anchors: ["procedure_N2188857", "procedure_160684307854"]
sha256: "b7a8e6f095dbd32351e0a8ec83b6575c3dc7efa256d22f3f58f559ee7cf221da"
---

When you generate a price list, the standard form shows the following information:

-   customer's address
    
-   date the list was generated
    
-   item names and descriptions
    
-   item prices
    
-   currencies, if applicable
    

If you use the Quantity Pricing feature, the price list shows a column for each quantity and the matching prices.

You can also customize your price list form, for example, by adding your logo.

If you customize a standard form, the header can show custom fields from customer records. You can also set u\[ the body to show custom fields from item records.

#### To customize a price list form: {#procedure_N2188857}

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  Next to the Standard Price List form, click **Customize**.
    
3.  Enter a custom form **Name**.
    
4.  Enter an **App ID**.
    
5.  Enter the internal custom transaction form **ID**.
    
6.  To set the formatting for printed and emailed transactions that use this custom form, choose a **Printing Type**.
    
    -   To use advanced PDF/HTML templates to format transactions, choose the **Advanced** option
        
    -   To use basic PDF and HTML layouts, choose the **Basic** option. For more information, see the next procedure.
        
7.  Select the template you want to use for printed transactions with this custom form.
    
    This includes the standard template for the transaction type and any custom templates you've created for it.
    
8.  Select the **Email Template** with the email attachment layout you want to use for this transaction type in the NetSuite UI.
    
9.  Enter a disclaimer or other message to show at the bottom of your custom form.
    
    You can enter up to 4,000 characters, including spaces.
    
10.  Enter the **Address** you want to show on this form.
     
     If you don't enter an address, your default company address is used.
     
11.  Select a company **Logo**.
     
     If you don't select a logo, your default company logo is used.
     
12.  Check the **Form is Preferred** box to make this your preferred form for this transaction type.
     
13.  Click **Save**.
     
14.  On the **Header**, **Columns**, **Body**, and **Footer** subtabs, select the data types you want to show on the custom form.
     

#### To define the basic printing type: {#procedure_160684307854}

1.  Fill out the optional **Header** subtab fields:
    
    -   To display the company name in the header, check the **Company Name** box and enter the company name in the Label field.
        
    -   To display the company logo in the header, check the **Company Logo** box.
        
    -   To display the company address in the header, check the **Company Address** box.
        
    -   To display the company phone number in the header, check the **Company Phone** box and enter the company phone number in the **Label** field.
        
    -   To display the company URL in the header, check the **Company URL** box and enter the company URL in the **Label** field.
        
    -   To display the business number in the header, check the **Business Number** box and enter the company business number in the **Label** field.
        
    -   To display the form title in the header, check the **Form Title** box and enter the form title in the **Label** field.
        
    -   To display the page number in the header, check the **Page Number** box and enter the page number in the **Label** field.
        
    -   To display the account number in the header, check the **Acct. No.** box and enter the account number in the **Label** field.
        
    -   To display the date in the header, check the **Date** box and enter the date in the **Label** field.
        
    -   To display the bill to address in the header, check the **Bill To** box and enter the bill to address in the Label field.
        
2.  The **Body** data from custom fields can be added as body fields, with the exception of multi-select fields. This applies to custom fields on customer records and item records.
    
    When you create a new custom entity field or custom item field, you can check the **Print on Price List** box to include the field. For more information, see [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html) or [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html).
    
3.  Complete the optional **Columns** subtab fields:
    
    -   Item
        
    -   Description
        
    -   Unit
        
    -   Unit Price
        
    
    You can optionally add the following data in columns:
    
    -   Parent Item
        
    -   Vendor Name
        
    -   UPC Code
        
    -   Drop Ship Item
        
    -   Special Order Item
        
    -   Manufacturer
        
    -   Manufacturer Part #
        
    -   Weight
        
    -   Price Level
        

For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

### Related Topics

-   [Customize Price List Pages and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2186163.html)
-   [Price List Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2187468.html)
-   [Searching for Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171136751.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171157590.html)
-   [Generating Bulk Price Lists and Customizing Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2187796.html)
-   [Generating an Individual Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188411.html)
-   [Working With Pricing Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2189322.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

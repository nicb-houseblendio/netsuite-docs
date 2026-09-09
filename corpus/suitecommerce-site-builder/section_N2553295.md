---
id: "section_N2553295"
type: "section"
title: "Scriptable Cart FAQ"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Scriptable Cart FAQ"
parent: "chapter_N2545000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html"
anchors: ["question_N2553309", "question_N2553334", "question_N2553364", "question_N2553387", "question_N2553408", "question_N2553439", "bridgehead_N2553473", "question_N2553515", "question_N2553589", "question_N2553707", "question_N2553744", "question_N2553766", "question_N2553796", "question_N2553829", "question_N2553861", "question_N2553892"]
sha256: "7b70984bc102a90ad3aa469508a4ca9f4b5e214bab7af8064b46f8a331bd1027"
---

### How do I turn on the Scriptable Cart? {#question_N2553309}

To use the scriptable cart, an administrator must enable the following features: Advanced Site Customization, and Client SuiteScript.

After you have turned on the required features, go to _Commerce > Websites > Website List_ and click Edit next to your website name. Then check the Scriptable Cart and Checkout box, and set the Scripting Template fields.

### Are there sample scripts available for testing? {#question_N2553334}

Yes. For more information, see [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html).

### What is the best way to test scripts for the shopping cart? {#question_N2553364}

Test your scripts in a Sandbox account before you deploy the Scriptable Cart in your live production website.

### Can I use SuiteScript on forms that I use for the Customer Center? {#question_N2553387}

Yes. You must customize a Standard Online Sales Order - Invoice (External) or Standard Online Sales Order - Cash Sale (External) form and then attach a client script.

### Can I use SuiteScript on website registration forms? {#question_N2553408}

No. SuiteScript is not compatible with online registration forms. You can use Suite Script Server Pages (SSP) for customizing the registration form. for more information, see [SSP Application Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html).

### Should I use form-level or record-level scripts for Scriptable Cart? {#question_N2553439}

**Using Form-Level Scripts in the Shopping Cart**

A form-level script provides the most flexibility for multiple websites. Using a form-level script, you can create different Invoice and Cash Sale forms for use on different websites.

Note that attaching a form to a script record is the first step when using SuiteScript in the shopping cart, however it is the third step when creating a script in a non-web store context. For general information about using form-level scripts, see [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html).

## Using Record-Level Scripts in the Shopping Cart {#bridgehead_N2553473}

A record-level script can run on all sales orders in the application and on the web store. When using a record-level script in the shopping cart, you are not required to maintain more than one Sales Order - Invoice and Sales Order - Cash Sale form.

The sample scripts for [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html) and [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html), both use a script of type, User Event which requires a record-level script and a script deployment.

### What type of sales order forms can I use for the Scriptable Cart? {#question_N2553515}

You can customize any of the sales order transaction forms listed below by attaching a client script, and then entering the functions on the Custom Code subtab:

-   Standard Sales Order - Invoice
    
-   Standard Sales Order - Cash Sale
    
-   Standard Online Sales Order - Invoice (External)
    
-   Standard Online Sales Order - Cash Sale (External)
    

Next, go to _Commerce > Websites > Website List_ and select the forms, you want to use in the Scripting Template (Credit Card), and Scripting Template (Invoice) fields.

Note:

It is important that the fields on the custom sales order form correspond with features you have enabled in your account. For example: If you use a script that reads revenue recognition fields, you must include these fields on your custom sales order form.

### What are the differences between a shopping and a checkout form? {#question_N2553589}

Shoppers on your web store must use a shopping form and a checkout form during web store checkout. You can use the same transaction form for both purposes.

The shopping form is transitory. It contains the order while customers are shopping on your site. Your custom SuiteScript is attached to the shopping form, and then used as a Scripting Template. However, when customers submit orders into NetSuite, they do so on a checkout form. The checkout form remains in the system.

During a web store sale, data is passed from the shopping form to the checkout form. The checkout form is then saved in the database, so you must ensure that fields on the shopping form correspond to fields on the checkout form.

**To set up your shopping and checkout forms:**

1.  Go to Setup > Transactions > Transaction forms.
    
    1.  Set up your shopping form for the Scriptable Cart: Customize a sales order form by attaching a client script, and then entering the functions on the Custom Code subtab. If you use terms for invoicing some customers, you must attach your script to both types of sales order forms: cash sale and invoice.
        
    2.  Set up your checkout form: Identify an existing sales order form or create a customized internal sales order form for use as the checkout form.
        
        Note:
        
        If the same custom fields do not exist on both the shopping and checkout forms, then the data that was collected by the shopping form is discarded. Also note that any client scripts attached to the checkout form do not run. The only scripts that can run on the checkout form are user-event scripts.
        
2.  Go to _Commerce > Websites > Website List_ to specify the forms you want to use on your web store for both shopping and checkout.
    
    1.  Specify the shopping form: On the Setup subtab, select the sales order form with your script attached in one or both of the Scripting Template fields.
        
    2.  Specify the checkout form: Click the Shopping subtab. In the Checkout Preferences section, select the sales order form (or forms) you created in Step1b.
        
3.  Click Save.
    

For more information, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### On which type of form do shoppers submit web orders? {#question_N2553707}

Shoppers on your website submit orders on internal sales order forms.

The forms you select on the Shopping subtab of the Setup Web Site page in the Checkout Preferences section determine the forms on which shoppers submit their web orders. You cannot select external forms for this purpose.

For more information, see [Shopping Cart and Checkout Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2571737.html).

### Can I use Scriptable Cart to change the workflow of the checkout process in a web store? {#question_N2553744}

No. You cannot use SuiteScript to skip pages or change the order in which checkout pages are displayed. SuiteScript is only supported in the web store shopping cart.

### Does a change to the Payment Method field or any custom field on the Order Summary page trigger the Field Changed event in a scriptable cart? {#question_N2553766}

Yes. The client event model is supported. For more information, see [Client Events Supported in Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html#bridgehead_N2545330).

### Can I use a Field Changed event to display an alert to the shopper? {#question_N2553796}

For information about creating alerts for your web store customers, see [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html).

Note that you must use a custom body field for the message you want to display to shoppers on your site. This type of custom field is updated in place without requesting a browser refresh. You must use client-side JavaScript to create an alert box.

### Can I use SuiteScript to create a button on a Sales Order form that launches a Suitelet in a new window to add or update line item values in the cart? {#question_N2553829}

Yes. Create a button or a link that opens the Suitelet using **window.open**. After the Suitelet finishes processing, you can write a response like this one:

              `response.write('<html><head><script>window.opener.sampleFunction();  self.close();</script></head><body></body></html>');` 
            

### Can I give away a $100 gift certificate for free with the purchase of other goods? {#question_N2553861}

Yes. You can look at the sample script provided for [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html), and then revise it to meet your specific business needs.

### Why does my script give an Invalid Field Reference error? {#question_N2553892}

Invalid field errors can indicate a problem with the form you selected as the Scripting template. This error might be returned if you are using a form that does not expose fields referenced by the script on the form. Note that not all fields are exposed on the Sales Order (External) form. If you see an error on submitting a web order, try using a customized Standard Sales Order - Invoice or Standard Sales Orders - Cash Sale form for your Scripting Template.

For example: Your script refers to a price level field, but your scripting template form does not expose the Price Level field. The web store shopper will generate an **Invalid price reference key** error when submitting an order.

### Related Topics

-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html)
-   [Custom Error Messages for ValidateLine Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549673.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

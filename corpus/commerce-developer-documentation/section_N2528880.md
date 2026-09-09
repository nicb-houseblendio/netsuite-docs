---
id: "section_N2528880"
type: "section"
title: "payment"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > payment"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2528880.html"
anchors: ["bridgehead_47194600302", "bridgehead_N2529392", "bridgehead_N2529409"]
sha256: "9d177935820720809fae6683cacd5028ec0affc37708336e146c3ecdbadb29ca"
---

This object contains payment information for the order.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| ach | JSON [ach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0404071044.html) object | Payment information when ach is selected as the payment method **Note**: See [Formatting Values for ACH Payments](#bridgehead_47194600302) for an example of how to format this information. | yes | yes |
| creditcard | JSON [creditcard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2518010.html) object | Payment information when credit card is selected as the payment method **Note**: See [Formatting Values for Credit Card Payments](#bridgehead_N2529392) for an example of how to format this information. If the Payment Instruments feature is enabled, and the credit card has been tokenized, this field contains the internal ID and payment method of payment card token. | yes | yes |
| paymentmethod | JSON [paymentmethod](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2529580.html) object | Details of the payment method selected by customer. | yes | yes |
| paymentterms | string | Payment terms selected by customer. Value should be CreditCard, Ach, or Invoice. **Notes**: Set this value to **Invoice** to use an invoice as payment. See [Using an Invoice as Payment](#bridgehead_N2529409) for an example. | yes | yes |
| paypal | JSON object | PayPal information if enabled | yes | no |
| status | JSON [status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2535212.html) object | Embedded status object used for web store business logic validation | yes | yes |

## Formatting Values for ACH Payments {#bridgehead_47194600302}

The following example code illustrates how to format details for a payment using an existing ACH bank account:

          `function service(request,response) {  payment = {     'paymentterms' : 'Ach',     'ach': {         'internalid': '146'           } };   var order = nlapiGetWebContainer().getShoppingSession().getOrder(); order.setPayment(payment)  };` 
        

## Formatting Values for Credit Card Payments {#bridgehead_N2529392}

The following example code illustrates how to format details for a payment using a new credit card:

          `function service(request,response) {   var payment = { creditcard: {   'ccname': 'Herb Joseph',   'ccnumber': '4111111111111111',    'expmonth' : '09',   'expyear': '2013',   'paymentmethod':  {       'internalid': '7',     'name': 'Visa',     'ispaypal': 'F',     'creditcard': 'T',     'key': '8,8,1135464'}  } };    var order = nlapiGetWebContainer().getShoppingSession().getOrder(); order.setPayment(payment)   };` 
        

The following example code illustrates how to format details for a payment using a stored credit card:

          `function service(request,response) {   var payment = { creditcard: {   'internalid': '35',   'paymentmethod':  {       'internalid': '7',     'name': 'Visa',     'ispaypal': 'F',     'creditcard': 'T',     'key': '8,8,1135464'}  } };    var order = nlapiGetWebContainer().getShoppingSession().getOrder(); order.setPayment(payment)   };` 
        

## Using an Invoice as Payment {#bridgehead_N2529409}

The following example code illustrates how to use an invoice as a payment method:

          `function service(request,response) {                                       var returnval = null;                                          try                     {                                         var payment = {                                                              paymentterms : 'Invoice'                                         };                                         nlapiGetWebContainer().getShoppingSession().getOrder().setPayment(payment);                     }                     catch (e)                     {                                         var nle = nlapiCreateError(e);                                         returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};                     }                     response.writeLine(JSON.stringify(returnval)); }` 
        

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2518010"
type: "section"
title: "creditcard"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > creditcard"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2518010.html"
anchors: []
sha256: "100d933b8790343db05389c325f0bdf9fdf295e531299e8a9b670bc4ab96c9c5"
---

This object contains credit card information.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| ccdefault | string | Indicates whether credit card is the default Value should be T or F. | yes | yes |
| ccexpiredate | string | Card expiration date | yes | no |
| ccname | string | Name on card | yes | yes |
| ccnumber | string | Card number Value returned by Get function is masked. | yes | yes |
| ccsecuritycode | string | Card security code Only needed if payment method is creditcard. | no | yes |
| customercode | string | Customer code | yes | yes |
| debtcardissueno | string | Card issue number for UK **Note**: Not exposed in Customer record. | yes | yes |
| expmonth | string | Card expiration month | yes | yes |
| expyear | string | Card expiration year | yes | yes |
| internalid | string | Internal ID of credit card. If the Payment Instruments feature is enabled, and the credit card has been tokenized, this contains the internal ID of payment card token. | yes | yes |
| paymentmethod | Object of type [paymentmethod](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2529580.html) | Payment method type **Note**: For credit card payments, this is the numerical code of the credit card type. If the Payment Instruments feature is enabled, and the credit card has been tokenized, this is the numerical code of the payment token type. | yes | yes |
| savecard | string | Indicates whether the card should be saved. Possible values are:
-   F - the card is not saved.
-   T - the card is saved.

If the order.submit() method is called with savecard set to T, the card is saved and it is also set as the default card. If the customer methods addCreditCard() and updateCreditCard() are called, the card is saved regardless of the value of the savecard parameter. However, for these methods, the card is set as the default card only if the value of ccdefault is T. | no | yes |
| validfrom | string | Card valid from date **Note**: Not exposed in Customer record. | yes | no |
| validfrommon | string | Card valid from month for UK | yes | yes |
| validfromyear | string | Card valid from month for UK | yes | yes |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

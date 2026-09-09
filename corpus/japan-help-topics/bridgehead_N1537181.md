---
id: "bridgehead_N1537181"
type: "bridgehead"
title: "Specifying Transactions for Inclusion in an Invoice Summary"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japanese Invoicing > Japanese Invoice Summary > Specifying Transactions for Inclusion in an Invoice Summary"
parent: "section_N1536907"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537181.html"
anchors: ["bridgehead_159954178107"]
sha256: "85b317e1af9b480f64a5cf967a3076cedbe74b65b14b2994983c9d7b402a46a8"
---

You can specify Japanese customer's transactions to be included in an invoice summary.

Transactions that can be included in an invoice summary are:

-   invoice
    
-   credit memo
    
-   tegata
    
-   journal
    
-   customer payment or deposit
    
    For more information, see [Applying a Customer Payment to an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1538934.html)
    
-   sales order (closed or canceled)
    
-   custom transactions for payment adjustments or accounts receivables (AR):
    
    -   AR Adj Debit Invoice Summary
        
    -   AR Adj Credit Invoice Summary
        
        For more information, see [Including Payment Adjustments in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954224986.html)
        

On any of the supported transaction records, check the **Include in Invoice Summary** box to include that transaction in the invoice summary when generated. The box is checked by default on the transaction record of a customer that uses invoice summaries.

Note:

If the **Use Invoice Summary** box is checked, customer payments are always included in the invoice summary. Customer payments don't have the Include in Invoice Summary box. If there are no payments in the billing period, the invoice summary Payment Details sections indicates 'There is no payment this billing period'.

For more information, see [Specifying Customers Who Use Invoice Summaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537000.html).

For journals, aside from having the Include in Invoice Summary box checked, they must meet these requirements to be included in an invoice summary:

-   Status must be Approved.
    
-   Customer is specified.
    
-   Account is accounts receivable type.
    

You can manually clear the Include in Invoice Summary box to exclude the transaction from the invoice summary. You can set the value of the Include in Invoice Summary box when creating or updating customer transactions through the user interface, CSV import, script, or web service.

After the invoice summary is generated, the system updates the **Invoice Summary Transaction** field on the transaction by adding a link to the invoice summary record.

Note:

Although a transaction has the Include in Invoice Summary box checked, you should still verify if the associated customer record uses invoice summary and has payment terms. If the **Use Invoice Summary** box on the customer record is cleared or payment terms are missing, problems in subsequent processing may be encountered. For example, a credit memo created from an invoice of a customer whose record doesn't use invoice summary, won't be included in invoice summary generation.

Furthermore, if Include in Invoice Summary on the transaction is checked, the system automatically validates and calculates the closing date and payment due date on the transaction based on the transaction date and date values specified for Japan payment terms. This is applied to all transaction records with Include in Invoice Summary checked, even if Use Invoice Summary on the customer record isn't checked.

The table shows the cases for including customer and transaction records in the invoice summary.

| Use Invoice Summary in customer record checked? | Include in Invoice Summary in transaction record checked? | Automatic validation and calculation of closing date and payment due date in transaction? | Transaction included in invoice summary? |
| --- | --- | --- | --- |
| Yes | Yes | Yes | Yes |
| Yes | No (initially checked by default, then manually cleared) | No | No |
| No | Yes (initially cleared by default, then manually checked) | No You must re-enter the transaction date or closing date in an invoice or credit memo to enable automatic calculation and validation, but only if Japan payment terms is set up on the customer record. | No |
| No | No | No | No |

As support for multi-subsidiary customer in OneWorld accounts, transactions of customers with Japan as secondary subsidiary can also be included in the invoice summary. However, this has limitations when accepting payments from multi-subsidiary customers in _Transactions > Customers > Accept Customer Payments_. On the **Apply** subtab, you must manually check the **Apply** box of the invoices in the list that you want to apply the payment to.

## More Details about Including Transactions and Payments in the Invoice Summary {#bridgehead_159954178107}

Consider these details when including transactions and payments in the invoice summary:

-   If no payments are included in the invoice summary, the invoice summary Payment Details sections indicates 'There is no payment this billing period'.
    
-   The Transaction Details section of the invoice summary includes invoices with status Open and Paid in Full.
    
-   The Transaction Details and Payment Details sections include transactionnumber and tranid.
    
-   Customer deposits and partial payments are applied or reflected in the Net Invoice This Period, under the Invoice Details section of the invoice summary.
    
-   Fully paid invoices are included in the Total Sales This Period, under the Summary section.
    

### Related Topics

-   [Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536907.html)
-   [Setting the Preferred Form for the Invoice Summary Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4357445509.html)
-   [Setting the Invoice Summary Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547537829.html)
-   [Specifying Customers Who Use Invoice Summaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537000.html)
-   [Applying a Customer Payment to an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1538934.html)
-   [Including Payment Adjustments in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954224986.html)
-   [Adding Field Values to the Invoice Summary Output](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547538342.html)
-   [Specifying a Folder to Save Invoice Summaries In](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954596474.html)
-   [Generating a Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539302.html)
-   [Regenerating an Invoice Summary for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355754839.html)
-   [Viewing Invoice Summary Generation Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159953645373.html)
-   [Invoice Summary Generation Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355762776.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

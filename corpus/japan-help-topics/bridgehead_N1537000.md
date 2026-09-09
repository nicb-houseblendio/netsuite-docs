---
id: "bridgehead_N1537000"
type: "bridgehead"
title: "Specifying Customers Who Use Invoice Summaries"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japanese Invoicing > Japanese Invoice Summary > Specifying Customers Who Use Invoice Summaries"
parent: "section_N1536907"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537000.html"
anchors: []
sha256: "660151d30639a5a0138168c17990cc1b4500fc1a0a8491116f32ae686670d719"
---

If you want to send a Japanese customer an invoice summary instead of individual invoices, check the **Use Invoice Summary** box on the **Japan Localization** subtab of the customer record.

Customer records with the Use Invoice Summary box checked, must have at least one set of payment terms defined. If no payment term is defined, you can't save the customer record. See [Setting Up Japan Payment Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4292577772.html).

If Use invoice Summary is checked on the customer record, the **Include in Invoice Summary** box on the customer's invoices, credit memos, tegatas, journals, customer deposits, and sales orders will be automatically checked. The customer and its transactions with Include in Invoice Summary checked, will be included when an invoice summary is generated.

In addition, if Use invoice Summary is checked, consider these cases:

-   The **Compute Due Date** box is automatically checked. This enables automatic computation of the due date as well as application of holiday checking and due date adjustment, for the customer. For more information, see [Enabling Compute Due Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0809110403.html).
    
-   You can enable the features supporting the 2023 Qualified Invoicing System by checking the **Apply Invoice Summary Tax Adjustment** box. This uses a new computation of the total consumption tax in the invoice summary and applies AR (accounts receivable) debit or credit adjustment for any difference in the tax amount between the transactions and invoice summary. However, if Use Invoice Summary is cleared, Apply Invoice Summary Tax Adjustment is automatically cleared. For more information, see [Support for Japan Qualified Invoicing System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0306032503.html).
    
-   Customer payments are always included in the invoice summary.
    

If Use Invoice Summary isn't checked on the customer record, and you generate an invoice summary, the customer and its transactions will not be included in the search result.

As support for multisubsidiary customer in OneWorld accounts, the **Use Invoice Summary** box is also available on customer records with Japan as secondary subsidiary. However, this has limitations when accepting payments from multi-subsidiary customers in _Transactions > Customers > Accept Customer Payments_. On the **Apply** subtab, you must manually check the **Apply** box of the invoices in the list that you want to apply the payment to.

### Related Topics

-   [Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536907.html)
-   [Setting the Invoice Summary Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547537829.html)
-   [Generating Invoice Summary PDF per Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161531931259.html)
-   [Specifying Transactions for Inclusion in an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537181.html)
-   [Applying a Customer Payment to an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1538934.html)
-   [Including Payment Adjustments in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954224986.html)
-   [Generating a Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539302.html)
-   [Regenerating an Invoice Summary for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355754839.html)
-   [Viewing Invoice Summary Generation Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159953645373.html)
-   [Invoice Summary Generation Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355762776.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

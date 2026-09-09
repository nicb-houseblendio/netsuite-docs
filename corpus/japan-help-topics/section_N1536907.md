---
id: "section_N1536907"
type: "section"
title: "Japanese Invoice Summary"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japanese Invoicing > Japanese Invoice Summary"
parent: "chapter_N1534283"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536907.html"
anchors: []
sha256: "1726084dda64345f2a05ea279224ae265479e0e192097043718e9d974582839d"
---

The invoice summary (formerly called item detail statement (IDS)), provided by the Japan Localization SuiteApp, is a is a merged invoice of all transactions with a customer within a billing period. Your company can generate invoice summaries using the Japan Localization SuiteApp, and then send them to your customers.

The invoice summary can include these transactions:

-   invoice
    
-   credit memo
    
-   tegata
    
-   journal
    
-   customer payment or deposit
    
-   sales order (closed or canceled)
    
-   custom transactions for payment adjustments or accounts receivables (AR):
    
    -   AR Adj Debit Invoice Summary
        
    -   AR Adj Credit Invoice Summary
        

You can send one invoice summary to a customer per billing period, instead of multiple invoices for every sale transaction. Therefore, your customers will only have to pay the amount in the invoice summary one time, which saves them the effort and bank transfer charges in paying multiple bills.

You can generate an invoice summary that includes many of the supported transactions as needed. This is done by checking the **Include in Invoice Summary** box on the transaction records, and the **Use Invoice Summary** box on the customer record. Customer payments are always included in the invoice summary, if Use Invoice Summary is checked on the customer record.

Credit memos created within a billing period, either as standalone ones or from an invoice or return authorization, are included in the invoice summary. The total amount of credit memos is indicated in the Total Credits This Period column in the Summary table of the generated PDF file of the invoice summary.

You also have the option to include in a current invoice summary, the overdue invoices from a previous invoice summary.

Multiple currencies can be supported in one invoice summary.

The invoice summary record and PDF file are generated using a scheduled script. When generation is completed, the system sends you an email notification with a link to the generated PDF file.

As a custom transaction type, the invoice summary is saved as a record, with a System Notes subtab that tracks changes.

If multiple customers are included in generation, multiple invoice summary records will be created, one record for each customer. But only one PDF file will be created containing all customers. You can open an invoice summary record of a customer to regenerate it.

If you've customers with subcustomers, you can use the consolidated invoice summary, which includes all transactions of your customers' subcustomers. This feature will be called 'consolidated invoice summary' throughout the Japan Help topics, while the term 'invoice summary' will refer to the standard or regular invoice summary with an individual customer. For more information, see [Consolidated Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164606685907.html).

The invoice summary has a Tax Details section indicating amounts for invoices for the current billing period (excluding overdue invoices). The Tax Details section contains information about Tax Code, Tax Rate, and tax amounts.

In addition, a Payment Details section is included, with fields indicating the Date, Transaction No., Transaction Details (sourced from the custom field Payment Details), and Amount.

### Related Topics

-   [Japan Localization Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159949887311.html)
-   [Japan Localization SuiteApp Limitations and Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4367577095.html)
-   [Japanese Billing Cycle and Payment Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536510.html)
-   [Including Japan Localization Custom Fields in Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4359065189.html)
-   [Meeting Japanese Invoicing Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536200.html)
-   [Roles and Permissions for Using Japanese Invoicing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4357171134.html)
-   [Setting the Preferred Form for the Invoice Summary Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4357445509.html)
-   [Setting Up Auto-Generated Invoice Summary Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4292736063.html)
-   [Setting the Invoice Summary Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547537829.html)
-   [Specifying Customers Who Use Invoice Summaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537000.html)
-   [Generating Invoice Summary PDF per Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161531931259.html)
-   [Specifying Transactions for Inclusion in an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537181.html)
-   [Applying a Customer Payment to an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1538934.html)
-   [Including Payment Adjustments in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954224986.html)
-   [Adding Field Values to the Invoice Summary Output](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547538342.html)
-   [Invoice Summary PDF File Naming](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4356558397.html)
-   [Specifying a Folder to Save Invoice Summaries In](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954596474.html)
-   [Including Tax Registration Number on Invoice Summaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161531915078.html)
-   [Generating a Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539302.html)
-   [Regenerating an Invoice Summary for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355754839.html)
-   [Viewing Invoice Summary Generation Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159953645373.html)
-   [Invoice Summary Generation Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355762776.html)
-   [Customizing the Japanese Invoice Summary XML Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539711.html)
-   [Invoice Summary Collection Calendar Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4327112408.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

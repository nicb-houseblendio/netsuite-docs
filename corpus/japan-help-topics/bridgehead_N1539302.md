---
id: "bridgehead_N1539302"
type: "bridgehead"
title: "Generating a Japanese Invoice Summary"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japanese Invoicing > Japanese Invoice Summary > Generating a Japanese Invoice Summary"
parent: "section_N1536907"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539302.html"
anchors: []
sha256: "fe32455234cad681f28d1d3869ab8eab456e4f55643b338e0168b2e5d8b79861"
---

Before generating an invoice summary, you must first determine the customers whom you need to generate an invoice summary for. The Generate Invoice Summary page has search fields where you can enter criteria to search for customers. Go to Transactions > Customers > Generate Invoice Summary.

To generate an invoice summary for transactions in a closed accounting period, you must first enable **Allow Non G/L Changes** for the closed period. For more information, see [Unlocking Period Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html). When generating an invoice summary, the system can update the invoice summary fields on transactions by adding links to the invoice summary record and PDF file. If Allow Non G/L Changes isn't enabled in the closed period, when you generate an invoice summary for transactions in that period, the system won't be able to add the links.

Invoice summary generation is processed by a scheduled script. If the system is still processing a previous invoice summary generation request when you clicked Generate, your recent request will be queued. The script will process your request as soon as the earlier invoice summary generation is completed.

Note:

The Multi-Queue feature isn't yet supported by the Japan Localization SuiteApp.

A transaction is prevented from being included in more than one invoice summary, because it isn't possible to generate an invoice summary if an earlier generation process, with has the same subsidiary and closing date, is in progress. In this case, an error message is displayed, indicating the name of the user who performed the previous invoice summary generation. Try generating the invoice summary later, after the previous generation with the same criteria is completed.

If you're not using a OneWorld account, you can't generate an invoice summary if an earlier generation process for the same closing date is still in progress, even if it's for a different customer.

Note:

You can apply tax rounding methods to the tax amount in an invoice summary. For more information, see [Setting Tax Rounding Methods - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1935242.html).

Ensure that you've met all prerequisites for invoice generation, then follow these procedures to generate your Invoice summary:

-   [Specifying Search Criteria for Transactions for Inclusion in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1226042814.html)
    
-   [Generating the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1226042830.html)
    

The time it takes to process invoice summary generation depends on the volume of transactions included for the selected period. For example, based on these conditions, the estimated processing time is about one hour:

-   the invoice summary contains 3,400 transactions (invoices, credit memos, sales orders);
    
-   each transaction has three lines; or
    
-   the transactions are evenly distributed across 50 customers.
    

Note:

To prevent errors in invoice summary generation, you must limit the number of transactions per batch to 4,000. The number of customers per invoice summary generation affects processing time more than the number of transactions. Therefore, 4,000 transactions spread across more customers will result in a longer generation time. Before generating the invoice summary, you can use the customer saved search on the Generate Invoice Summary page, to verify that the number of transactions in the batch doesn't exceed 4,000. In using the saved search, try to limit the number of results by being more specific with the customer filter or search criteria.

For more information about working with invoices and invoice summaries for Japanese customers, read these topics:

### Related Topics

-   [Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536907.html)
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
-   [Regenerating an Invoice Summary for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355754839.html)
-   [Viewing Invoice Summary Generation Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159953645373.html)
-   [Invoice Summary Generation Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355762776.html)
-   [Customizing the Japanese Invoice Summary XML Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539711.html)
-   [Invoice Summary Collection Calendar Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4327112408.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

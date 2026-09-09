---
id: "section_N1973237"
type: "section"
title: "Generating the PT SAF-T"
branch: "portugal-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Portugal Help Topics > Portugal Tax Topics In Accounts Without SuiteTax > Portugal Standard Audit File for Tax Purposes (PT SAF-T) > Generating the PT SAF-T"
parent: "section_N1971159"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1973237.html"
anchors: []
sha256: "846fbefdbccf46afb426fb3f5fe472bb3a30439e946befa706ffb341215fdd85"
---

Important:

This topic pertains to the Portugal SAF-T files generation feature, which is no longer supported as of Tax Audit File SuiteApp version 1.85.0. You can only use this SuiteApp to generate Portugal SAF-T files from 2022 and earlier. To generate this report, see [Generating the PT SAF-T File in Portugal Localization SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161831214836.html).

NetSuite supports PT SAF-T Version 1.03.

The contents of the PT SAF-T are gathered from the following sources:

-   Data entries in your General Ledger or Chart of Accounts
    
    Note:
    
    For OneWorld accounts, use the Statutory Chart of Accounts if the standard Chart of Accounts doesn't comply with regulatory requirements. For example, if the standard chart of accounts is shared with other subsidiaries, or if the parent company requires a subsidiary to use account names and numbers that aren't in the formats required for statutory compliance in the subsidiary's country.
    
    The Statutory Chart of Accounts is included in the Tax Audit File SuiteApp and is available for PT SAF-T. For more information, see [Statutory Chart of Accounts for Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3929759676.html).
    
-   Master file data of customers and suppliers
    
-   Details of invoices, orders, payments, adjustments, and item fulfillment transactions
    

NetSuite's Tax Audit Files SuiteApp provides the following Portugal SAF-T reports:

| Report | Tables |
| --- | --- |
| **Portugal SAF-T** | 
-   General Ledger
-   Customer
-   Supplier
-   Product
-   Tax Table
-   General Ledger Entries
-   Sales Invoices
-   Movement of Goods
-   Working Documents
-   Payments

 |
| **Portugal SAF-T Invoicing** | 

-   Customer
-   Supplier
-   Product
-   Tax Table
-   Sales Invoices
-   Movement of Goods
-   Working Documents
-   Payments

 |
| **Portugal SAF-T Accounting** | 

-   General Ledger
-   Customer
-   Supplier
-   Tax Table
-   General Ledger Entries
-   Payments

 |

Note:

The generated PT SAF-T includes the Payments table only if the **Cash Basis Reporting** preference is enabled. To enable this preference, go to Setup > Accounting > Accounting Preferences. On the **General** subtab, check the **Cash Basis Reporting** box under General Ledger.

Important:

The current version of PT SAF-T only supports required tags as specified in the [Portuguese Tax Authority (Autoridade Tributária e Aduaneira)](https://info.portaldasfinancas.gov.pt/pt/apoio_contribuinte/SAFT_PT/Paginas/news-saf-t-pt.aspx) requirements. If the PT SAF-T validator will support optional tags, the NetSuite PT SAF-T solution will be updated accordingly.

To generate the Portugal tax audit file, see [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html). Ensure that you first configure your TAF Enhanced Trial Balance Saved Reports before generating tax audit files. For more details about generating tax audit files, see [Generating a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077452.html).

Some data in the generated XML may be truncated by the system if they exceed the maximum length defined in the schema.

If you're generating an audit file covering a long period of time or a large volume of transactions, you should run the PT SAF-T overnight because the audit file generation may take several hours to complete.

### Additional Information

-   [Portugal Localization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161822794592.html)
-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)

### Related Topics

-   [Setting Up the PT SAF-T](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3958232661.html)
-   [Field Mapping for Portugal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497423852.html)
-   [Formatting Portugal PDF Documents](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1972506.html)
-   [Portugal Standard Audit File for Tax Purposes (PT SAF-T)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1971159.html)
-   [Portugal Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1973379.html)
-   [Portugal VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1974556.html)
-   [EU Sales List for Portugal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1978248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

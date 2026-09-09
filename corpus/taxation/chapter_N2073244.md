---
id: "chapter_N2073244"
type: "chapter"
title: "Tax Audit Files"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Tax Audit Files"
parent: "preface_3710626699"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html"
anchors: []
sha256: "8381928d3df74d81ed92f9ce984cc345b7811bbaf364b8bdd34b8c4e9aa8e551"
---

Important:

Tax Audit Files SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

Tax authorities in different countries ask for a general ledger (GL) data for auditing purposes to verify if businesses are reporting their tax returns correctly. Taxpayers can give this electronic record to tax auditors to support their tax returns and review their accounting records.

With the Tax Audit Files SuiteApp, you can export general ledger data in a format that meets government requirements.

| Supported Tax Audit Files | Description | Related Help Topic |
| --- | --- | --- |
| Malaysia GST Audit Files | The Malaysian tax bureau, Jabatan Kastam Diraja Malaysia (JKDM), requires local businesses to submit their tax data for GST compliance audits. With Tax Audit Files, you can generate the Malaysia GST Audit File (GAF) in the format JKDM requires. The file is available in XML or text file format, and can be submitted to JKDM. | [Malaysia GST Audit File (GAF)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4228553324.html) |
| Mexico DIOT File | The Mexico tax authority, Servicio de Administración Tributaria (SAT), requires taxpayers to submit the Mexico Declaración Informativa de Operaciones con Terceros (DIOT) File to declare third-party transactions. SAT requires taxpayers to submit a monthly declaration of all third-party transactions, with details of the applicable value-added tax. With Tax Audit Files, you can generate DIOT files that meet SAT's requirements. You can also submit this online using the DIOT\_11 software. | [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html) |
| Mexico Electronic Accounting File | The Second Amendment to the Temporary Tax Regulations defines the tax reporting requirements for accounting information in Mexico. Under these rules, taxpayers in Mexico must file accounting information with the tax authorities every month. With Tax Audit Files, you can generate Mexico Electronic Accounting File records that meet the tax authority's requirements. | [Mexico Electronic Accounting File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4219758919.html) |
| Norway SAF-T Financial | The Norway Standard Audit File for Tax (SAF-T) is a standard file format for exporting various accounting transactional data in XML. The report structure is based on the Organization for Economic Cooperation and Development or OECD's SAF-T standard. | [Norway Standard Audit File for Tax (SAF-T) Financial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_43132133850.html) |
| Philippines RR No. 09-2009 Audit Files | Businesses in the Philippines must generate and export tax audit files in the format set by the Bureau of Internal Revenue (BIR) in Revenue Regulations No. 09-2009. With Tax Audit Files, you can generate the following data in the format required by RR No. 09-2009:
-   General Ledger
-   General Journal
-   Sales Journal
-   Purchase Journal
-   Cash Receipts Journal
-   Cash Disbursements Journal
-   Inventory Book

 | [Philippines Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967465.html) |
| Singapore IAF | The IRAS Audit File (IAF) is a standard electronic file that the Inland Revenue Authority of Singapore (IRAS) requests businesses for audits. IRAS conducts periodic audits to ensure that tax returns are being prepared correctly. If selected, a Singapore company must submit a detailed breakdown of its business transactions through the IAF. IRAS doesn't assume that a business has made GST errors if it's selected for audit. Audits are conducted on a broad range of industries to check overall compliance. You should keep sales and purchases listings that support the figures reported in your GST returns. Acceptable IAF formats are flat files that can be either XML or pipe delimited text files, and the Tax Audit Files SuiteApp supports both. You can generate an IAF file from data entries in your general ledger or chart of accounts, along with customers and supplier data, and details of invoices, orders, payments, and adjustments. | [Singapore Tax Topics for Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1981261.html) |
| Spain Online VAT Register Reports | The Spain tax agency (Agencia Estatal de Administración Tributaria) requires companies to submit issued and received invoices electronically through their online system. With Tax Audit Files, you can generate reports in the format the tax authority requires. | [Spain Online VAT Register](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1496817614.html) |
| OECD SAF-T | For many countries, the Organisation for Economic Co-operation and Development (OECD) has issued the Standard Audit File for Tax (SAF-T) standard to assist auditors in determining if a business has paid the correct tax at the right time, following local tax laws. It results from a specification of one of the principles set out in the [Guidance on Tax Compliance for Business and Accounting Software](http://www.oecd.org/ctp/taxadministration/34910263.pdf). The NetSuite SAF-T in XML meets the OECD's minimum requirements and can be submitted to tax authorities. The file captures the following data from several areas found in your general ledger or chart of accounts:

-   Master data of customers and suppliers
-   Details of invoices, orders, payments and adjustments

 | [Guidance on Tax Compliance for Business and Accounting Software](http://www.oecd.org/ctp/taxadministration/34910263.pdf) |
| United Arab Emirates FTA VAT Audit File | The United Arab Emirates tax authority, Federal Tax Authority (FTA), audits businesses to make sure tax declarations are accurate and on time. As part of the audit, business must provide accounting information to validate their submitted tax declarations. The FTA VAT Audit File (FAF) is an export of accounting entries in CSV file with a format specified by the FTA. This is based on general ledger chart of accounts entries, master file data for customers and suppliers, and details of invoices, payments, and adjustments. | [United Arab Emirates Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539749458.html) |
| GL Data Extract | Important: Before you generate a GL data extract, make sure the GL Audit Numbering feature is enabled and you've run the GL numbering sequence. Otherwise, file generation and download will fail. For more information, see [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html) and [Running GL Audit Numbering Sequences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4805209975.html). With Tax Audit Files, you can generate a general ledger data extract (GL Data Extract) that can be used by any country for audit purposes. The extract includes key transaction data such as posting date, account, debit and credit amounts, document currency, reporting currency, and more in CSV format. Note: If the generated CSV file has special characters, the data won't display correctly and may have inaccurate information when viewed in Microsoft Excel. To avoid this, make sure your transaction line items don't have special characters. | [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html) [Running GL Audit Numbering Sequences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4805209975.html) [Adding Custom Fields to GL Data Extracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078555.html) |

To use the Tax Audit Files SuiteApp, read the following help topics:

-   [Prerequisites for Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_98164624128.html)
    
-   [Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074100.html)
    
-   [Creating or Customizing Roles to Use Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074456.html)
    
-   [Setting Up Tax Audit Files to Use Multiple Queues or Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4361709092.html)
    
-   [Setting Up Threshold Configuration on Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1516603486.html)
    
-   [Setting Tax Audit Files Report Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158080650603.html)
    
-   [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html)
    
    -   [Generating a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077452.html)
        
    -   [Troubleshooting Tax Audit File Generation Failures](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077778.html)
        
    -   [Downloading a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078033.html)
        
    -   [Deleting a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078309.html)
        
    -   [Adding Custom Fields to GL Data Extracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078555.html)
        
    -   [Statutory Chart of Accounts for Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3929759676.html)
        

For country-specific information about tax audit files, read the following topics:

-   [Malaysia GST Audit File (GAF)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4228553324.html)
    
-   [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html)
    
-   [Mexico Electronic Accounting File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4219758919.html)
    
-   [Norway Standard Audit File for Tax (SAF-T) Financial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158945380851.html)
    
-   [Philippines Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967465.html)
    
-   [Singapore Tax Topics for Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1981261.html)
    
-   [Spain Online VAT Register](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1496817614.html)
    
-   [United Arab Emirates Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539749458.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

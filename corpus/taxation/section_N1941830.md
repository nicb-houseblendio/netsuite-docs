---
id: "section_N1941830"
type: "section"
title: "Mexico DIOT File (Mexico Compliance SuiteApp)"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Mexico Tax Topics (Mexico Compliance SuiteApp) > Mexico DIOT File (Mexico Compliance SuiteApp)"
parent: "chapter_N1940317"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html"
anchors: ["bridgehead_3738830551", "bridgehead_N1941919", "procedure_N1941929"]
sha256: "2ddff34502f65b68b0e70f2d716e8390ae369502952ddf17c43abff004268eb5"
---

Important:

To use the Mexico DIOT reporting feature, you must install the Mexico Compliance SuiteApp, the Tax Audit Files SuiteApp, and the International Tax Reports SuiteApp. See [Installing SuiteApps for Mexico](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1940317.html#bridgehead_3738744847).

In Mexico, taxpayers must submit a monthly declaration of all payments made to third parties, with details of the applicable value added tax.

Using the NetSuite Tax Audit Files SuiteApp, you can generate a Declaración Informativa de Operaciones con Terceros (DIOT) file that conforms to the requirements specified by the Mexican tax authority Servicio de Administración Tributaria (SAT), and can be submitted online to SAT using the DIOT\_11 software.

The Mexico DIOT file is a text file that contains a list of all payments made by a subsidiary to third parties within a selected period, and includes details of applicable value added tax. Only transactions with IVA (VAT) relevant tax codes are included in the DIOT file. If a transaction has no tax code, or if the tax code is marked as Exclude from VAT reports, the transaction will not be included in the DIOT file. Tax codes for Mexico are described in the [Tax Code Table for Mexico](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1940638.html#bridgehead_N1940696). For information about transactions included in the DIOT file, see [Tax Code Mapping for Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3738825237.html).

For vendor bills, only those that have been paid (through any of the payment transactions) and reconciled with the bank account will be included in the DIOT file.

Important:

The DIOT report shows only cleared transactions. Be sure to reconcile transactions before generating the DIOT report. For more information about reconciling bank statements, see [Bank Account Reconciliation and Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1552053.html).

## Required Fields for Mexico DIOT Reporting {#bridgehead_3738830551}

For DIOT reporting, you must complete the following fields on entity and transaction records for companies or subsidiaries in Mexico:

-   **Billing address Country field on the vendor record**
    
    In the DIOT file, vendors must be classified as national vendor, foreign vendor, or global vendor. Be sure to provide a value in the Country field of the vendor billing address. Currently, NetSuite cannot identify global vendors.
    
-   **Mexico RFC field on the employee, vendor, and customer record**
    
    If there is no value in the RFC code field on the employee record, vendor record, and customer record, the DIOT report also shows an empty RFC field for the entity.
    
-   **Operation Type field**
    
    Each transaction must have an indication of its operation type, which could be Professional Services, Real Estate Leasing, or Others. If you do not enter a value, the DIOT report uses Others as the default operation type for the transaction.
    
-   **Vendor field**
    
    In the DIOT file, all lines on expense reports must indicate the name of the vendor or supplier.
    

Note:

For information about custom fields and validations for Mexico, see [Mexico Compliance Features (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3738749895.html).

## Generating the Mexico DIOT File {#bridgehead_N1941919}

#### To generate a Mexico DIOT file: {#procedure_N1941929}

1.  Go to Reports > Tax > Audit Files.
    
2.  Select DIOT (Text) from the Report dropdown.
    
3.  If you are using a OneWorld account, select the Mexico parent company or a Mexico subsidiary company.
    
4.  Select an accounting period.
    
5.  Click Generate.
    
    The system queues the process for generation, and then notifies you by email when the audit file has been generated. The email notification includes a link to the downloadable file. During the time that the tax audit file is being generated, you can see its progress in the Download column of the Audit Files table. Click Refresh to update the Download column. When file generation is complete, the Download status displays a link to the downloadable file.
    
6.  To generate a new report, click Reset and repeat steps **2** to **5**.
    
7.  When a Mexico DIOT file has been successfully generated, you can download it for submission to Servicio de Administración Tributaria. To download, see [Downloading a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078033.html). To delete a DIOT file, see [Deleting a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078309.html).
    

The System Notes subtab makes a record of everything you do using the Tax Audit Files SuiteApp (create, delete, cancel, generate, and download), including user names and dates. Specific file details are also recorded, such as period, subsidiary, and report type.

For information about roles and permissions to use the Tax Audit Files SuiteApp, see [Creating or Customizing Roles to Use Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074456.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Mexico Tax Setup (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941750.html)
-   [Mexico Tax Codes (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1940638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

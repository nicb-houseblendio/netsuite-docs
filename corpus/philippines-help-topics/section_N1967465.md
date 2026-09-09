---
id: "section_N1967465"
type: "section"
title: "Philippines Tax Audit Files"
branch: "philippines-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Philippines Help Topics > Philippines Tax Topics > Philippines Tax Audit Files"
parent: "chapter_N1950898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967465.html"
anchors: ["bridgehead_3808798763", "bridgehead_29161803781", "bridgehead_0808095943"]
sha256: "309a1dcf91981995d6be333cb701ebb25f81948d7239d7c618324cf0b89e1ac9"
---

The Tax Audit Files SuiteApp lets you generate and export audit files in the format defined by the Bureau of Internal Revenue (BIR) in Revenue Regulation 09-2009.

Revenue Regulation 09-2009 defines the requirements for the maintenance, retention, and submission of electronic records. If requested, companies or subsidiaries that do business in the Philippines must make their audit files available to the BIR.

Using the Tax Audit Files SuiteApp, you can generate audit files per subsidiary, or a group of subsidiaries if you're using a OneWorld account. For steps to generate a tax audit file, see [Generating a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077452.html).

## Philippines RR09-2009 Audit Files {#bridgehead_3808798763}

NetSuite provides Philippines RR09-2009 audit files composed of the following data exports in CSV format:

-   [Philippines General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_63125735788.html)
    
-   [Philippines General Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_50130518656.html)
    
-   [Philippines Sales Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_11131220910.html)
    
-   [Philippines Purchase Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_22132003997.html)
    
-   [Philippines Cash Receipts Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_19132705522.html)
    
-   [Philippines Cash Disbursement Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_67133514002.html)
    
-   [Philippines Inventory Book](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_17134537447.html)
    

Note:

For the Inventory Book, if your NetSuite account does not have the **Inventory** feature enabled, the Amount column shows blank values. Similarly, if your account does not have the **Multiple Units of Measure** enabled, the Unit column shows blank values.

## Audit Files Headers {#bridgehead_29161803781}

The following table lists the headers available for Philippines Tax Audit Files.

| Report Header | Description |
| --- | --- |
| Taxable Year | Displays the year entered in the **Period** and **To** fields. |
| Company Name | Displays the registered name of the company. |
| Company Address | Displays the address of the company. |
| VAT REG TIN or NON-VAT REG TIN | Displays the VAT or NON-VAT registered Tax Identification Number (TIN) entered in the account. See [VAT REG TIN or NON-VAT REG TIN Header](#bridgehead_0808095943). |
| PTU No. / AC Control No. | Displays the Permit to Use (PTU) number or Acknowledgment Certificate Control Number (ACCN) issued by the BIR. |
| PTU / ACCN Issue Date | Displays the issue date of the PTU or ACCN. |
| Software Name | Displays the Oracle NetSuite version used to generate the report. |
| File Name | Displays the default name of the report. |
| File Type | Displays the file type of the report. The default file type for Philippines report is CSV. |
| Number of Records | Displays the total number of transactions in the report. |
| Amount Field Control Total | Displays the sum of all transaction amounts and is used to ensure all data was included and calculated correctly. |
| Period Covered | Displays the date range based on the selected time period. |
| Run Date | Displays the date and time the report is generated. |
| Extracted by | Displays the ID of the user that generated the report. |

## VAT REG TIN or NON-VAT REG TIN Header {#bridgehead_0808095943}

The **PH Seller Type** field in your Subsidiary or Company record determines which registered TIN header appears in most audit files. If you have the Southeast Asia (SEA) Localization SuiteApp installed, the system automatically retrieves this information from the SuiteApp and populates it in the **Philippines Invoicing** subtab. Otherwise, you need to enter these taxpayer registration details manually in the **Philippines Invoicing** subtab.

#### To manually add taxpayer details:

1.  If you have a OneWorld account, go to Setup > Company > Classifications > Subsidiaries, then click the **Edit** link of the Philippines subsidiary.
    
    If you don't have a OneWorld account, go to Setup > Company > Company Information.
    
2.  Click the **Philippines Invoicing** subtab.
    
3.  Enter values for the following fields:
    
    -   **PH Seller Type** - Specify whether your company is VAT Registered or Non-VAT Registered.
        
    -   **CAS Document Issued by BIR** - Select either Permit to Use (PTU) or Acknowledgment Certificate (AC).
        
    -   **PTU No.** - Enter the PTU number issued by the BIR.
        
    -   **PTU Date Issued** - Enter the date when the PTU was issued to your company.
        
    -   **AC Control No. (ACCN)** - Enter the AC Control No. (ACCN) in the format AC\_RDO\_MMYYYY\_XXXXXX, where:
        
        -   AC - Means Acknowledgement Certificate
            
        -   RDO - The 3-character alphanumeric RDO Code, for example, 038, 044, 132, 17A, 21C
            
        -   MM - Month that the Acknowledgement Certificate was prepared or issued
            
        -   YYYY - Year that the Acknowledgement Certificate was prepared or issued, must be 2020 onwards
            
        -   XXXXXX - Is a 6-digit number series
            
    -   **ACCN Issue Date** - Enter the date when Acknowledgement Certificate was issued to your company.
        

Note:

The system uses the **VAT Registered** setting to determine which registered TIN header appears with the corresponding 9-digit registered TIN in the Inventory Book. If the box is checked, the **VAT REG TIN** header appears. Otherwise, the **NON-VAT REG TIN** header appears. For more information, see [Setting Up Tax Filing for the Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1955261.html)

### Related Topics

-   [Prerequisites for Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_98164624128.html)
-   [Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074100.html)
-   [Creating or Customizing Roles to Use Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074456.html)
-   [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html)
-   [Generating a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077452.html)
-   [Adding Custom Fields to GL Data Extracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078555.html)
-   [Troubleshooting Tax Audit File Generation Failures](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077778.html)
-   [Downloading a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078033.html)
-   [Deleting a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078309.html)
-   [VAT Reports - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1955015.html)
-   [VAT RELIEF Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1955531.html)
-   [Philippines General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_63125735788.html)
-   [Philippines General Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_50130518656.html)
-   [Philippines Sales Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_11131220910.html)
-   [Philippines Purchase Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_22132003997.html)
-   [Philippines Cash Receipts Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_19132705522.html)
-   [Philippines Cash Disbursement Journal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_67133514002.html)
-   [Philippines Inventory Book](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_17134537447.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

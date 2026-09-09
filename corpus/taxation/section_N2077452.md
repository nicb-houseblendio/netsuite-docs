---
id: "section_N2077452"
type: "section"
title: "Generating a Tax Audit File"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Tax Audit Files > Using Tax Audit Files > Generating a Tax Audit File"
parent: "section_N2077183"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077452.html"
anchors: ["procedure_158624493426", "procedure_N2077460"]
sha256: "2d1f8a4923a7606cc6f781736659e4551dbc1533129484f84d987cab547f24b3"
---

Before you can generate tax audit files, you'll need to configure your TAF Enhanced Trial Balance Saved Reports.

Note:

The configuration steps apply to the following tax audit files and reports:

-   Mexico Trial Balance report
    
-   Mexico Complementary Trial Balance report
    
-   Mexico Auxiliary Report of Accounts
    
-   Portugal Standard Audit File for Tax Purposes (SAF-T)
    
-   Portugal SAF-T Invoicing
    
-   Portugal SAF-T Accounting
    

#### To Configure TAF Enhanced Trial Balance Saved Reports: {#procedure_158624493426}

1.  Go to Reports > Saved Reports > TAF Enhanced Trial Balance > Customize.
    
2.  On the Report Builder page, click Edit Columns.
    
3.  In the Report Preview pane, do the following:
    
    -   Click the **Last Debit** column.
        
        -   On the **Alternate Period Range Type** dropdown list, select **Relative to report date**.
            
        -   Check the **Cumulative Value** box.
            
        -   Click the **Alternate Period Range** popup list. Select **This Period**.
            
    -   Click the **Last Credit** column.
        
        -   On the **Alternate Period Range Type** dropdown list, select **Relative to report date**.
            
        -   Check the **Cumulative Value** box.
            
        -   Click the **Alternate Period Range** popup list. Select **This Period**.
            
    -   Click the **Current Debit** column.
        
        -   On the **Alternate Period Range Type** dropdown list, select **Relative to report date**.
            
        -   Click the **Alternate Period Range** popup list. Select **This Period**.
            
    -   Click the **Current Credit** column.
        
        -   On the **Alternate Period Range Type** dropdown list, select **Relative to report date**.
            
        -   Click the **Alternate Period Range** popup list. Select **This Period**.
            
4.  Click **Save**.
    

#### To generate a tax audit file: {#procedure_N2077460}

1.  Go to Reports > Tax > Audit Files.
    
2.  On the Audit Files page, set values for the following fields:
    
3.  Provide values for the following fields:
    
    -   **Report** - Select a tax audit file to generate.
        
    -   **Subsidiary** (for OneWorld accounts) - Select the subsidiary you want to generate a tax audit file report for. The dropdown list only shows subsidiaries your role can access.
        
    -   **Period** - Select the starting period for the report.
        
    -   **To** - Select the ending period for the report.
        
    -   **Group** (for OneWorld accounts) - Check this box if your tax authority allows group reporting. Group reporting includes data from child subsidiaries.
        
    -   **Accounting Book** - Select the accounting book that will be used to generate the report. The dropdown list shows active accounting books associated with the selected subsidiary.
        
        Note:
        
        The following features aren't supported right now:
        
        -   Group reporting for secondary accounting books
            
        -   Advanced intercompany journal entries
            
        
    -   **Accounting Context** - Select the applicable accounting context for the report. The generated file uses information from the selected accounting context to map the account name and numbers.
        
        Note:
        
        The Accounting Context filter becomes available if you've defined at least one accounting context in your account. For more information, see [Accounting Contexts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4640155582.html).
        
4.  Click **Generate**.
    
    The system queues the file for generation. When it's done, NetSuite sends you an email that includes a link to download the file. When the tax audit file is being generated, you can see its progress in the Download column of the Audit Files table. Click **Refresh** to update the column. When it's finished, you'll see a download link.
    
    If file generation fails, see [Troubleshooting Tax Audit File Generation Failures](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077778.html).
    
5.  To generate a new report, click **Reset** and repeat steps **2** to **3**.
    

You can download the successfully generated tax audit file and save it on your computer for submission to your tax authority. To download a tax audit file, see [Downloading a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078033.html).

### Related Topics

-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)
-   [Prerequisites for Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_98164624128.html)
-   [Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074100.html)
-   [Creating or Customizing Roles to Use Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074456.html)
-   [Setting Up Tax Audit Files to Use Multiple Queues or Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4361709092.html)
-   [Setting Up Threshold Configuration on Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1516603486.html)
-   [Setting Tax Audit Files Report Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158080650603.html)
-   [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html)
-   [Troubleshooting Tax Audit File Generation Failures](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077778.html)
-   [Downloading a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078033.html)
-   [Deleting a Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078309.html)
-   [Adding Custom Fields to GL Data Extracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2078555.html)
-   [Statutory Chart of Accounts for Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3929759676.html)
-   [France Fichier d'Ecritures Comptables (FEC)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3929748561.html)
-   [Germany GoBD Data Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3838969498.html)
-   [Malaysia GST Audit File (GAF)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4228553324.html)
-   [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html)
-   [Mexico Electronic Accounting File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4219758919.html)
-   [Philippines Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967465.html)
-   [Portugal Standard Audit File for Tax Purposes (PT SAF-T)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1971159.html)
-   [Singapore Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html)
-   [United Arab Emirates Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539749458.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

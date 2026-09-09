---
id: "section_N745334"
type: "section"
title: "Exporting a Saved Report as an Excel Web Query"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Exporting a Saved Report as an Excel Web Query"
parent: "chapter_N736328"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745334.html"
anchors: ["procedure_N745358"]
sha256: "cd8d979fe012c19d8ea8585f07dfd6bf5f549a396a42853b9e8ebf98311e397b"
---

You can export a saved report as an Excel Web Query. When the report is exported, data can be refreshed from within Microsoft® Excel with the latest information from your NetSuite account.

Important:

Web Query functionality is not available for financial statements. You won't see the Allow Web Query option for the following reports: Income Statement, Income Statement Detail, Comparative Income Statement, Balance Sheet, Balance Sheet Detail, Comparative Balance Sheet, Cash Flow Statement, Budget Income Statement, Budget Income Statement Detail, Budget vs. Actual, Cash Statement, and Cash Statement Detail.

#### To create an Excel Web Query: {#procedure_N745358}

1.  Start the Report Builder by clicking Customize on any report or by clicking **Edit** next to a report name on a list of saved reports.
    
2.  On the Report Builder page, click **More Options**.
    
3.  Check the **Allow Web Query** box.
    
4.  Click **Save**.
    
5.  Verify that you want to overwrite the previously saved version of the report.
    
    If you don't want to overwrite the previous version, you can save the report with a different name. Click **Cancel**, rename the report and click **Save As**.
    
6.  After the report runs, select **Export-Excel Web Query** in the footer.
    
    The report is saved as an .iqy file.
    
7.  In the File Download window, you can click **Open** or **Save** if you are running on a PC. If you are running on a Mac, save the file.
    
    -   If you've saved an .iqy file on a PC, you have to double-click it to run it in Microsoft® Excel.
        
    -   If you've saved an .iqy file on a Mac, first start Microsoft® Excel, then import the file manually by going to Data > Get External Data > Run Saved Query, and selecting the .iqy file.
        
8.  The .iqy file opens in Microsoft® Excel. In the Enter Parameter Value window, enter the email address you use to log in to your NetSuite account. Or, if you didn't create the Web query, use the email address of the person who did. Check the option if you want, and click **OK**.
    
    Note:
    
    The email address is case sensitive.
    
    -   Your data loads into Microsoft® Excel.
        
    -   Click **Refresh Data** to get the latest data from your NetSuite account.
        

**Notes:**

-   Use caution when checking the **Use this value/reference for future refreshes** box. Checking the box enables you and anyone with access to the report to refresh it from Microsoft® Excel any time without having to reenter an email address. The only way to deny future access is to leave this box cleared, clear the Allow Web Query box, or delete the saved report.
    
-   If you plan to send a Web query to others, be aware that IP address rules may prevent them from accessing it. For example, if IP address rules are defined when you create a Web query, users logging in from other IP addresses won't be able to access it. For information about these rules, see [Enabling and Creating IP Address Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4726612641.html).
    
-   When a user accesses a Web query created by someone else, a mismatch in usage information occurs in login audit trail information and related saved searches. The user name is recorded as the creator of the saved report exported as a Web query, but the IP address belongs to the other person who accessed the query.
    
-   If you export a report as an Excel Web Query (.iqy) file when you're logged in using SAML Single Sign-on, the file may not be able to retrieve data from NetSuite. In this case, you need to log in to NetSuite using the NetSuite login page and export the report again.
    

Warning:

Make sure that you're not breaching your organization's security policy before sharing .iqy files with others. The files are personalized and generated for your use only. Anyone you share the file with can run the report at any time and see the same live data you can, even if their role wouldn't normally give them access. The only thing needed to view the report is the email address used to create it, which could be guessed by the recipient.

### Related Topics

-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Report Builder Interface](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736822.html)
-   [Report Customization Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738489.html)
-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)
-   [Formatting Numbers on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741457.html)
-   [Filtering Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742381.html)
-   [Sorting Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N743154.html)
-   [Setting Additional Options for Custom Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744268.html)
-   [Arranging Data on Summary Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4353206428.html)
-   [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html)
-   [Sharing Custom Reports with Other Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745002.html)
-   [Example Report Format Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745576.html)
-   [Saving a Custom Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513909963.html)
-   [Deleting a Custom Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4224521464.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

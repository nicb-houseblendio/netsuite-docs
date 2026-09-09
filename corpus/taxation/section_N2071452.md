---
id: "section_N2071452"
type: "section"
title: "Generating an EU Intrastat Report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > European Union (EU) Tax Topics > EU Intrastat Report > Generating an EU Intrastat Report"
parent: "section_N2069213"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2071452.html"
anchors: ["procedure_N2071494", "bridgehead_4180161062", "bridgehead_N2071647"]
sha256: "714dbe0c552e843812a5bd6d7b95b27d1a398e7e968757957409092b2fd1f731"
---

The EU Intrastat Report collates the information for the monthly Intrastat Supplementary Declaration form for goods sold to or purchased from another EU member state. You can directly send the information to your tax agency or save the report as a CSV file and submit electronically, if your country allows it.

#### To generate an EU Intrastat Report: {#procedure_N2071494}

1.  Go to Reports > VAT/GST > EU Intrastat Report.
    
2.  Select a subsidiary.
    
3.  In the **Report Type** field, select **Sale** for Dispatches or **Purchase** for Arrivals.
    
4.  Select a country form.
    
5.  Select a reporting period. Using the date selector, select the start date in **Tax Period** and the end date in **To**. Note that Intrastat reports are submitted monthly.
    
6.  In the **Accounting Book** field, select which accounting book will be used to generate the report. The dropdown list shows all active books associated with the selected subsidiary.
    
    Note:
    
    This field is available if the Multi-Book Accounting feature is enabled in your account. For more information, see [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html).
    
7.  To display the report, click **Refresh**. You need to click **Refresh** each time you change the reporting criteria.
    
    Important:
    
    For saved reports in the International Tax Reporting SuiteApp, results are limited to 25,000 rows. You'll see the following note at the bottom of truncated reports:
    
    'The results of this report are too large. Please narrow your results.' If you want to request for an increase in the limit, you'll need to file a support case through the NetSuite Partner Center.
    
    The following countries have specific conditions for transaction consolidation in saved reports:
    
    -   For the Netherlands, transaction lines with values less than 200 Euros are consolidated per member state and declared as one transaction. For consolidated transactions, the value of Commodity Code is 9950 0000. Credit memos and vendor credits aren't consolidated. Instead, the report displays the amounts as negative numbers for these transactions.
        
    -   For Belgium, transaction lines with the same values of Commodity Code, Member State, NOTC, Region of Origin, Mode of Transport, and Incoterm are consolidated and declared as one transaction. For consolidated transactions, Net Mass, Value in Euro, and Supplementary Unit columns are added.
        
    -   For Denmark, transaction lines with the same values of Commodity Code, Member State, and NOTC are consolidated and declared as one transaction.
        
    
8.  Review the report. Take note of the following when reviewing reports:
    
    -   Review all pages of the report.
        
    -   to To specify the number of rows displayed on each page, go to the **General** subtab in _Home > Set Preferences_.
        
    -   Column headers vary depending on the country form selected.
        
    -   For some country forms, you can click the customer name to view the customer record or the reference number to view the transaction.
        
9.  Check the **Exclude** box for each transaction you want to leave out of your report. You can also click **Mark All** or **Unmark All**.
    
10.  To save the report, click any of these options:
     
     -   **Print** - Generates a PDF version you can print or save. Lines with the Exclude box checked aren't included in the PDF.
         
     -   **Export to Excel** - Saves the Intrastat report as a Microsoft Excel (.xls) file. Lines with the Exclude box checked aren't included in the file.
         

## Electronic Filing of Intrastat Reports {#bridgehead_4180161062}

For Belgium, Denmark, Finland, Germany, the Netherlands, and United Kingdom, NetSuite's International Tax Reports SuiteApp lets you export Intrastat reports in a format acceptable for upload to the tax agency website.

You can export the report in electronic format and upload it to the tax agency website. These are the formats used for EU Intrastat Filing:

-   If you select a Netherlands subsidiary on the EU Intrastat Report page, click **Export to ASCII** to generate an ASCII file.
    
-   For Belgium, Finland, Germany, or UK subsidiaries, on the EU Intrastat Report page, click **Export to CSV** to generate a CSV file.
    
    Important:
    
    When prompted to open or save a CSV file, click **Save File**. Don't open it in Excel first because it can change the format. Save it first, and if you want to view it, use a text editor like Notepad.
    
-   For a Belgium subsidiary on the EU Intrastat Report page, click **Export to XML** to generate an XML file of the report.
    
-   For a Denmark subsidiary on the EU Intrastat Report page, click **Export to Excel** to generate an XLS file of the report.
    

## EU Intrastat Reports {#bridgehead_N2071647}

You can customize the following EU Intrastat reports and use it for any EU country. The reports are available from Reports > Saved Reports.

-   Intrastat Purchases Report \[Custom\]
    
-   Intrastat Sales Report \[Custom\]
    

For information about how to customize a report, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).

### Related Topics:

-   [EU Sales List (ESL) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068052.html)
-   [Intrastat Report Dispatches and Arrivals Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070008.html)
-   [Generating an EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2071452.html)
-   [Intrastat Report for Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587020795.html)
-   [Intrastat Report for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1552962932.html)
-   [Intrastat Report for Denmark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505371864.html)
-   [Intrastat Report for Finland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504769975.html)
-   [France Intrastat Declaration of Exchange of Goods (DEB) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157018267486.html)
-   [Intrastat Report for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4149981058.html)
-   [Intrastat Report for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503450407.html)
-   [Intrastat Report for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035309.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

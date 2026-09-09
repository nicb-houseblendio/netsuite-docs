---
id: "section_N2068441"
type: "section"
title: "Generating an EU Sales List Report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > European Union (EU) Tax Topics > EU Sales List (ESL) Report > Generating an EU Sales List Report"
parent: "section_N2068052"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068441.html"
anchors: ["procedure_N2068549"]
sha256: "73e4c03d8bd0b29e612f7a2a1426ef237fc6fa02b92552c9189b3336fed12cda"
---

With the International Tax Reports SuiteApp, you can generate reports for European Union (EU) countries. Before you try to generate an EU sales list report, make sure you have the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) SuiteApp installed in your account.

Important:

If you've entered your EU customers' VAT registration number and country correctly, and used the right VAT tax code on your sales transactions, that data will be generated on the reports. It's your responsibility to make sure your customers' and vendors' VAT registration IDs are validated against the Europa database (or an alternative database if you have one). You can do this by clicking the VIES link on the Financial tab of the customer record. If there's no VAT number specified on the customer record, NetSuite will show an error on the report. If a subcustomer record doesn't have a VAT number, NetSuite will use the parent customer's VAT number.

Important:

Make sure every customer record has a shipping address, as the tax rules on reporting are based on the **Ship To** address. If there's no shipping address, NetSuite will use the **Bill To** address from the customer record. If the invoice is charged to a project, NetSuite will use address saved from the customer record associated with the project.

#### To generate an EU Sales List Report: {#procedure_N2068549}

1.  Go to Reports > VAT/GST > EU Sales List Report.
    
2.  Select a subsidiary.
    
3.  Check the **Group** box if you want a consolidated report that includes child subsidiaries. Use this if your company is part of a VAT group.
    
4.  Select a country form.
    
5.  Select a reporting period by entering the **Tax Period** From and To dates. You can select a month or a quarter.
    
6.  In the **Accounting Book** field, select which accounting book to use to generate the report. This field becomes available if the Multi-Book Accounting feature is enabled. The dropdown list shows all active books associated with the selected subsidiary. For more information, see [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html).
    
7.  To display the report, click **Refresh**.
    
    Whenever you change the reporting criteria such as the tax period, click **Refresh** to reload the report.
    
8.  Review the report.
    
    -   Make sure you review all pages of the report. To set how many rows show on each page, go to the **General** subtab in _Home > Set Preferences_.
        
    -   Click the customer names to view the customer records.
        
    -   For the **Country Code** column, NetSuite gets the value from the customer's VAT registration number. If the customer has a defined VAT registration number with a country code prefix, NetSuite displays this prefix. The country code is blank if the defined VAT registration number has no prefix.
        
    -   If you're generating a report for Italy, you can click the **Invoice Number** links to view the transaction records.
        
    
    Important:
    
    Saved reports in the International Tax Reporting SuiteApp are limited to 25,000 rows. If your report is too big, a truncated report will be generated. At the bottom of the page, you'll see the note 'The results of this report are too large. Please narrow your results.' If you want a higher limit, you'll need to file a Support case.
    
9.  Make sure you verify and correct data as necessary. If NetSuite finds any inconsistencies based on your reporting criteria, you'll see them marked with color codes on the ESL report. By default, the **Exclude** box is checked for transactions with data inconsistencies, except for VAT number errors.
    
    The following table lists the color codes and their description.
    
    ![Screenshot of the Legend information on the EU Sales List report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/EUSalesListLegend.png)
    
    | Code | Definition |
    | --- | --- |
    | Customer is in same country | If the customer name is red, it means that the country of the EU Sales List form and the country on the customer's transaction record are the same. Make sure that you have used the correct shipping country on the transaction. |
    | Non-EU country transaction | If the customer name is brown, it means that the country in the shipping address of the transaction record isn't an EU country. Make sure that you have used the correct shipping country on the transaction. |
    | Customer without valid VAT ID/shipping address | If the customer name is blue, it means that there's no identified shipping or billing address on the customer's transaction record. If VAT number is blue, it could mean that the VAT country code does not match the country indicated on the shipping address, or it could mean that the VAT number isn't in the correct format for that country. |
    
    Note:
    
    Each EU country has its own VAT prefix and numbering format. For more information, refer to this [VAT identification number structure](http://ec.europa.eu/taxation_customs/vies/faqvies.do) published by the European Commission.
    
10.  Check the **Exclude** box for any lines you want to leave out of your report, or clear it for lines you want to include in the report. You can also check the box in the column header to exclude all lines on the current page.
     
11.  In the **Indicator** column for each line, review the transaction type, and edit it if necessary:
     
     -   **B2B Goods** - products that you deliver directly to a customer.
         
     -   **Triangulated Goods** - sales that involve supplies of goods between three VAT-registered traders in three different EU member states. This is the default indicator for transactions that you marked as part of an EU triangulation deal. For more information, see [Identifying EU Triangulated Goods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4380703631.html).
         
     -   **Services** - services that you provided to your customer.
         
12.  To select a page to view, use the paging toolbar at the bottom of the page. Click the arrows to go to the next page, or type a page number and press **Enter**.
     
13.  To save the report, click any of the following options. Lines with the **Exclude** box checked aren't included in the exported file.
     
     -   **Print** - makes a PDF version of the report that you can print or save for your records.
         
     -   **Export** - saves the ESL report as a Microsoft Excel (.xls) file.
         
     -   **Export to XML** - generates an XML file of the ESL report that you can submit for electronic filing. This option is available only for Austria, Belgium, Czechia, and Ireland.
         
         Important:
         
         For Belgium, you can only generate an XML file for a monthly or quarterly tax period. The tax period specified in the **From** and **To** fields must match.
         
     
     The following options are for UK only:
     
     -   **Export (HMRC)** - converts the ESL into a CSV file that complies with the format required by the UK tax agency (HMRC). When prompted, click **Save File**. Don't open it in Excel, or the format will change and may result in submission errors. Save it, and if you want to view it, use a text editor such as Notepad.
         
     -   **Submit Online** - submits the EU sales list directly to the UK tax agency (HMRC).
         
         Before you submit the EU Sales List Report for UK, you'll need to update the URL in the system.
         
         #### To update the URL:
         
         1.  Go to Reports > VAT/GST > EU Sales List Report.
             
         2.  On the EU Sales List (ESL) Report page, click **Setup** and select **EU Sales Filing**.
             
         3.  On the EU Sales Filing Setup window, click **Save**.
             
         
     
     For more information about ESL online filing for UK, see [EU Sales List for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2032559.html) and [Submitting an EU Sales List (ESL) Online in the United Kingdom to HMRC](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034464.html).
     
     Note:
     
     NetSuite also saves a copy of the file in the File Cabinet, and sends you an email with a link to it's location. The file size limit is 5 MB, and the File Cabinet storage limit is 10 GB.
     

For more information about the localized EU sales list reports, see the country-specific tax topics.

### Related Topics:

-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [EU Sales List (ESL) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068052.html)
-   [EU Sales List Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068226.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

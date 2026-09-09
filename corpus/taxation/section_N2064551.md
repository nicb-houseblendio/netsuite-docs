---
id: "section_N2064551"
type: "section"
title: "Generating VAT/GST Reports"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > VAT/GST Reports > Generating VAT/GST Reports"
parent: "section_N2063644"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html"
anchors: ["procedure_N2064610"]
sha256: "93ed93334035878fc954e7993273163637969414305e3b0acc26bc0b8a0eaed0"
---

Note:

VAT/GST reporting requires the International Tax Reports SuiteApp.

NetSuite supports VAT/GST reporting for various countries in Europe, Asia, and Latin America. For some countries, NetSuite also provides reports in XML or CSV format required by tax agencies for electronic filing. For a list of country-specific VAT forms available, see [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html). For information about using NetSuite generated reports for electronic filing, see [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html).

Important:

The NetSuite VAT/GST tax form is made to look like the official tax form for convenience, but it's not intended to be printed and submitted to the tax agency. For some countries, NetSuite lets you to export the VAT return in a format that you can upload to the tax agency portal for electronic filing (XML, CSV, or DAT file). Make sure you review all the values before you submit the report.

#### To generate an international VAT/GST report: {#procedure_N2064610}

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  On the Tax Reports page, select values for the following fields:
    
    1.  **Subsidiary** - Select a subsidiary. The dropdown list only shows subsidiaries your role can access.
        
        To generate a consolidated report that includes child subsidiaries, check the **Group** box. You can use consolidated reporting if your company and its child subsidiaries belong to one VAT group, or is registered as a single tax entity for VAT purposes.
        
        Note:
        
        Nondeductible transactions aren't supported in consolidated reports.
        
    2.  **Country Form** - Select the VAT report that you want to generate.
        
    3.  **Tax Period** - Select the tax reporting period to use for the report.
        
    4.  **Accounting Book** - Select which accounting book will be used to generate the report. This field only shows if Multi-Book Accounting is enabled.
        
        Whenever you change the accounting book or reporting period, click **Refresh** to reload the report.
        
        The dropdown list shows all active books associated with the selected subsidiary. For more information, see [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html).
        
        Note:
        
        Adjusting tax amounts and group reporting aren't currently supported for secondary accounting books.
        
        For some countries, supplementary VAT reports are available. Click the **Supplementary** button on the Tax Reports page to generate supplementary reports.
        
3.  If you want NetSuite to generate an XML file of your VAT return for electronic filing, you must set up your electronic tax filing details before you generate the XML file. For more information, see [Setting Up Tax Filing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2053829.html).
    
    Note:
    
    The Tax Filing Setup page is only available for certain countries right now.
    
4.  To change the date and number format on the report, click **Setup**, and then click **Formatting**. For more information, see [Formatting Dates and Numbers for VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065022.html).
    
5.  Review the report carefully. Some boxes may not be filled in automatically, so you'll need to enter data manually. For system-generated data, you can click the figures in the boxes to view detailed transaction information. To view detailed reports, see [Viewing VAT Report Transaction Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065235.html).
    
    Example:
    
6.  To change the tax amounts on the VAT report, click **Adjust Return**. For more information, see [Making Adjustments on a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067438.html).
    
7.  Click **Print** to save the VAT report as a PDF. NetSuite saves the file in the VAT Folder of the File Cabinet. Saving and printing a PDF makes sure you have a record of manually entered values, because for some VAT reports, there may be boxes that NetSuite can't automatically generate values for. Use Adobe Acrobat Reader for viewing the PDF.
    
8.  Click the **Export to XML** or **Export to CSV** button to export the VAT report in a format you can submit to your tax agency.
    
    For some countries, NetSuite can generate files you can submit to the tax agency for electronic tax filing. When you generate an XML, CSV, or DAT file for electronic filing, you can flag the tax period in the report to exclude them from subsequent VAT returns. For more information, see [Flagging Tax Periods in a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721526384.html).
    
    The **System Notes** tab on the VAT form stores a copy of each exported file and a PDF of the final or submitted VAT form. For more information, see [Viewing the VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721544005.html).
    

### Related Topics:

-   [Formatting Dates and Numbers for VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065022.html)
-   [Viewing VAT Report Transaction Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065235.html)
-   [Making Adjustments on a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067438.html)
-   [Flagging Tax Periods in a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721526384.html)
-   [Viewing the VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721544005.html)
-   [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html)
-   [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [Setting Up Tax Filing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2053829.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

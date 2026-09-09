---
id: "section_N2022385"
type: "section"
title: "Türkiye VAT Report"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Türkiye Tax Topics > Türkiye VAT Report"
parent: "chapter_N2021231"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2022385.html"
anchors: ["bridgehead_N2022488", "procedure_N2022498", "bridgehead_N2022550", "procedure_N2022559", "bridgehead_N2022613", "procedure_N2022623"]
sha256: "bd2fbb01c31652059db428ed60eed1eec799aac50eabe04861242cb3a059d635"
---

If you have a Türkiye subsidiary and nexus and you have the International Tax Reports SuiteApp installed in your account, you can generate the VAT1015A Return 1 and the Customs Declaration for Exports. To generate the report, go to Reports > VAT/GST > Tax Reports (International).

Important:

To generate the tax report for Türkiye correctly, use the tax code properties provided by the International Tax Reports SuiteApp. See [Türkiye Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2021408.html).

NetSuite gets the values in the report from your transactions, but you may need to enter some data manually. It's important that you save a PDF file of the report for your own records because NetSuite can't audit manually entered data. For more information, see [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html).

You should review all the values in the report. You can click the values in the boxes of the VAT report to view drill down details.

Important:

The NetSuite VAT/GST tax form is made to look like the official tax form for convenience. It's not intended to be printed and submitted to the tax agency.

Note:

You can also customize saved reports from the International Tax Reports SuiteApp to view both detail and summary reports for purchases or sales, grouped by tax code. For more information, see [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html).

## Displaying the Customs Registration Number Field on Transaction Forms {#bridgehead_N2022488}

Important:

You must enter a value in the Customs Registration Number field for every sales transaction related to exports. NetSuite extracts and adds this information to the Customs Declaration for Exports. This field becomes available if you install International Tax Reports, but it's hidden by default.

#### To display the Customs Registration Number field on transaction forms: {#procedure_N2022498}

1.  Go to Setup > Customization > Transaction Body Fields
    
2.  On the list of **Transaction Column Fields**, click the **Customs Registration Number** link.
    
3.  Click the **Display** subtab.
    
4.  Set **Display Type** to **Normal**.
    
5.  Click **Save**. The **Customs Registration Number** field is now displayed on sales orders, invoices, and cash sales when you create a transaction for your Türkiye company (or Türkiye subsidiary for OneWorld accounts).
    

## Generating the Türkiye VAT Report {#bridgehead_N2022550}

#### To generate the VAT1015A Return 1: {#procedure_N2022559}

1.  Go to Reports > VAT > Tax Reports (International).
    
2.  On the Tax Return Reports page, select **Türkiye** from the **Country Form** dropdown.
    
3.  Select a parent company or subsidiary.
    
4.  Select a tax period.
    
5.  Click **Refresh** to display the report. For more information, see [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html).
    

## Generating the Customs Declaration for Exports {#bridgehead_N2022613}

#### To generate the Customs Declaration for Exports: {#procedure_N2022623}

1.  Generate a VAT1015A Return 1. (See [Generating the Türkiye VAT Report](#bridgehead_N2022550).)
    
2.  Click **Customs Declaration**. The system generates the **Customs Declaration for Exports** as a PDF file.
    

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Türkiye Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2021408.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

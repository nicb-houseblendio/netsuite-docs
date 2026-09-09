---
id: "section_N2065235"
type: "section"
title: "Viewing VAT Report Transaction Details"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > VAT/GST Reports > Generating VAT/GST Reports > Viewing VAT Report Transaction Details"
parent: "section_N2064551"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065235.html"
anchors: ["bridgehead_4297581247", "bridgehead_4297581443", "procedure_N2067154", "bridgehead_4297582044", "procedure_N2067234", "bridgehead_4297582355", "procedure_N2067292"]
sha256: "e09611dd51da391af66174e8357eaaca40e7e1f0ae4239d510b60a56e02065df"
---

On a VAT report, if you click a system-generated value in a box or field, you'll see a Detailed Report that shows all the transactions that make up that value. For example, system-generated values show up as underlined numbers in a box or field. You can click the number to see a detailed report of the associated box.

Each row of the report shows the following information:

-   Tax code
    
-   Date (transaction date)
    
-   Entity name
    
-   Transaction number - If there's no transaction number entered on the transaction record, you'll see an asterisk (\*) in the detailed report.
    
-   Transaction type
    
-   Net amount
    
-   Tax amount
    
    Note:
    
    For Belgium and the UK, the tax amount total is rounded to two decimal places.
    
-   Notional amount
    
    Note:
    
    For Belgium and the UK, the notional amount total is rounded to two decimal places.
    
-   Gross amount
    
-   Total amounts (grand total, column total, and page total)
    

Note:

The number of lines shown per page depends on the value saved in the **Number of Rows in List Segments** field in the General page. To view this field, go to Home > Set Preferences > General. If you have a lot of transactions, you may need to wait a few minutes for the report to load. You'll see a progress bar when it's loading.

The Detailed Report can only show 100,000 lines per saved report. If you go over that, the total amount in the Detailed Report may not match the system-generated value in the box. For more information about row limitations and suggested workaround, see [Row Limitations for Report Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719691.html).

When viewing the Detailed Report, you can do the following:

-   Click the entity name to open the entity record
    
-   Click the transaction number to open the transaction record
    
    Note:
    
    If there's no transaction number entered on the transaction record, you'll see an asterisk (\*) in the detailed report. You can click the asterisk to view the transaction record.
    
-   Sort all rows by column, in ascending or descending order
    
-   Select a page to view using the paging toolbar
    
-   Resize columns as needed
    
-   Move columns around (for example, you can move the date column before the tax code column)
    
-   Export the report to Microsoft Excel format
    
    Note:
    
    The exported file uses the default column order and sort, even if you changed them in the UI. Also, Excel follows your computer's regional settings, not your browser, so that's how numbers, dates, and currencies will show up.
    

## To view the entity record: {#bridgehead_4297581247}

Click the customer or vendor name in the **Name** column.

## To view the transaction record: {#bridgehead_4297581443}

Click the transaction number in the **Number** column. If there's no transaction number entered on the transaction record, you'll see an asterisk (\*) on the detailed report. You can click the asterisk to view the transaction record.

#### To sort rows by column: {#procedure_N2067154}

1.  Place your mouse pointer on a column header to reveal a dropdown arrow.
    
2.  Click the arrow.
    
3.  Select **Sort Ascending** or **Sort Descending**.
    

## To select a page to view: {#bridgehead_4297582044}

In the paging toolbar at the bottom of the page, click the arrows to find the page you want, or type the page number and press **Enter**.

#### To resize a column: {#procedure_N2067234}

1.  Place your mouse pointer on the right border of a column header. The pointer becomes a double-sided arrow that looks like a cross.
    
2.  Click and drag the double-sided arrow to the right or to the left, and then release the mouse when the column is as wide or as narrow as you want it to be.
    

## To move a column: {#bridgehead_4297582355}

Click and drag the column header to where you want it, then drop it.

For example, if you want to make the **Date** column the first column on the table, click and hold it's header, drag it to the left border of the **Tax Code** column, and let go.

#### To export to Excel: {#procedure_N2067292}

1.  At the bottom right corner of the Detailed Report page, click the arrow on the **Export** button, and then click **Export Microsoft Excel**. The system exports the entire report.
    
2.  On the export popup window, you can choose to save the file or open it.
    
    Note:
    
    Choose **Save File** if the report has a large amount of data.
    
    -   If you choose **Save File**, make sure the saved file has the .xls extension, and then open it using Microsoft Excel.
        
    -   If you choose **Open with**, don't open it from the browser. Instead, select Microsoft Excel to open the file. When the file is opened, save it using **Save As** and pick the .xls file extension.
        

### Related Topics:

-   [Formatting Dates and Numbers for VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065022.html)
-   [Making Adjustments on a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067438.html)
-   [Flagging Tax Periods in a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721526384.html)
-   [Viewing the VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721544005.html)
-   [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [Setting Up Tax Filing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2053829.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

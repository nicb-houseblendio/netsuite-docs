---
id: "section_N2019313"
type: "section"
title: "Thailand VAT Reports"
branch: "thailand-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Thailand Help Topics > Thailand Tax Topics > Thailand VAT Reports"
parent: "chapter_N2018510"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2019313.html"
anchors: ["bridgehead_N2019415", "bridgehead_N2019592", "bridgehead_N2019609", "bridgehead_N2019622", "bridgehead_N2019677", "bridgehead_N2019824", "procedure_N2019833"]
sha256: "de365c5d3dec4a4d37719d57314f46ba319c2e7de36a43c1590ecc4c5d18f6f1"
---

If you have a Thailand subsidiary and nexus and you have the International Tax Reports SuiteApp installed in your NetSuite account, you can generate the following reports:

-   Value Added Tax Return under the Revenue Code for Internet Filing (Form P.P.30),
    
-   Output Tax Report
    
-   Input Tax Report
    

Important:

To generate the VAT report for Thailand, use the tax code properties provided by the International Tax Reports SuiteApp. See [Thailand Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2018677.html).

The VAT forms areavailable in English and Thai, from Reports > VAT/GST > Tax Reports (International). NetSuite gets the values in the report from your transactions, but some boxes in the forms may require you to enter data manually. It's important that you save a PDF file of the report for your own records because NetSuite cannot audit manually entered data. For information, see [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html).

You should review all the values in the report. You can click the values in the boxes of the VAT report to view drilldown details. To understand how NetSuite uses the tax codes to get the values for the Thailand VAT Return, see [What goes into each box - Thailand VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2020046.html).

Important:

The NetSuite VAT/GST tax form is designed to look like the official tax form for ease of use when completing the official return form. It's not intended for submission to the tax agency.

## VAT Reporting by Location {#bridgehead_N2019415}

Note:

The Location filter on the Thailand VAT report is not available to the Tax Reporting roles and the Accountant (Reviewer) role. To access to this feature, the Administrator must give you the Locations permission with Edit access level.

## Locations {#bridgehead_N2019592}

If you're using the Locations feature in NetSuite, you can generate the Thailand VAT Return Form P.P.30 for each location. You would use this VAT reporting by location feature if you're using Location records in NetSuite to represent VAT reporting entities.

A Location record must be assigned to the subsidiary that has a Thailand nexus so that you can select it in the Location field of the VAT form. When a location is selected, the VAT form loads the branch code and address of the location.

## Multi-Location Inventory {#bridgehead_N2019609}

If your NetSuite account has the Multi-Location Inventory feature enabled, your warehouses must be set up as children of a VAT-reporting branch (the parent location). The VAT-reporting branch is what you should select in the Location field of the VAT form.

## Branch No. {#bridgehead_N2019622}

![A Thailand VAT Form showing the Branch No.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/ThailandVATFormBranchNo.png)

-   In accounts **with the Locations feature enabled** (either NetSuite or NetSuite OneWorld), NetSuite gets the Branch No. value for the VAT report from the Branch ID field of the Location record.
    
-   In accounts **without the Locations feature**, NetSuite retrieves the branch number from the VAT Registration No. or VAT ID field. The first 13 characters comprise the VAT ID, and if there are numbers after the 13th character, those make up the branch code. For example, if the value in the VAT ID field is 123456789012398765, it means that 1-2345-67890-12-3 make up the VAT ID, and 98765 make up the branch code. In OneWorld accounts, the VAT Registration No. field can be found in the Company Information page and/or Subsidiary record. If you don't have a OneWorld account, the VAT Registration No. field can be found only in the Company Information page.
    

## Thailand VAT Return Form P.P.30 {#bridgehead_N2019677}

**To generate a Thailand VAT Return Form P.P.30:**

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  If you're using a OneWorld account, select the **Thailand** subsidiary (or a subsidiary that has a Thailand nexus).
    
3.  Select the **Thailand** country form (Thai or English version).
    
4.  If you're generating a report for a location, select a location. Otherwise, leave the **Location** field empty.
    
5.  Select a tax period for the report.
    
6.  Click **Refresh** to generate the report.
    
    Important:
    
    Each time you change a subsidiary, location, country form, or tax period, click **Refresh**.
    
7.  Carefully review the report. You can click the values in the boxes to view drilldown details. NetSuite gets the values in the reports from your transactions, but some boxes in the form may require you to manually enter data.
    
    Note:
    
    To understand how NetSuite uses the tax codes to get the values for the Value Added Tax Return for Thailand, see [What goes into each box - Thailand VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2020046.html).
    
8.  Click **Print** to save a PDF file of the report.
    
    ![Thailand VAT Return Form P.P.30](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/ThailandVATReportbyLocation.png)

Note:

You can also use customizable saved reports provided by the International Tax Reports SuiteApp to view both detail and summary reports for purchases or sales, grouped by tax code. For more information, see [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html).

## Supplemental VAT Reports for Thailand {#bridgehead_N2019824}

#### To generate the Input or Output Tax Reports: {#procedure_N2019833}

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  If you're using a OneWorld account, select the **Thailand** subsidiary (or a subsidiary that has a Thailand nexus).
    
3.  Select the **Thailand** country form (Thai or English version).
    
4.  If you're generating a report for a location, select a location. Otherwise, leave the **Location** field empty.
    
5.  Select a tax period.
    
6.  To generate the **Output Tax Report**:
    
    1.  Click **Output**.
        
    2.  Click **Excel** or **PDF** to download the file.
        
7.  To generate the **Input Tax Report**:
    
    1.  Click **Input**.
        
    2.  Click **Excel** or **PDF** to download the file.
        

Important:

Each time you change a subsidiary, location, country form, or tax period, click **Refresh**.

### Related Topics

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)
-   [Thailand Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2018677.html)
-   [What goes into each box - Thailand VAT report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2020046.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

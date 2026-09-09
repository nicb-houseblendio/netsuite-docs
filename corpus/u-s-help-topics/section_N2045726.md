---
id: "section_N2045726"
type: "section"
title: "Form 1099-MISC - Miscellaneous Income Statement"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > U.S. Tax Reports > Form 1099-MISC - Miscellaneous Income Statement"
parent: "section_N2042330"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2045726.html"
anchors: ["subsect_1504274714", "procedure_1534189601", "procedure_0831092701"]
sha256: "97925d514a698ebf0589b523aea96e9c3379dc0ed0633aa94f30a06eadef5488"
---

Important:

NetSuite does not support 1099-MISC forms. Instead, NetSuite provides customized saved searches to help you report 1099-MISC vendor payments to other providers, such as Sovos or Avalara.

## Reporting 1099-MISC Vendor Payments to a Third-Party Provider {#subsect_1504274714}

NetSuite provides customized saved searches to help you export 1099-MISC vendor payments to a third-party provider, such as Sovos or Avalara. You can edit the saved search for your particular needs. For example, if you want to include payments made by checks in the saved search, you might need to replace the Date Closed field with the Date field.

[View the Exporting 1099-MISC Information video](https://videohub.oracle.com/media/1_c6asa9j8).

Important:

You are responsible for the information that you report to the Internal Revenue Service (IRS). The saved search provided by NetSuite might not include all of the information that you need to report. Review the output of the saved search for accuracy before you export the data to a provider.

#### To set up a vendor as 1099 eligible: {#procedure_1534189601}

1.  Go to _Lists > Relationships > Vendors_.
    
2.  Click **Edit** next to the vendor whose record you want to make eligible.
    
    NetSuite reports the total you paid to these vendors. The total includes payments made by paying existing bills or by writing checks.
    
3.  On the vendor record, click the **Financial** subtab.
    
4.  Under Tax Information, check the **1099 Eligible** box.
    
5.  Click **Save**.
    

Note:

For information about associating 1099-MISC categories with expense accounts, see [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html).

#### To use the 1099 saved searches to report vendor payments: {#procedure_0831092701}

1.  Go to _Customization > SuiteBundler > Search & Install Bundles_
    
2.  In the **Keywords** field, enter **1099 Vendor Payment Report**.
    
3.  Click the name of the bundle for your third-party provider, and then click **Install**.
    
4.  Click **Install Bundle**.
    
5.  After the saved search is installed, go to Reports > Saved Searches > 1099 Vendor Payment Report - _Vendor Name_ > Edit.
    
6.  Edit the search according to your needs.
    
7.  Export the search to a CSV or Excel file.
    

Note:

The report includes all vendor payments. You might need to filter out vendors who don't meet the minimum payments thresholds set by the Internal Revenue Service. More detailed information about 1099-MISC reporting requirements can be found at [www.irs.gov/uac/about-form-1099misc](https://www.irs.gov/forms-pubs/about-form-1099misc).

### Related Topics:

-   [Sales Tax Liability by Tax Item Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042683.html)
-   [Sales Tax Liability by Tax Agency Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2043102.html)
-   [Sales Tax on Sales Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2044611.html)
-   [Sales Tax on Sales Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2044970.html)
-   [Sales Tax Analysis Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2045340.html)
-   [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html)
-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

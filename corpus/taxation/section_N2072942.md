---
id: "section_N2072942"
type: "section"
title: "International Tax Reports Best Practices"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > International Tax Reports Best Practices"
parent: "chapter_N2050955"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html"
anchors: ["bridgehead_N2073004"]
sha256: "7fd2ec7a019a5e18f304c32c357e35150df0dac74616d50fa47301b00574ab3d"
---

Important:

International Tax Reports SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

Follow these guidelines when you use the International Tax Reports (ITR) SuiteApp:

-   Make sure your tax code set up is correct. You can rename tax codes, but you must make sure the properties on each are set correctly.
    
-   Close tax periods before generating tax reports for filing.
    
-   Click **Refresh** every time you change a subsidiary or tax period when generating a report.
    
-   Click **Print** to save PDF files of your reports in the NetSuite File Cabinet.
    
-   Don't rename the saved reports provided by International Tax Reports SuiteApp to avoid having issues with report generation.
    
-   To generate a report successfully, make sure you don't have more than 100,000 transaction lines per period. If you need to generate reports with a large volume of transaction lines, you must split it into batches and generate it for shorter periods.
    
-   After you install the ITR SuiteApp, make sure the ITR scripts are at the top of the list to avoid conflicts with other scripts.
    
    #### To reorder your scripts:
    
    1.  Go to Customization > Scripting > Scripted Records (Administrator).
        
    2.  Click the **Record** column heading to sort the list by record.
        
    3.  Click **Edit** next to the **Vendor Bill** record, and then do both of the following:
        
        -   On the **User Event Scripts** subtab, drag the Tax Transaction Fields UE script to the top of the list.
            
        -   On the **Client Scripts** subtab, drag the Tax Transaction Fields CS script to the top of the list.
            
    4.  Click **Save**.
        
    

## For EU users {#bridgehead_N2073004}

-   Ensure that your customer and vendor records have VAT numbers. Each EU country has its own VAT number format, so be sure to use the correct VAT number formats. For more information, see the Additional Setup Steps under [Installing and Setting Up International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051712.html).
    
-   Verify that the customer and vendor VAT registration IDs are valid on the current date by clicking the VIES link on the Financial subtab of the customer or vendor record. Regularly check your EU customer's VAT registration ID to ensure that the details are still valid and hasn't been deregistered. This helps you avoid errors in your EU Sales List and Intrastat reports.
    
    Each EU country has its own VAT prefix and numbering format. For more information, refer the this [VAT identification number structure](http://ec.europa.eu/taxation_customs/vies/faqvies.do) published by the European Commission.
    
-   Make sure that each customer record has a shipping address. If there's no shipping address, NetSuite will use the billing address saved on the customer record. If the invoice is charged to a project, NetSuite will use the address saved on the customer record that the project is associated with.
    

### Additional Information:

-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [EU Sales List (ESL) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068052.html)
-   [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html)

### Related Topics:

-   [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [Setting Up Tax Filing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2053829.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

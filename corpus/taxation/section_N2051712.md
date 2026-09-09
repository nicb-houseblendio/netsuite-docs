---
id: "section_N2051712"
type: "section"
title: "Installing and Setting Up International Tax Reports"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > International Tax Reports > Installing and Setting Up International Tax Reports"
parent: "section_N2051341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051712.html"
anchors: ["bridgehead_4102301062", "procedure_N2051788", "bridgehead_N2053004"]
sha256: "6b15413c00b5e38e9f6f63a18a66e1ca76f1d478055f2c3d753bf44bdcae5def"
---

Important:

International Tax Reports SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

If you're an account administrator, you can install the International Tax Reports SuiteApp in your account.

-   The International Tax Reports SuiteApp (previously named Tax Reporting and Filing Bundle 8375) has been changed to a managed bundle, effective June 1, 2011. This means that updates will be installed automatically, with a list of fixes and changes documented in the accompanying release notes.
    
-   If you already had the bundle before it became managed, you'll need to go to Customization > SuiteBundler > Search & Install Bundles > List, find the bundle and click **Update** to get automatic updates. You'll see a message informing you that it's now a managed bundle. It will then ask you to let NetSuite install future updates to your account. Click **OK** to agree.
    
-   The International Tax Reports SuiteApp requires the tax reporting periods feature. You can only use this SuiteApp in OneWorld, International, UK, Australia, and Japan editions. For more information, see [NetSuite Editions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N270055.html).
    

## Prerequisites {#bridgehead_4102301062}

Make sure you do the following prerequisites before you install the International Tax Reports SuiteApp:

-   Set up your tax reporting periods. For more information, see [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html) and [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html).
    
-   Enable the following SuiteCloud features. Go to Setup > Company > Enable Features and check the box for the following features on the SuiteCloud tab:
    
    -   Custom Records
        
    -   Client SuiteScript
        
    -   Server SuiteScript
        

#### To install the International Tax Reports SuiteApp: {#procedure_N2051788}

1.  Go to Customization > SuiteBundler > Search & Install Bundles.
    
2.  On the Search & Install Bundles page, click **Advanced**.
    
3.  Enter the following:
    
    -   Keywords = International Tax Reports
        
    -   Location = Production Account
        
    -   Account ID = 3776651
        
4.  Click **Search**.
    
5.  Click the link for **International Tax Reports** (Bundle ID: 43003).
    
6.  On the SuiteApp Details page for International Tax Reports, click **Install**.
    

Warning:

If you remove the bundle, you'll lose the histories of your UK VAT 100 and EC Sales online submissions. Any custom fields on item and transaction records such as following are also deleted:

-   Commodity Code
    
-   Delivery Terms
    
-   Nature of Transaction Codes
    
-   Customs Registration Number fields used for Intrastat Reports and Türkiye Customs Declaration for Exports
    

You'll also lose all custom tax code properties on your tax code records.

## Additional Setup {#bridgehead_N2053004}

After installing the International Tax Reports SuiteApp, perform the following setup steps:

1.  **Roles and Permissions**
    
    Use the following roles provided by the International Tax Reports SuiteApp. They're already set up with all the required permissions and script access you need:
    
    -   Tax Reporting Accountant
        
    -   Tax Reporting Accountant Reviewer
        
    -   Tax Reporting CFO
        
    -   Tax Reporting Bookkeeper
        
    
    If you want to use your own customized roles, read [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html).
    
    Note:
    
    The standard Bookkeeper role can't access the reports in the International Tax Reports SuiteApp, even if you add permissions and grant the role access to scripts and reports. You should use the preconfigured Tax Reporting Bookkeeper role instead.
    
2.  **Report By Period**
    
    Make sure the Report By Period field in Home > Set Preferences > Analytics subtab is set to either **Financials Only** or **All Reports**. Report By Period should not be set to **Never**. This preference determines whether report data is calculated by date range or by period. See [Reporting Preferences on the Set Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N716534.html).
    
3.  **Manage Tax Reporting**
    
    For EU nexuses, set up nature of transaction codes for Intrastat reporting. See [Nature of Transaction Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070738.html).
    
4.  **For Türkiye only: Customs Registration Number**
    
    Display the Customs Registration Number field on your transaction forms. This field is hidden by default when you install the SuiteApp, but you'll need it for the Customs Declaration for Exports. The customs registration number is required for the Customs Declaration for Exports. To display the field on your forms, follow the steps in [Displaying the Customs Registration Number Field on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2022385.html#bridgehead_N2022488).
    
5.  **For Thailand only: Location filter**
    
    The Location filter on the Thailand VAT report isn't available to the Tax Reporting roles and the Accountant (Reviewer) role. To use the VAT reporting by location feature for Thailand, the Administrator must give those roles the Locations permission with Edit access.
    
6.  **Commodity Code**
    
    Make sure you add commodity codes to item records used in EU transactions. The commodity code is used for Intrastat reporting. The Commodity Code field is found on the EU Intrastat Reporting subtab of the Item record. For an example, and for information about Item types that use commodity codes, see [Commodity Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070438.html).
    
7.  **VAT Registration Number**
    
    Make sure you add valid VAT registration numbers to your customer records and vendor records. **The Tax Reg. Number** or **VAT Registration No.** field is on the Financial subtab of the Customer record and Vendor record. For EU customers and vendors, the system validates the VAT number you enter in the field. In addition, a VIES Validation link is provided. You can also click this link to validate the number.
    
    Each EU country has its own VAT prefix and numbering format. For information, refer to the [VAT identification number structure](https://euipo.europa.eu/tunnel-web/secure/webdav/guest/document_library/Documents/COSME/VAT%20numbers%20EU.pdf) published by the European Commission.
    
8.  **Formats of dates and numbers**
    
    For each nexus associated with your subsidiaries, define how dates and numbers are displayed on VAT reports. The formats that you set up are applied to the VAT form, PDF, and drilldown reports. For more information, see [Formatting Dates and Numbers for VAT Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065022.html).
    
9.  **Scripted Records**
    
    Move the International Tax Reports Scripts to the top of the list to avoid conflicts with other scripts. For more information, see [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html).
    

### Related Topics:

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html)
-   [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html)
-   [EU Sales List (ESL) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068052.html)
-   [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

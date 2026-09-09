---
id: "section_N2054151"
type: "section"
title: "Creating or Customizing Roles to Use the International Tax Reports"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports"
parent: "chapter_N2050955"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html"
anchors: ["bridgehead_N2054496", "bridgehead_N2054555"]
sha256: "8c7fa6e004f901df256e4f021036d88c25e6f439608792fdd460f3d98742e5b5"
---

Important:

International Tax Reports SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

The International Tax Reporting features are accessible to the following standard NetSuite roles: Administrator, Accountant, Accountant Reviewer, and Chief Financial Officer. The SuiteApp also gives you roles that already have all the permissions you need, so you can use them as templates for custom roles:

-   Tax Reporting Accountant
    
-   Tax Reporting Accountant Reviewer
    
-   Tax Reporting CFO
    
-   Tax Reporting Bookkeeper
    

If you're an Administrator, you can create a new role, or customize a standard or tax reporting role, then give these new roles access to the international tax reporting features. But before you do that, take note of the following:

-   If you customize any standard NetSuite role, you'll need to add permissions and access to scripts and other components to the new custom role so it can use the international tax reporting features.
    
-   The standard Bookkeeper role can't access the reports in the International Tax Reports SuiteApp even if you add permissions and grant the role access to scripts and reports. Use the Tax Reporting Bookkeeper role provided by the SuiteApp instead.
    
-   If you create a new role, you'll need to add permissions to use other NetSuite features, not only those required for the International Tax Reports SuiteApp.
    
-   If you've previously created a script that has parameters, make sure the new role has access to both the script deployments and the script deployment parameters.
    

Important:

Copying a tax reporting role and saving it as a new role doesn't copy the script deployments and custom fields used for tax reporting. If you want to use your own custom roles for international tax reporting, you should customize the roles already included in the SuiteApp:

-   Tax Reporting Accountant
    
-   Tax Reporting Accountant Reviewer
    
-   Tax Reporting CFO,
    
-   Tax Reporting Bookkeeper
    

Make sure your custom roles have access to script deployments and any custom fields.

To enable your custom roles to use the features provided by the International Tax Reports SuiteApp, complete the steps in the following topics:

## For all countries {#bridgehead_N2054496}

-   [International Tax Reports Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054820.html)
    
-   [Granting Access to VAT/GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html)
    
-   [Granting Access to Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060594.html)
    

## For European Union member states {#bridgehead_N2054555}

-   [International Tax Reports Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054820.html)
    
-   [Granting Access to VAT/GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html)
    
-   [Granting Access to Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060594.html)
    
-   [Granting Access to the Manage Tax Reporting Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061085.html)
    
-   [Granting Access to Intrastat Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061400.html)
    
-   [Granting Access to EU Sales Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061855.html)
    

Important:

Before granting access to Intrastat Reports and EU Sales Lists, you must first grant access to scripts for VAT/GST Reporting. See [Granting Access to VAT/GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html).

### Related Topics

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Defining Script Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999041.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Installing and Setting Up International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051712.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

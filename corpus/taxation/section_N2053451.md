---
id: "section_N2053451"
type: "section"
title: "Automatic Tax Code Provisioning"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Automatic Tax Code Provisioning"
parent: "chapter_N2050955"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html"
anchors: []
sha256: "4cfbd87adb9df3170d6f5ded5df16300e368b1f357c5fbde95e4e094c0a86c67"
---

Important:

International Tax Reports SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, don't install this SuiteApp.

To use automatic tax code provisioning, make sure you install the International Tax Reports SuiteApp in your account before you create subsidiaries. In OneWorld accounts with the International Tax Reports SuiteApp, when you add a new subsidiary country, the system creates the nexus and the VAT/GST tax codes at the same time. This is why you need to have the International Tax Reports SuiteApp installed before you add subsidiaries. If you create a subsidiary country before you have installed the SuiteApp, NetSuite adds its nexus but only provides a few default tax codes.

**Important things to note:**

-   For some tax codes created by the International Tax Reports SuiteApp, you'll need to set the correct value in the **Available on** field of the Tax Code page. This preference isn't set automatically by the automatic tax code provisioning feature. See [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html) for instructions on how to do this, and read the country-specific tax topics to see the tax code tables for each country. Consult your tax agency to make sure your tax code rates are correct.
    
-   Without the International Tax Reports SuiteApp, NetSuite makes default tax codes available when you add a nexus to your account. In some NetSuite implementations, the nexus may have already been added before the SuiteApp was installed. When you first set up your NetSuite account, the home nexus is created automatically. You should review the tax codes and edit or add new ones if needed. Use the country-specific tax code tables in the Help Center to set the correct properties. Note that the SuiteApp only creates VAT/GST tax codes for supported countries, because those tax codes are used for tax reports. For a list of supported countries, see [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html).
    
-   Tax codes for nondeductible tax aren't included in the automatic tax code provisioning, so you'll need to create them manually. For more information, see [Recording Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822590.html).
    
-   When you add a nexus for Colombia or Singapore, the SuiteApp creates the tax codes, but you'll need to manually create additional tax control accounts and tax types, and then edit the relevant tax code to set the correct tax type. For details, see [Colombia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1867954.html) and [Singapore Tax Topics for Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1981261.html).
    
-   Tax codes for Mexico are also created when you add a Mexico nexus. These are used to generate the DIOT file. For more information, see [Mexico Tax Topics (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1940317.html) and [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html).
    

You can also create other tax codes, but they won't show up in the VAT/GST reports unless they follow the properties defined in the tax code matrix. Make sure you use the correct properties for those tax codes to be picked up by the VAT/GST reports. Refer to the country-specific topics to see each country's tax code settings.

You can use any tax code name you prefer, provided you've set the correct properties for them to be picked up by the VAT/GST reports. Tax reports identify transactions by looking at the tax code properties, not the tax code names. For information about current tax rates, be sure to consult your tax agency.

Some country-specific tax topics have tables that show what goes into each box of the VAT/GST reports.

Read the following topics for more information about tax code provisioning:

-   [Automatic Tax Code Provisioning Workaround](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1548655148.html) - Procedure for activating the automatic tax code provisioning feature if you installed the International Tax Reports SuiteApp after the subsidiary and nexus were created.
    
-   [EU One Stop Shop Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4174874694.html) - Automatic tax code provisioning of OSS tax codes for OneWorld accounts with EU nexuses.
    
-   [OSS Tax Code Provisioning for Regular NetSuite Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4204428442.html) - Procedure for provisioning OSS tax codes to non-OneWorld accounts.
    

### Related Topics:

-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
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

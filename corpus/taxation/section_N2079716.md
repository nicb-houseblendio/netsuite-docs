---
id: "section_N2079716"
type: "section"
title: "Setting Up Withholding Tax"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Up Withholding Tax"
parent: "chapter_N2078886"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html"
anchors: ["bridgehead_N2079748", "bridgehead_N2079965", "bridgehead_N2080032"]
sha256: "83eae4a901f54a3d2616d33f0e58a9d3656a9e8a992b36680d9d952aca16c11f"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

To use the withholding tax features in NetSuite, you must install the Withholding Tax SuiteApp.

Note:

US and Canada nexuses aren't supported.

## Prerequisites {#bridgehead_N2079748}

**Before installing the Withholding Tax SuiteApp:**

1.  Make sure that the following features are enabled in your account before installing the Withholding Tax SuiteApp:
    
    1.  Advanced Taxes
        
    2.  Custom Records
        
    3.  Server SuiteScript
        
    4.  Client SuiteScript
        
    
    To enable these features, go to Setup > Company > Enable Features. For Server SuiteScript and Client SuiteScript, you must agree to the SuiteCloud Terms of Service when you enable these features. For more information, see [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html).
    
2.  Make sure that Expand Account Lists is enabled in your account. To enable this preference, go to Setup > Accounting > Accounting Preferences. For more information, see [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).
    
3.  For new OneWorld accounts, install the International Tax Reports SuiteApp. This SuiteApp enables the automatic creation of tax codes when you add a new country nexus to your NetSuite account. For more information, see [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html). You can also create tax codes manually. You can refer to country-specific tax topics for guidance.
    
4.  For each nexus where you use withholding tax, make sure you have VAT/GST or sales tax codes set up as follows:
    
    -   Exclude from VAT reports
        
    -   Tax Rate: 0%
        
        You can use the UNDEF tax code provisioned by NetSuite.
        
5.  If you're using the Multi-Location Inventory feature, make sure the Location field is displayed on custom forms. This field is required when the Multi-Location Inventory feature is enabled. Hiding it can cause issues. For help on custom transaction forms, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).
    

## Installing the Withholding Tax SuiteApp {#bridgehead_N2079965}

The Withholding Tax SuiteApp is a managed bundle and updates automatically whenever there are improvements or new features added.

You can install the Withholding Tax SuiteApp in any NetSuite account, including OneWorld.

#### To install the Withholding Tax SuiteApp:

Important:

Move the International Tax Reports and Withholding Tax scripts at the top of your scripts lists to avoid conflicts with other scripts. For more information, see [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html).

1.  Go to Setup > Company > Enable features.
    
2.  Click the **Tax** subtab.
    
3.  Click **Withholding Tax**.
    
4.  On the SuiteApp Details page for Withholding Tax (Bundle ID: 47459), click **Install**.
    

For information about installing SuiteApps, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).

For information about the limitations of the Withholding Tax SuiteApp, see [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html).

## Withholding Tax Setup Steps {#bridgehead_N2080032}

After you install the Withholding Tax SuiteApp, set up withholding tax preferences, tax types, tax codes, and tax groups for each nexus that use withholding tax. You can also set default withholding tax codes on items, customers, and vendors. For more information, read the following topics:

1.  [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html)
    
2.  [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html)
    
3.  [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html)
    
4.  [Setting Up Withholding Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085135.html)
    
5.  [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
    

For information about roles and permissions for withholding tax features, see [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html).

When you install the Withholding Tax SuiteApp, withholding tax fields show up by default on all custom transaction forms. In the custom form definition, the **Show** box is already checked for the withholding tax fields.

Important:

The withholding tax fields display on the form only if withholding tax is enabled for the subsidiary. For new custom transaction forms, make sure the withholding tax fields are shown.

The following transaction column fields are used for withholding tax on transactions:

-   Withholding Tax Amount - Expense
    
-   Apply WH Tax?
    
-   Item's Default WT Code
    
-   Withholding Tax Base Amount - Expense
    
-   Withholding Tax Rate - Expense
    
-   Withholding Tax Code - Expense
    
-   Withholding Tax Line - Expense
    

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Up Withholding Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2083657.html)
-   [Setting Up Withholding Tax Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084141.html)
-   [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html)
-   [Setting Up Withholding Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085135.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "bridgehead_N2151888"
type: "bridgehead"
title: "General Subtab"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Creating Fixed Assets Management Records > Creating Asset Records Manually > General Subtab"
parent: "section_164689339824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2151888.html"
anchors: []
sha256: "a2378799963a34ff857b5c871de787d88d40abc7b4858360932ea1455b95a6e0"
---

On the General subtab, enter values for the following fields:

-   **Department** - Enter a department for this asset.
    
-   **Class** - Enter a class for this asset.
    
-   **Location** - Enter a location for this asset.
    
    Note:
    
    If location, department, or class are required fields for journal entries, you must set them on the asset record. For example, if you setup requires journal entries to be posted on department change, you must enter a department on the record. For more information, see [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html).
    
-   **Subsidiary** - If a you're using a OneWorld account, select the asset's subsidiary.
    
    For more information about transferring assets between subsidiaries, see [Asset Transfer Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862663749.html).
    
-   **Currency** - Shows the subsidiary's base currency.
    
-   **Custodian** - Select the employee responsible for the asset. The Assets subtab on the Employee record shows a list of assets that the employee is a custodian of.
    
-   **Physical Location** - Enter the location of the asset.
    
-   **Include In Reports** - Check this box to include the asset in the Asset Register and Asset Summary Report. By default, all assets are included in the report.
    
-   **Purchase Date** - Enter the date when the asset was purchased.
    
-   **Depreciation Start Date** - Enter the date depreciation starts. For example, an asset can be purchased but not received or placed into service until a few months later.
    
-   **Depreciation End Date** - Enter the date depreciation is expected to end. By default, the value is set to the asset's depreciation start date plus the useful lifetime.
    
    The system shows an error if the end date is before the start date. If you enter valid start and end dates, the system automatically calculates the Asset Lifetime. If you change the end date and it's valid, the system recalculates the Asset Lifetime. The system shows a message whenever it changes the depreciation end date.
    
    Note:
    
    The SuiteApp can't recalculate the Asset Lifetime if you change the **Depreciation End Date** through CSV import or script.
    
-   **Last Depreciation Period** - Set to zero by default.
    
-   **Last Depreciation Amount** - Set to zero by default.
    
-   **Last Depreciation Date** - Set to 1/1/1980 by default.
    
-   **Target Depreciation Date** - Enter the next depreciation date.
    
-   **Depreciation Active** - Select whether the asset is active and included in depreciation processing. For project assets, you can set depreciation to automatically start when the project ends.
    
    Note:
    
    The system automatically creates an Acquisition History Record when you set a depreciation start date for the asset. When **Depreciation Active** is set to **False**, no Acquisition History record is created. When **Depreciation Active** is set to **On Project Completion**, the Depreciation Start Date is automatically populated when the project ends.
    
-   **Depreciation Rules** - Select from the following values:
    
    -   **Acquisition** - The asset depeciates in the same period it's first activated.
        
    -   **Disposal** - The asset depreciates in its final period.
        
    -   **Pro-rata** - The asset depreciates in proportionally for partial months in the acquisition and disposal periods, using a standard 30-day month. For example, if depreciation starts on June 18, 2011 and ends on September 17, 2011, then 13 days worth of depreciation is recorded in the first depreciation period, and 17 days worth of depreciation is recorded in the final depreciation period.
        
        The following examples illustrate Pro-rata depreciation calculation when depreciation starts on the last day of the month:
        
        -   If depreciation starts on the last day of a 30-day or 31-day month (for example, April 30 or January 31), depreciation is recorded for 1 day in the acquisition period, and for 29 days in the disposal period.
            
        -   If depreciation starts on the last day of February, depreciation in the acquisition period is calculated for 1 day plus the number of days to complete 30 days. The asset depreciates for the corresponding partial month in the disposal period. For example, if depreciation starts on February 28, three days worth of depreciation (the 28th plus 2 days to make 30) is recorded for the first depreciation period, and 27 days worth of depreciation is recorded in the final depreciation period.
            
    -   **Mid-month** - If Depreciation Start Date is in the first half of the month, then depreciation starts on the same month of the asset acquisition. Otherwise, depreciation starts on the month after the asset acquisition month.
        
-   **Revision Rules** - Controls how revaluations affect the asset. The default value is set by Asset Type.
    
    -   **Current Period** - The system recalculates depreciation to date and posts the difference between the calculated depreciation and the previously posted depreciation in the current period.
        
    -   **Remaining Life** - The revision affects only future depreciation calculations.
        
-   **Manufacturer** - Enter the asset's manufacturer.
    
-   **Date of Manufacture** - If known, enter the asset's manufacture date.
    
-   **Supplier** - Enter the supplier (vendor) the asset was purchased from.
    
-   **Purchase Order** - Select the purchase order for the asset.
    
-   **Parent Transaction** - Select the transaction that generated or represents this asset's acquisition.
    

### Related Topics

-   [Creating Asset Records Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689339824.html)
-   [Asset Values Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1506382738.html)
-   [Compound Assets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4609649173.html)
-   [Accounts Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2152269.html)
-   [Lease Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2152301.html)
-   [Insurance Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2153588.html)
-   [Maintenance Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2153700.html)
-   [Components Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4522188043.html)
-   [Asset Sale/Disposal Tab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154456.html)
-   [Depreciation History Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154557.html)
-   [Asset Usage Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154643.html)
-   [Sub-Assets Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154774.html)
-   [Income/Expense Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154956.html)
-   [Notes Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154992.html)
-   [Files Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2155005.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

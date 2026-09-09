---
id: "section_N2140095"
type: "section"
title: "Depreciation Formula"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > Depreciation Methods > Depreciation Formula"
parent: "section_164862696596"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140095.html"
anchors: []
sha256: "0c8dcc6943c33a59e01b9bf090f5ba18226b87a617544ff22af24696253a1e74"
---

In the Fixed Assets Management SuiteApp, each depreciation method uses a formula to show how the monthly or annual depreciation is calculated.

The Depreciation Method page shows a list of available operators and constants that you can use:

-   ^ (to the power of, for example, 5^2 = 5 squared)
    
-   ( ) \* / +
    
-   any number with decimals (for example, 12345.67)
    
    Note:
    
    When creating a custom depreciation formula, you cannot use a comma for decimal places (for example, 12345,67).
    
-   IF condition THEN value if true ELSE value if true ENDIF
    
    comparison operators (<=, <, ==, !=, >, >=)
    
-   ~ (maximum of two values, for example, 2~5 = 5)
    
-   Original Asset Cost (OC) - The original cost of the asset or purchase price.
    
-   Current Asset Cost (CC) - The current asset cost is typically the same as the original cost, but provides an additional cost value to track changes when the cost differs. Write downs affect this value.
    
-   Net Book Value (NB) - The current depreciated value of the asset.
    
-   Residual Value (RV) - The lowest value the asset is reduced to. This is usually zero, unless you set a residual value for the asset.
    
-   Asset Lifetime (AL) - The number of periods an asset is depreciated for (asset effective life for tax).
    
-   Current Period or Age (CP) - The current age of the asset.
    
-   Total Depreciation Amount (TD) - The total amount of depreciation applied to the asset.
    
-   Current Usage (CU) - The current recorded usage of the asset.
    
-   Lifetime Usage (LU) - The total usage lifetime configured against the asset.
    
-   Last Depreciation Amount (LD) - The last depreciation amount.
    
-   Days held in current period (DH) - The number of days between the asset acquisition date or start of the current period (whichever is later) and the disposal date or the end of the current period (whichever is earlier).
    
-   Prior year net book value (PB) - The closing net book value at the end of the last financial year, as stored on the asset record. The **Financial Year Start** field sets the start and end of the year for the method. The Prior Year NBV updates when the month being depreciated matches the Financial Year Start month. This captures the NBV value as it was for the financial year that ended.
    
-   Depreciation Period (DP) - The number of days in a period.
    
-   Fiscal Year (FY) - The number of days in a fiscal year.
    
-   R1..Rn - A placeholder for values used in the depreciation rate table.
    
-   ROUND - If the asset's currency is Japanese Yen, this function rounds values based on the rounding preference specified in the FAM System Setup page. Otherwise, it rounds values based on the asset's currency precision.
    

### Related Topics

-   [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html)
-   [Creating a New Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2139727.html)
-   [Formula Example: Straight Line Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140285.html)
-   [Formula Example: Maximum of Two Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140329.html)
-   [Formula Example: Diminishing Value Method for Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140427.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

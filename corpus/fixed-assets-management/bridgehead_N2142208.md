---
id: "bridgehead_N2142208"
type: "bridgehead"
title: "Asset Type General Subtab"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > FAM Asset Types > Asset Type General Subtab"
parent: "section_164862669287"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142208.html"
anchors: []
sha256: "b224d2196f64b1900b974eda5feb780e7eb8605da242b23348766d1b1f520b4a"
---

On the General subtab, enter values for the following fields:

-   **Depreciation Active** - Select from the following options:
    
    -   **True** - Select this option to make this asset type active and include it in depreciation.
        
    -   **False** - Select this option if you don't want to include this asset type in depreciation.
        
    -   **On Project Completion** - For assets related to a project, this option starts depreciation when the project is completed.
        
        Note:
        
        The Depreciation Start Date and the Acquisition History record become available only when the project is closed.
        
-   **Include in Reports** - Check this box to include the asset type in the Asset Summary Report. All assets are included by default.
    
-   **Revision Rules** - Controls how revisions (revaluation) affect the asset:
    
    -   **Current Period** - The depreciation to date is recalculated using the new values, and the difference between the calculated and previously posted depreciation is posted in the current period.
        
    -   **Remaining Life** - The revision only affects future depreciation calculations from this point on.
        
-   **Depreciation Rules** - Select from the following options:
    
    -   **Acquisition** - The asset is depreciated in the same period it's made active.
        
    -   **Disposal** - The asset is depreciated in its final period.
        
    -   **Pro-rata** - The asset depreciates for a partial month in both the acquisition and disposal periods, based on a 30-day month.
        
        For example, if depreciation starts on June 18, 2011 and ends on September 17, 2011, you'll record 13 days of depreciation in the first depreciation period, and 17 days in the final depreciation period.
        
        The following are examples of pro-rata depreciation when it starts on the last day of the month:
        
        -   If depreciation starts on the last day of a 30-day month (April 30) or of a 31-day month (January 31), depreciation is recorded for 1 day in the acquisition period, and 29 days in the disposal period.
            
        -   If depreciation starts on the last day of February, depreciation in the acquisition period is calculated for 1 day plus the number of days to make 30 days. The asset depreciates for the corresponding partial month in the disposal period. For example, if depreciation starts on February 28, 3 days (the 28th plus 2 days to make 30) of depreciation is recorded for the first depreciation period, and 27 days in the final depreciation period.
            
    -   **Mid-month** - If the Depreciation Start Date is in the first half of the month (for example, July 11), depreciation starts on the same month of the asset acquisition (July). If the Depreciation Start Date is in the second half of the month (for example, June 18), depreciation starts after the month of asset acquisition (July).
        
-   **Depreciation Period** - Select whether the asset will be depreciated monthly or annually.
    
-   **Custodian** - Select the default employee responsible for this asset type.
    
-   **Supplier** - Enter the vendor that assets of this type are purchased from.
    
-   **Disposal Item** - Select a non inventory item (for sale), to use on the sales invoice, when the asset is sold.
    

### Related Topics

-   [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html)
-   [FAM Asset Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862669287.html)
-   [Asset Type Accounts Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142366.html)
-   [Asset Type Maintenance Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142485.html)
-   [Asset Type Other Methods Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142565.html)
-   [Asset Type Lifetimes Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142773.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

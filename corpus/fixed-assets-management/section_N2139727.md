---
id: "section_N2139727"
type: "section"
title: "Creating a New Depreciation Method"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > Depreciation Methods > Creating a New Depreciation Method"
parent: "section_164862696596"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2139727.html"
anchors: ["procedure_N2139766"]
sha256: "cc58a9e5e1ba67ed503001cc3c3f6790b7a91c0414d24a940b94ef8ad2fa5130"
---

In the Fixed Assets Management SuiteApp, you can create depreciation methods such as Units-of-Production Depreciation Method, or Units of Time Depreciation.

#### To create a new depreciation method: {#procedure_N2139766}

1.  Go to Fixed Assets > Setup > Depreciation Methods > New.
    
2.  On the New FAM Depreciation Method page, enter the following details:
    
    -   **Name** - Enter a name for the depreciation method.
        
    -   **Depreciation Method Description** - Enter a brief description of the depreciation method.
        
    -   **Depreciation Period** - Select the period units for depreciation calculation. You can select Monthly or Annually for Other Methods, but only Monthly for the Accounting Method
        
        -   **Monthly** - This option computes depreciation amounts monthly.
            
        -   **Annually** - This option computes depreciation amounts annually.
            
        -   **Annual Depreciation, Monthly Posting** - This option computes the depreciation annually, divides the amount into 12, and posts it to the depreciation journal every month.
            
            The Japanese National Tax Authority requires a different calculation to determine the depreciation amount for months 1-11 and for month 12. For month 12, the depreciation value is calculated as the difference between the total annual depreciation and the sum of the first 11 months. For example, if an asset is valued at $1,000,000 and should be depreciated by $500,000 on Year 1, depreciation amount is calculated as follows:
            
            Depreciation for Months 1-11:
            
            -   $500,000 / 12 = $41,666.66
                
            -   Round up = **$41,667**
                
            
            Depreciation for Month 12:
            
            -   $500,000 - Sum of depreciation for Months 1-11
                
            -   $500,00 - ($41,667\*11)
                
            -   $500,000-458,337 = **$41,663**
                
            
            Note:
            
            For this depreciation period, the asset lifetime reflects the number of fiscal years for the asset. Selecting this depreciation method adjusts the asset's depreciation end date to the end of the last fiscal year. This depreciation period is only available for Japan.
            
    -   **End Period Number** - If this depreciation method covers a limited period (for example, only the first 12 months of the asset's life), enter the number of periods that the depreciation method can be used for. If left blank, depreciation continues until the asset is fully depreciated or retired.
        
    -   **Next Depreciation Method** - This feature lets you link depreciation methods. If the current depreciation method covers a limited period (for example, only the first 12 months of the asset's life), select the next depreciation method to use after the current method's end period.
        
    -   **Depreciation Rate Table** - Select the depreciation table that the system uses to set the depreciation rates to this method. These options are currently only applicable to Japan depreciation.
        
        See [FAM 20.2 Japan Depreciation Rate Table](https://system.netsuite.com/app/help/helpcenter.nl?fid=FAM20.2_JapanDepreciationRateTable.pdf) to check the rates used to compute depreciation for each rate table.
        
    -   **Depreciation Formula** - Use the terms on the screen to enter a formula expression for this depreciation method. The formula will display with underline to show how terms are grouped with operators. This visual guide helps you determine if extra parentheses are needed to change the evaluation order.
        
    -   Select from the following **Final Period Convention** options:
        
        Note:
        
        This field is relevant only to accruals.
        
        If left blank, **Fully Depreciate** is assigned by default.
        
        -   **Fully Depreciate** - Includes the remaining balance in the final period calculation so the remaining value becomes zero.
            
        -   **Retain Balance** - Calculates the final period using the relevant accrual convention without including any remaining balance. The remaining value doesn't become zero.
            
        -   **Value Based** - Extends asset depreciation beyond its useful life until the net book value equals the residual value.
            
3.  Click **Save**.
    

### Related Topics

-   [Fixed Assets Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126441.html)
-   [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html)
-   [Preconfigured Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2137654.html)
-   [Depreciation Formula](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140095.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

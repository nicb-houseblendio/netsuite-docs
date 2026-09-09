---
id: "section_N2150936"
type: "section"
title: "Restricting the Editing of Asset Values"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Updating Fixed Assets Management Records > Restricting the Editing of Asset Values"
parent: "chapter_N2147919"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html"
anchors: []
sha256: "55ce5465473d16ac63a366cac27936b5e9fde4cf7b41c5c88ef762f6a9dd6ed9"
---

On the Fixed Assets Management System Setup page, you can restrict the editing of asset values. You can edit asset values manually on the Edit FAM Asset page, by inline editing on the Asset list, or by CSV import.

On the System Setup page, checking the **Allow Asset Value Editing** box gives the Administrator role full permission to edit asset record values. You can also let other users edit asset values by granting permission to additional roles.

Warning:

When you enable **Allow Asset Value Editing**, you can edit fields that are otherwise locked to prevent errors. Be aware that changing any of these fields without updating the related records can cause errors in the system.

If the **Allow Asset Value Editing** box isn't checked, most fields are set to read-only to prevent asset editing.

-   The following fields are set to read-only to prevent manual editing by anyone, regardless of the asset condition and user's role:
    
    -   Cumulative Depreciation
        
    -   Last Depreciation Period
        
    -   Last Depreciation Amount
        
    -   Last Depreciation Date
        
    -   Asset Status
        
-   When depreciation has started for an asset (the **Cumulative Depreciation** field has a value more than zero), or when the **Asset Status** is **Disposed**, the following fields are set to read-only to prevent manual editing by anyone, regardless of the user's role:
    
    -   Accounting Method
        
    -   Residual Value Percentage
        
    -   Residual Value
        
    -   Asset Lifetime
        
    -   Asset Lifetime Usage
        
    -   Asset Original Cost
        
    -   Asset Current Cost
        
    -   Purchase Date
        
    -   Depreciation Start Date
        
    -   Depreciation End Date
        
    -   Depreciation Rules
        
    -   Currency
        
    -   Quantity
        
    -   Asset Serial Number (not editable only if a value has been saved for this field)
        
    -   Alternate Asset Number (not editable only if a value has been saved for this field)
        
    -   Current Net Book Value (even if the field is disabled, the value can be updated if the asset is new)
        

### Related Topics

-   [Fixed Assets Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126441.html)
-   [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html)
-   [Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862707730.html)
-   [Creating Asset Records through CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689335971.html)
-   [Adding Tax Depreciation Methods to an Asset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141463.html)
-   [Updating Asset Records Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148181.html)
-   [Adding Alternate Depreciation Methods Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html)
-   [Manually Editing Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150682.html)
-   [Creating FAM Alternate Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2153972.html)
-   [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html)
-   [Depreciation History Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154557.html)
-   [Triggering the Asset Reset Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530828764.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

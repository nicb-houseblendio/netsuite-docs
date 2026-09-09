---
id: "section_N1814149"
type: "section"
title: "Setting Tax Rounding Levels, Methods, and Precision Settings"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Setting Tax Preferences > Setting Tax Rounding Levels, Methods, and Precision Settings"
parent: "section_N1813668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html"
anchors: ["procedure_N1814170"]
sha256: "c1875948d704391651b435f9aad30761ffdb06d5f8f6a5e7e1fbcccc8046c1b5"
---

Important:

It is critical to specify the rounding precision and rounding method for tax values based on the requirements of your tax authority. Failure to do so could result in incorrect tax amounts being reported. Also note that at this time, it isn't possible to specify Rounding Precision or Rounding Method using CSV Import, Web Services, or Mass Updates. You must specify these values either on the Setup > Accounting > Setup Taxes page under the tab for the country, or check the **Allow override rounding setting per Entity** box to specify rounding settings on each customer and vendor record.

For each nexus, on the Set Up Taxes page (Setup > Accounting > Set Up Taxes), define the tax rounding levels, methods, and precision settings that apply the preferences, described in the procedure below.

#### To set tax rounding levels, methods, and precision settings: {#procedure_N1814170}

1.  **Tax Rounding Level**
    
    Note:
    
    The **Tax Rounding Level** preference isn't available for U.S. and Canada. It is only available for nexuses that use VAT/GST.
    
    Note:
    
    The Allow override rounding setting per entity does not consider the tax rounding level. If the **Allow Override Rounding Setting per Entity** box is checked, the line level rounding type is then used.
    
    Specify the tax rounding level for this nexus:
    
    -   If you select **Item Line Level**, tax is rounded per line.
        
    -   If you select **Transaction Level**, the rounding is applied at the tax total level, using this formula: round (Subtotal x Tax Rate) = Tax Total.
        
    
    Note:
    
    Transaction level tax rounding is applicable only to the following transaction types: credit memos, opportunities, estimates, purchase orders, vendor bills, vendor credits, sales orders, invoices, and cash sales. The rounding adjustment is done on each subtab (**Item**, **Billable Item**, **Billable Time**, and **Billable Expense**).
    
    If the nexus has been configured to calculate tax at the transaction level, then when you add an item line to the transaction, the system immediately validates the calculations. If NetSuite finds a discrepancy between the rounded total tax amount and the sum of the rounded tax amounts per line, the system adjusts the tax amount on the line that results in the minimum percentage change in tax amount. But if all the item lines have the same amounts, the system will do the adjustment on the last line.
    
    You can manually change the tax amounts of any of the lines only if the tax rounding level has been set to Item Line Level. For roundings set at Transaction Level, the tax amount and gross amount columns on item lines are set to read-only in the user interface. If there are multiple tax codes in one transaction, the rounding is done within each group of item lines that share the same tax code, and the total tax is the sum of the rounded tax for each group.
    
2.  **Tax Rounding Precision**
    
    Note:
    
    The **Tax Rounding Precision** preference isn't available for Australia, Canada, UK, and US. Also note that Japan does not use decimal places (see [Japan Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1934076.html)).
    
    Specify the decimal or whole number precision you want to use for values entered in tax reports for this nexus. The following options are available:
    
    -   **.01 and Below** - Values in tax fields will be rounded to two decimal points. (Default)
        
    -   **.1 and Below** - Values in tax fields will be rounded to one decimal point.
        
    -   **1 and Below** - Values in tax fields will be rounded to the nearest single integer.
        
    -   **10 and Below** - Values in tax fields will be rounded to the nearest 10 points.
        
    -   **100 and Below** - Values in tax fields will be rounded to the nearest 100 points.
        
3.  **Tax Rounding Method**
    
    Note:
    
    The **Tax Rounding Method** preference isn't available for Australia, Canada, UK, and US.
    
    Specify how to apply the Rounding Precision to tax field values for this nexus. The following options are available:
    
    -   **Round off** - Values in tax fields will be rounded to the nearest integer or decimal place specified in the Tax Rounding Precision field.
        
    -   **Round down** - Values in tax fields will be rounded down to the nearest integer or decimal place specified in the Tax Rounding Precision field.
        
    -   **Round up** -Values in tax fields will be rounded up to the nearest integer or decimal place specified in the Tax Rounding Precision field.
        
4.  **Apply Rounding precision setting if Currency precision isn't 0**
    
    Note:
    
    The **Apply Rounding precision setting if Currency precision isn't 0** preference isn't available for Australia, Canada, UK, and US.
    
    Check this box to use the specified Rounding Precision setting and Rounding method when the Currency setting is set to any value other than 0. By default, this box is clear, so that the level of precision specified in the currency will be applied to values in tax fields for this nexus.
    
    If the **Apply rounding precision setting if currency precision isn't 0 box** is checked, NetSuite will round every value in the specified currency, which means this preference overrides all other rounding preferences. The following scenarios illustrate this behavior:
    
    -   If the **Apply rounding precision setting if currency precision isn't 0** box is checked, and the **Tax Rounding Level** field is set to **Transaction Level**, the system ignores the transaction level rounding because the amount is already rounded based on currency.
        
    -   If the **Apply rounding precision setting if currency precision isn't 0** box is checked, and the **Allow override rounding setting per Entity** box is checked, the system ignores the rounding setting specified on the Entity record.
        
5.  **Allow override rounding setting per Entity**
    
    Note:
    
    The **Allow override rounding setting per Entity** preference isn't available for Australia, Canada, UK, and US.
    
    Check this box if you want to set the tax rounding method and precision for each customer or vendor individually for this nexus.
    
    To set the tax rounding method and precision for a customer or vendor, open the customer or vendor record. On the Financial subtab, set the method and precision in the **Tax Rounding Precision** field and the **Tax Rounding Method** field.
    
    If the **Allow override rounding setting per Entity box** isn't checked, tax amounts will follow the tax rounding method and precision defined for the country nexus, no matter what tax rounding method and precision have been set for customers and vendors. If tax rounding preferences are not defined on the entity record, the system uses the preferences defined for the country nexus.
    

Note:

For information about the other fields on the Set Up Taxes page, see [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html).

### Related Topics

-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

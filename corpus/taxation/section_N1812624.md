---
id: "section_N1812624"
type: "section"
title: "Managing Tax Rate Changes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Managing Tax Rate Changes"
parent: "chapter_N1805198"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812624.html"
anchors: ["bridgehead_N1812663", "bridgehead_N1812712", "bridgehead_N1812724", "bridgehead_N1812736"]
sha256: "be1d4e9c1273644177dbbb429c225de3d66233a255216bba376aeec34129b4b4"
---

Note:

This topic isn't applicable to US and Canada edition accounts.

Tax authorities announce rate changes, and the rules can vary. Administrators of accounts with the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) are usually notified of upcoming rate changes, but it's your responsibility to make sure you're using the latest rates. Check rates carefully before updating your account.

Important:

Don't change the rate on the current tax codes. This could affect historical records and audit accountability.

#### To update tax rates: {#bridgehead_N1812663}

1.  Rename your current tax codes if you want to use your own naming convention.
    
2.  Create a new tax code, adding the date it takes effect in the **Effective Date** field. Rename the old code first, then use the original name for the new tax code.
    
3.  Inactivate the old tax code or add the validity date in the **Valid Until** field.
    
4.  If you've enabled Advanced Taxes in your account, update the tax schedules.
    
5.  Update default tax codes on customer, vendor, and item records.
    

## When should you make these changes? {#bridgehead_N1812712}

The decision on when to make these changes will depend on several factors, such as the following:

-   the effective date of the new rate
    
-   whether you trade over the weekend
    
-   whether you have a web store
    
-   the rules pertaining to that country
    

## My Item prices in NetSuite are VAT inclusive, what do I have to do? {#bridgehead_N1812724}

No action is needed because NetSuite stores prices on a net basis. When you change the tax code, your item record updates automatically.

## Example {#bridgehead_N1812736}

Here's how to manage a standard VAT rate change from 20% to 21% starting January 1, 2013, in Czechia (CZ).

1.  Rename the current tax codes if you would like to use your own naming convention.
    
    1.  Go to _Setup > Accounting > Taxes > Tax Codes_.
        
    2.  Click the Edit link of the current Standard rate tax code.
        
    3.  On the Edit Tax Code page, rename the tax code (for example, rename your current standard tax code S-CZ to S2012-CZ)
        
    4.  For a European Union (EU) member state, also rename the tax codes you use for EU zero rated sales, reverse charge sales and other related tax codes. For example, rename ES-CZ to ES2012-CZ.
        
2.  Create the new Tax Code effective January 1, 2013
    
    1.  Go to _Setup > Accounting > Taxes > Tax Codes_.
        
    2.  Click **New**.
        
    3.  If Advanced Taxes is enabled, select the nexus.
        
    4.  Create the standard rate tax code with the new rate and use the original name (S-CZ with the rate of 21%).
        
    5.  For an EU member state, create additional tax codes for:
        
        -   EU goods and related services
            
        -   Reverse charge services
            
        -   Purchase of services where the reverse charge rules apply
            
        
        For each of these tax codes, set the notional rate to the new rate and select the right properties for each tax code. The properties have to be the same as the old tax codes.
        
    6.  Select a date in the **Effective From** field. In this example, January 1, 2013.
        
3.  Inactivate the old standard rate and other tax codes that are no longer required.
    
    Depending on the rules in that particular country, consider the following questions:
    
    -   Will you issue credit notes for invoices raised before January 1, 2013?
        
    -   Do you have stock adjustments or sales orders fulfilled but not yet invoiced?
        
    
    If the answer is no to both, inactivate the old tax code.
    
    If you answer yes to either, leave it for now and inactivate it later.
    
    1.  Go to _Setup > Accounting > Taxes > Tax Codes_.
        
    2.  Click the Edit link of the old Standard rate tax code.
        
    3.  On the Edit Tax Code page, check the **Inactive** box.
        
4.  If the Advanced Taxes feature is enabled in your account, update the tax schedules.
    
    1.  Go to _Setup > Accounting> Taxes > Tax Schedules_.
        
    2.  Select the tax schedule (for example, Standard).
        
    3.  On the **Non-US Nexuses** subtab, make sure that the new tax codes are shown.
        
5.  Update the customer, vendor, and item records, to reflect the new tax codes, if applicable. If Advanced Taxes is enabled, select the updated tax schedule on item records.
    

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

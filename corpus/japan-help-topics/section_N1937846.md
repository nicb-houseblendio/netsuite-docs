---
id: "section_N1937846"
type: "section"
title: "Deductible Purchase Tax for Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Tax Topics > Deductible Purchase Tax for Japan"
parent: "chapter_N1934076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937846.html"
anchors: []
sha256: "c6a385f70d08b679201eb583a6f3d0533c47ac2c52849ccf2f156b5b53db74c0"
---

Important:

Starting April 1, 2012, Japanese companies can deduct all purchase tax amounts only if their taxable sales are more than 95% and their annual sales are less than 500M JPY.

The Japan Localization SuiteApp supports deductible purchase tax for Japan subsidiaries and their purchase transactions and records.

These transactions can be subject to deductible purchase tax:

-   purchase orders
    
-   vendor bills
    
-   vendor returns
    
-   vendor credit
    
-   journal entry
    
-   expense report
    

For deductible purchase tax to work, you must enable these required features:

-   A/P
    
-   purchase order
    
-   vendor return
    
-   expense report
    

Before you can subject transactions or records to deductible purchase tax, you should first apply purchase tax rates to corresponding tax codes.

#### To set purchase tax rates to tax codes:

1.  Go to Setup > Accounting > Tax Codes.
    
2.  Edit a Japan tax code for standard rate and reduced rate.
    
3.  In the **Tax Deductible** field, select either **100%**, **80%** or **50%**.
    
    The purchase tax rate selected is the percent that will be deducted from the transaction tax amount.
    
4.  Click **Save**.
    

Next, you should apply the tax code, with deductible purchase tax rate, to purchase transactions or records.

#### To apply a tax code with purchase tax rate to transactions or records:

1.  Create or edit supported purchase transaction or record that you want to subject to deductible purchase tax.
    
2.  Do any of these steps:
    
    -   For a purchase transaction or a journal entry, ensure that a Japan subsidiary is selected.
        
    -   For an expense report, ensure that an employee from a Japan subsidiary is selected.
        
3.  Select any of these tax codes with purchase tax rate you want in the **Tax Code** field:
    
    -   a line item on the **Expenses and Items** subtab of a purchase transaction
        
    -   a line item on the **Expenses** subtab of an expense report
        
    -   a debit or credit line on the **Lines** subtab of a journal entry
        
    -   an item or expense on the **Lines** subtab or **Expense** subtab of a purchase order, if the preference **Allow Expenses on Purchases** is enabled for purchase orders
        
4.  Click **Save**.
    

You can use CSV import to input or update deductible purchase tax values for **Account**, **Tax Codes** and **Amount** fields on purchase orders, vendor bills, vendor returns, vendor credit, journal entry, and expense report. This is applicable to the item and expense sublists of supported purchase transactions.

Note:

In CSV import, if you want to input or update and already explicitly set the **Amount**, **Tax** and **Gross Amount** in the CSV file of journal entries and expense reports, you must disable or clear **Run Server SuiteScript and Trigger Workflows** in **Advanced Options**. For more information, see [Server Scripting and Workflow Execution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676525683.html).

Deductible purchase tax is automatically calculated by NetSuite, and then applies it on the transaction tax amount, which is indicated on relevant tax reports.

Note:

Consider these cases:

-   If the preference, **Allow Expenses on Purchases**, is enabled for purchase orders, then expenses or items on the Expense subtab of purchase orders (aside from items on the Lines subtab) can be subject to deductible purchase tax.
    
-   The tax agency accepts only rounding down or rounding off the tax amount for transactions with deductible purchase tax rates. Use Round Down or Round Off only for purchase tax. Don't use Round Up. For more information, see [Setting Tax Rounding Methods - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1935242.html).
    
-   Don't use Tax Group for your transactions, use Tax Codes instead. Deductible purchase tax isn't available on tax groups.
    
-   Deductible purchase tax calculation isn't yet included in the appendices of the Japan Consumption Tax Form.
    

### Related Topics

-   [Japan Consumption Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1934460.html)
-   [Tax Categories for Individual Calculation of Deductible Purchase Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1938040.html)
-   [Using Tax Categories on Transactions and Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1938146.html)
-   [Purchase Tax by Tax Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1565782452.html)
-   [Setting Up Consumption Tax - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1934652.html)
-   [Setting Tax Rounding Methods - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1935242.html)
-   [Selecting Precision Settings - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937177.html)
-   [Japan Consumption Tax Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937672.html)
-   [What goes into each box - Japan Consumption Tax Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4824768809.html)
-   [Japan Consumption Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1565781755.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

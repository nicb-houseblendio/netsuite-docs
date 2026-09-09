---
id: "section_N1859840"
type: "section"
title: "Paying Provincial Sales Tax - Canada"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Tax Topics For Accounts Without SuiteTax > Paying Provincial Sales Tax - Canada"
parent: "section_156941156434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html"
anchors: ["procedure_N1859889"]
sha256: "deb02e1fc8b5b81e7f8f6c62d297104f5e083601844978d7f8cb8d920e749bed"
---

A tax payment is a remittance to a tax authority. When you specify a tax agency and tax rate in an invoice or sales receipt, NetSuite calculates tax for any items marked as taxable and includes that tax in the total amount you charge your customer. The amount of a tax payment is based on these tax calculations.

#### To pay sales tax: {#procedure_N1859889}

1.  For accounts that are not OneWorld, go to Transactions > Bank > Pay PST (Administrator).
    
    For OneWorld accounts, go to Transactions > Bank > Pay Sales Tax (Administrator).
    
    The Sales Tax Payment page shows a list of all tax codes and the amount you owe for each.
    
2.  If you have subsidiaries, select the subsidiary you are paying sales tax for.
    
3.  Select the bank account to be used for this payment. Only the accounts associated with this subsidiary are shown here. To associate an account with a subsidiary, open the account record, and select the subsidiary in the **Subsidiary** field. The balance for the account you selected shows in the **Account Balance** field.
    
4.  If you are using Advanced Taxes, select the nexus you are paying sales tax for.
    
5.  Accept or select a date in the **Date** field.
    
6.  In the **Posting Period** field, select the period to which you want to post this sales tax payment. If a period is closed, you can't post to that period.
    
7.  Check the **To Be Printed** box if you want to save this transaction in a print queue to print later.
    
8.  In the **Adjustment Account** field, select an account to record the amount of the sales tax liability. This liability amount is based on the values in the **Adjustment** column.
    
9.  In the **Memo** field, enter the memo that you want to appear on the check.
    
10.  On the **Tax Codes** subtab, do the following:
     
     1.  In the **End Date** field, enter a date to filter the sales tax liabilities. Only the open tax liabilities incurred on and before this date populate the **Tax Codes** subtab and are calculated in the **Amount Due** column. The end date defaults to the current date.
         
     2.  Check the **Include All Payments Made After End Date** box if you want all the tax payments, including those paid after the end date, to be taken into account when calculating the tax liability.
         
     3.  Check the box in the **Pay** column next to the tax codes you want to pay. Click **Mark All** to select all items on the page. The total of the payment appears in the **Amount** field.
         
     4.  In the **Adjustment** column, you can enter an amount to adjust a specific sales tax liability linked to a tax code. For example, you can use this feature to enter a discount for early payment.
         
         Enter a positive amount to increase liability and a negative amount to decrease liability. The difference posts as a line on the sales tax payment to the adjustment account you specify in the header.
         
         Adjustments entered will apply to the period that you selected for this sales tax payment.
         
11.  The **Other Tax Payable** subtab shows journal entry transactions that credit your sales tax payables by being assigned to a tax agency, but are not linked to a tax code. For example, you can view a journal entry that credits sales tax payable, debits an expense account, and is assigned to a tax agency vendor.
     
     On this subtab, check the box in the **Pay** column next to the other tax payables you want to pay.
     
12.  Click **Save**. NetSuite automatically creates a check transaction.
     

To print the check, go to _Transactions > Management > Print Checks and Forms_, and click the Checks link.

For more information about setting up tax agencies, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).

### Related Topics

-   [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html)
-   [Creating Tax Codes - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856762.html)
-   [Creating Tax Groups - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857206.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
-   [Viewing Canadian Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1860262.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Processing Goods and Services Tax (GST) Refunds - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859567.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

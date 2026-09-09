---
id: "section_N2041996"
type: "section"
title: "Paying Sales Tax - United States"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Paying Sales Tax - United States"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html"
anchors: ["procedure_N2042039"]
sha256: "f8066e2f01a724ff70726d95c2ac013b4c1a45640893b46d6d896346a6c16635"
---

A tax payment is a remittance to a tax authority, which you have set up as a vendor. When you specify a tax agency and tax rate on an invoice or sales receipt, NetSuite calculates tax for any items marked as taxable. Then, the calculated tax is included in the total amount you charge your customer. The amount of a tax payment is based on these tax calculations.

#### To pay sales tax: {#procedure_N2042039}

1.  Go to _Transactions > Bank > Pay Sales Tax_. The Sales Tax Payment page shows a list of all tax items and the amount you owe for each.
    
2.  Select the subsidiary you are paying sales tax for.
    
3.  Select the bank account to be used for this payment.
    
    Only the accounts associated with this subsidiary are shown here. To associate an account with a subsidiary, open the account record, and select the subsidiary in the **Subsidiary** field.
    
4.  If the Advanced Taxes feature is enabled, select the nexus you are paying sales tax for.
    
5.  Accept or select a date in the **Date** field.
    
6.  In the **Posting Period** field, select the period you want to post this sales tax payment to. If a period is closed, you can't post to that period.
    
    The balance for the account selected shows in the **Account Balance** field.
    
7.  Check **To Be Printed** if you want to save this transaction in a print queue to print later.
    
8.  In the **Adjustment Account** field, select an account to record the amount of the sales tax liability. This liability amount is based on the values in the **Adjustment** column.
    
9.  In the **Memo** field, enter the memo that you want to appear on the check.
    
10.  On the **Tax Codes** subtab, do the following:
     
     1.  In the **End Date** field, enter a date to filter the sales tax liabilities. Only the open tax liabilities incurred on and before this date populate the **Tax Codes** subtab and are calculated in the amount due column. The end date defaults to the current date.
         
     2.  Check the **Include All Payments Made After End Date** box if you want all the tax payments, including those paid after the end date, to be taken into account when calculating the tax liability.
         
     3.  Check the box in the **Pay** column next to the tax codes you want to pay. Click **Mark All** to select all items on the page. The total of the payment appears in the **Amount** field.
         
     4.  In the **Adjustment** column, you can enter an amount to adjust a specific sales tax liability linked to a tax code. For example, you can use this feature to enter a discount for early payment.
         
         To increase liability, enter a positive amount. To decrease liability, enter a negative amount. The difference posts as a line on the sales tax payment to the adjustment account you specify in the header.
         
         Adjustments entered will apply to the period that you selected for this sales tax payment.
         
11.  The **Other Tax Payable** subtab shows journal entry transactions that credit and debit (net amount is shown) your sales tax payables by being assigned to a tax agency but are not linked to a tax code. For example, you can view a journal entry that credits Sales Tax Payable, debits an expense account, and is assigned to a tax agency vendor. However, if there are also transactions that debit Sales Tax Payable, the net amount is shown.
     
     On this subtab, check the box in the **Pay** column next to the **Other Tax Payables** you want to pay.
     
12.  Click **Save**. NetSuite automatically creates a check transaction.
     

To print the check, go to _Transactions > Management > Print Checks and Forms_, and click the Checks link.

For more information about setting up tax agencies, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)
-   [U.S. Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042330.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

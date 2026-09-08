---
id: "bridgehead_N252671"
type: "bridgehead"
title: "Transaction Numbers Available for Auto-Numbering"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Set Auto-Generated Numbers > Records and Transactions Available for Auto-Numbering > Transaction Numbers Available for Auto-Numbering"
parent: "section_N252520"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N252671.html"
anchors: []
sha256: "d5913b04444b0981cb62100450fe56133c924fd6efc279d1e0774aef01537629"
---

Some transaction types listed on the Transaction Numbers subtab of the Set Up Auto-Generated Numbers page are not available if the features aren't enabled in your account.

Auto-generated transaction numbers are internal, gapless, and can't be changed. They're generated for each standard and custom transaction type when you save the record.

For more information, see [Auto-Generated Transaction Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4340444343.html).

Important:

In the old Transactions subtab, you could overwrite the internal number of transactions if the Allow Override box was checked for the transaction type. That could cause duplicate internal numbering in these historical transactions. In the new Transaction Numbers subtab, you can't overwrite transaction numbers, only document numbers. NetSuite doesn't renumber historical internal transaction numbers.

If the Use Deletion Reason feature is enabled in your account, users must provide a reason when deleting transaction type records. For more information, see [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html).

You can place letters before or after the numbers of the following transaction types:

| Assembly Build | Assembly Unbuild |
| --- | --- |
| Bill (Vendor Bill) | Bill Credit (Vendor Credit) |
| Bill Payment (Vendor Payment) | Bin Putaway Worksheet |
| Bin Transfer | Blanket Purchase Order |
| CCard Refund (Credit Card Refund) | Cash Refund |
| Cash Sale | Check |
| Commission | Credit Card (Customer Credit Card Charge) |
| Credit Memo | Currency Revaluation |
| Custom | Customer Deposit |
| Customer Refund | Deposit |
| Deposit Application | Estimate |
| Expense Report | Finance Charge Note: This numbering sequence is shared with Invoice. |
| Fixed Asset Accrual | Inventory Adjustment |
| Inventory Cost Revaluation | Inventory Count |
| Inventory Distribution | Inventory Transfer |
| Inventory Worksheet | Invoice Note: This numbering sequence is shared with Finance Charge. |
| Item Fulfillment | Item Receipt |
| Journal | Opportunity |
| Paycheck | Paycheck Journal |
| Payment (Customer) | Payroll Adjustment (Year-to-Date) |
| Payroll Liability Check | Purchase Contract |
| Purchase Order | Request For Quote |
| Requisition | Return Authorization |
| Revenue Commitment | Revenue Commitment Reversal |
| Revenue Contract | Sales Order |
| Sales Tax Payment (Tax Payment) | Statement Charge |
| Store Pickup Fulfillment | Tax Liability Cheque (Tax Liability) |
| Tegata Payable | Tegata Receivable |
| Transfer | Transfer Order |
| Vendor Request For Quote | Vendor Return Authorization |
| Work Order | Work Order Close |
| Work Order Completion | Work Order Issue |

Account-based transaction types display an additional read-only, auto-generated number in the Transaction Number field. You'll see this additional number on Check transactions, where the numbering sequence depends on a particular account. You'll also see these numbers on transactions where the numbers are used for external reference, such as Vendor Bill.

Here are the transaction types where the numbering sequences are either account-based or externally referenced:

-   Bill (Vendor Bill), Externally referenced
    
-   Bill Credit (Vendor Credit), Externally referenced
    
-   Bill Payment (Vendor Payment), Account-based
    
-   Check, Account-based
    
-   Credit Card Charge (Customer Credit Card), Externally referenced
    
-   Credit Card Refund (CCard Refund), Externally referenced
    
-   Customer Refund, Account-based
    
-   Paycheck, Account-based
    
-   Payroll Liability Check, Account-based
    
-   Sales Tax Payment (Tax Payment), Account-based
    
-   Tax Liability Cheque (Tax Liability), Account-based
    

Note:

The **Transaction Number** field is visible by default on standard NetSuite forms, but not on custom forms. You can customize a form to show this field if you want.

By default, transaction lists show only the **Number** field in searches and reports. The **Transaction Number** field is different from the **Number** field for the account-based and externally referenced transaction types listed previously. For all other transaction types, the two values are the same.

Important:

If you copy an externally referenced transaction such as Vendor Bill, the reference number isn't copied to avoid duplicates.

Warning:

You can't auto-generate numbers for journals if you set the Always Allow Per-line Classifications on Journals preference.

### Related Topics

-   [Records and Transactions Available for Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252520.html)
-   [Entity Records Available for Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N252528.html)
-   [Document Numbers Available for Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4341187904.html)
-   [CRM Records Available for Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N253217.html)
-   [Schedule Records Available for Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N253307.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

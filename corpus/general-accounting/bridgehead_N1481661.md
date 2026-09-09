---
id: "bridgehead_N1481661"
type: "bridgehead"
title: "Accepting a Customer Payment to Write Off Bad Debt"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Bad Debt Overview > Accepting a Customer Payment to Write Off Bad Debt"
parent: "section_N1481280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1481661.html"
anchors: ["procedure_N1481674"]
sha256: "e372e5063d76b8a6c57b8cf2999e9e2a3e82b54ab0eb99e3e0061a583c8cd225"
---

After you have entered a journal entry to write off bad debt, the next task is to accept a customer payment.

After this payment record is saved, the invoice is no longer included in the Open Invoices report or in A/R Aging reports. You aren't required to void the invoice.

#### To accept a zero customer payment amount: {#procedure_N1481674}

1.  Go to _Transactions > Customers > Accept Customer Payment_.
    
2.  In the **Customer** field, select the customer with the unpaid invoice.
    
    You can change the **Date** if appropriate, but accept the default choice of **Undeposited Funds**.
    
3.  In the **A/R Account** field, select a posting account for this transaction.
    
    Only invoices charged to this account show in the list.
    
4.  Click the **Apply** subtab.
    
5.  Click the **Credits** subtab and then check the **Apply** box for the journal entry you created.
    
6.  Click the **Invoices** subtab and then check the **Apply** box for the unpaid invoice.
    
    The Payment Amount is automatically set to 0.00.
    
7.  Click **Save**.
    

The payment isn't included in the customer payments list page because the payment amount is 0.

Because the payment amount is 0.00, the general ledger isn't affected by this transaction. For information about the general ledger impact of other customer payment transactions, see [Customer Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html).

### Related Topics

-   [Bad Debt Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481280.html)
-   [Allowance for Bad Debts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4279824892.html)
-   [Creating a Journal Entry to Write Off Bad Debt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1481347.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

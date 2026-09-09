---
id: "section_N1775784"
type: "section"
title: "Associating Amortization Templates with Expenses"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Associating Amortization Templates with Expenses"
parent: "section_N1767815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html"
anchors: ["procedure_N1775815"]
sha256: "29016fdcb28b001af4a8f13b80e4a6ddf605c89b5b9e0cc732a3b6b8e75edc41"
---

Amortization templates can be used to generate amortization schedules for expenses, based on the association of templates with expense lines on vendor bills and credits.

You can select amortization templates for expense lines on vendor bill and vendor credit transactions. To amortize an expense line, a deferral account must be specified on the expense account record or the amortization template record. If both records have deferral accounts, the template's deferral account is used. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).

#### To associate an amortization template with a transaction expense line: {#procedure_N1775815}

1.  Do one of the following:
    
    -   For vendor bills, go to _Transactions > Payables > Enter Bills_.
        
    -   For vendor credits, go to _Transactions > Payables > Enter Vendor Credits_.
        
2.  Under Primary Information, select a **Vendor**, and select values for other fields as needed.
    
3.  On the **Expenses** subtab, select an expense account and an amount.
    
4.  In the **Amort. Schedule** column, select the appropriate template.
    
    A deferral account must be specified on either the template or the item record. Since expense lines don't include items, be sure to select an amortization template that specifies a deferral account. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
    If you select a variable template, you must also select the associated project in the Customer column dropdown.
    
5.  Enter an amortization start and end date, if needed.
    
    An error occurs if either of these dates is in an accounting period that isn't yet set up. You must create accounting periods for the range of time your amortization schedules will cover. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).
    
    An error also occurs if either of these dates is before the posting period selected for the transaction.
    
6.  Enter the residual amount not to be recognized, if needed.
    
    The following screenshot of a portion of a vendor bill shows the required fields to associate an amortization template with an expense line. The layout of a vendor credit is similar.
    
    ![Screenshot of portion of a vendor bill showing the required fields to associate an amortization template with an expense line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/VendorBillExpenseLineAmortization.png)
7.  Enter additional information as needed for this line item.
    
8.  Click **Add**.
    
9.  Repeat steps 3-8 for additional items as needed.
    
10.  Click **Save**.
     

Note:

This process is basically the same when you generate a credit directly from a vendor bill, except that any amortization information set for expense lines on the bill is inherited by the credit and can't be changed.

### Related Topics

-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html)
-   [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html)
-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

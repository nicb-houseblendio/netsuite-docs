---
id: "section_N1295419"
type: "section"
title: "Correcting Account Balances for NSF Checks Using a Journal Entry"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Payments > Handling Returned/NSF Checks > Correcting Account Balances for NSF Checks Using a Journal Entry"
parent: "section_N1295030"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295419.html"
anchors: ["procedure_N1295450", "bridgehead_4586549341", "procedure_4586482573", "procedure_4586485705"]
sha256: "6e59e6f1d3fe041ec797966ac3b4da1387f1d58c24718f8cb4ac3f1a48e215a3"
---

To make corrections for an insufficient funds check, you can make a journal entry that reverses the impact of the payment from the check and creates a new accounts receivable balance.

Important:

Please note that by using the journal entry method, the original invoice remains closed and the balance due shows as a **new** receivable and is not aged based on the original receivable.

#### To make an NSF correction journal entry, you must perform the following tasks: {#procedure_N1295450}

1.  Debit the amount of the NSF check from the Accounts Receivable account. For details on debiting an amount from a ledger account, see [Debiting and Crediting Amounts Using Journal Entries](#bridgehead_4586549341).
    
2.  Credit the amount of the NSF check to the bank account affected by the NSF check. For information on crediting an amount using a journal entry, see [Debiting and Crediting Amounts Using Journal Entries](#bridgehead_4586549341).
    
3.  Debit the bank fee from the expenses account for the bank service fee.
    
4.  Credit the amount of the bank fee to the bank account affected by the bank service fee for this NSF check.
    
5.  Debit the amount of the fee you charge for a returned check from the Accounts Receivable account.
    
6.  Credit the amount of the fee you charge for a returned check to the income account for NSF check fees.
    

## Debiting and Crediting Amounts Using Journal Entries {#bridgehead_4586549341}

NetSuite enforces double-entry bookkeeping, so journal entries post changes to accounts using offsetting debits and credits. Each journal entry includes at least one debit amount and at least one credit amount.

#### To debit an amount from an account using a journal entry: {#procedure_4586482573}

1.  Go to _Transactions > Financial > Make Journal Entries_.
    
2.  On the **Lines** subtab:
    
    1.  In the **Account** field, select the ledger account from which you want to debit the amount.
        
    2.  In the **Debit** field, enter the amount you want to debit.
        
    3.  In the **Name** field, select a name of a person, vendor, or company to associate with this entry (Optional).
        
3.  Click **Save**.
    

#### To credit an amount to an account using a journal entry: {#procedure_4586485705}

1.  Go to _Transactions > Financial > Make Journal Entries_.
    
2.  On the **Lines** subtab:
    
    1.  In the **Account** field, select the ledger account to which you want to credit the amount.
        
    2.  In the **Credit** field, enter the amount you want to credit.
        
    3.  In the **Name** field, select a name of a person, vendor, or company to associate with this entry (Optional).
        
3.  Click **Save**.
    

For more information on creating journal entries, read [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

### Related Topics:

-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)
-   [Returned Check/NSF Fees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295837.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

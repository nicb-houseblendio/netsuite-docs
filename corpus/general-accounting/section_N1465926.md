---
id: "section_N1465926"
type: "section"
title: "Bank Transaction GL Impact"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > General Ledger Impact of Transactions > Bank Transaction GL Impact"
parent: "chapter_N1459499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1465926.html"
anchors: ["bridgehead_N1465946", "bridgehead_N1466118", "bridgehead_N1466141", "bridgehead_N1466756", "bridgehead_N1468283"]
sha256: "59be065fd3f91d4a3d45fa244bd29c854b177cdd3649b0b3aee8d0e475610991"
---

You must regularly examine your bank account balances. Account balances are determined by bank transactions that affect these accounts such as deposits you make and checks that you write.

## Bank Deposits {#bridgehead_N1465946}

When you make a deposit with your bank, the deposit increases the total amount of money in a bank account. For example, you have checks from customers that paid invoices this week. The total of all the checks is $2,500. When you take the checks to the bank and deposit them into your checking account, record the $2,500 deposit in NetSuite to track the balance in your checking account.

When you record the deposit, the payment posts to the journal accounts affected by the deposit. Recording a deposit increases the total amount of money you have in your Checking account. The deposit also decreases the total amount of money due to be deposited in your bank account. The deposit posts a $2,500 decrease in the Undeposited Funds account.

These journal lines are posted by the deposit:

| Account | Debit | Credit |
| --- | --- | --- |
| Checking Account | $2,500 |  |
| Undeposited Funds |  | $2,500 |

Record bank deposits at _Transactions > Bank > Make Deposits_.

## Recording Deposits from Transactions {#bridgehead_N1466118}

When entering customer payments, customer deposits, or cash sales, you can specify that the transaction amount directly post into a bank account instead of into your Undeposited Funds account. NetSuite doesn't track each deposit made into a bank account when you choose to directly post transactions.

To set the account to which a transaction posts, click the Account button and select a bank account in the list. After you save the transaction, NetSuite remembers the account you selected the next time you open that type of form.

## Recording Deposits on Payment Method Records {#bridgehead_N1466141}

You can set the account to which payments post based on the type of payment method used. For example, you can set all payments made by credit card to automatically records funds deposited in your checking account.

To set an account to deposit to on payment method records, go to _Setup > Accounting > Accounting Lists_ and click Edit next to the payment method. On the payment method record, click Deposit To and select an account into which the funds should be deposited. Click Save. Now when you select the payment method on a transaction, the funds deposit to the account you indicated.

To create a new payment method record, go to _Setup > Accounting > Accounting Lists > New_ and then click Payment Method.

## Writing Checks {#bridgehead_N1466756}

When you spend money by writing a check, recording the check in NetSuite shows how much money you spent by decreasing the total amount of money in a bank account. If you record expenses on the check, the check shows how you spent the money.

Note:

There is an important difference between entering checks and entering other transactions. Many transactions default to automatically post into certain ledger accounts. When you write a check, however, you choose the journal account affected by the payment and the check amount posts into that account.

For example, you pay $30 to buy a case of paper for the printer in your office. When you write the check, you record how much you spend and why the money was spent. The check posts a $30 decrease in the total amount of funds in the checking account, and $30 is added to the account to which the expense should be posted such as the Office Expense account.

These journal lines are posted by the payment:

| Account | Debit | Credit |
| --- | --- | --- |
| Office Expense | $30 |  |
| Checking Account |  | $30 |

Checks you write can post to more than one expense account, if needed. For example, each month you write a check to your phone company for monthly expenses. Your monthly phone bill shows charges for land-line phones in your office as well as cell phones and pagers your employees use. This month your office phone charges are $175, cell phone charges are $300, and pager charges are $50. Your total bill from the phone company is $525. Because you previously set up expense accounts to track each type of phone expense, you can enter the exact amount for each expense when you write the check.

These journal lines are posted by the check:

| Account | Debit | Credit |
| --- | --- | --- |
| Telephone: Office | $175 |  |
| Telephone: Cell | $300 |  |
| Telephone: Pager | $50 |  |
| Checking Account |  | $525 |

Note:

To keep your accounts in balance, the total amount of the debit lines must be equal to the credit amount to save the check and post the entries.

Write checks at _Transactions > Bank > Write Checks_.

## Entering Checks to Record Non-Check Debits {#bridgehead_N1468283}

You can enter a check to record other purchase methods that decrease funds from bank accounts. For example, you can enter a check to track cash purchases, debit card transactions, ATM (automated teller machine) transactions, and EFT (electronic funds transfer) payments.

To record non-check debits, go to _Transactions > Bank > Write Checks_. Enter the payee and the amount you spent. Verify the account you're debiting. In the Check # field, enter CASH, ATM, DEBIT or EFT to identify the transaction. On the Expenses and Items subtabs, enter line items for the expenses or items associated with this cash transaction. Click Save.

### Additional Topics

-   [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html)

### Related Topics

-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [GL Impact Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481077.html)
-   [Sales Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459773.html)
-   [Customer Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html)
-   [Vendor/Purchase Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1461991.html)
-   [Cost of Goods Sold (COGS) GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1464868.html)
-   [General Ledger Tracking in Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556628.html)
-   [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

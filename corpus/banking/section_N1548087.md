---
id: "section_N1548087"
type: "section"
title: "Transferring Funds Between Bank Accounts"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Transferring Funds > Transferring Funds Between Bank Accounts"
parent: "chapter_N1547981"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548087.html"
anchors: ["procedure_N1548113"]
sha256: "1fcbd70e921b8804b2be31b167dac475a7f6e68c960b37d0b0b17fc34b6d5c0a"
---

NetSuite lets you make two types of bank transfers. You can transfer funds between two bank accounts with the same currency, or from a base currency account to a foreign currency account.

Note:

You can only transfer funds between bank accounts in the same subsidiary.

-   **Two bank accounts with shared currency** - Transfer funds between two bank accounts that share a currency. The exchange rate is always one. The G/L impact is in the subsidiary's base currency. NetSuite translates the transfer amount to the base currency using the default system rate. For example, if you transfer 100 euros between Australian euro accounts with AUD as the base currency, NetSuite still converts the amount using the system rate.
    
    Note:
    
    The default system rate is not visible on the user interface.
    
-   **Base currency bank account to foreign currency bank account** - Transfer funds from a base currency bank account to any foreign currency bank account. The exchange rate is between the subsidiary's base currency and the selected foreign currency. When you select the From and To accounts, NetSuite displays the default system exchange rate between the two currencies.
    
    When you enter a value in the From Amount field, NetSuite translates it and displays it in the To Amount field without rounding.
    
    NetSuite updates the exchange rate if:
    
    -   The translated From Amount field value multiplied by the exchange rate does not equal the To Amount field value after rounding.
        
    -   You change the translated value in the From Amount field.
        
    
    For example, if you transfer 100 USD from a U.S. bank account to a U.K. bank account in GBP, NetSuite displays the default exchange rate (1.6). Entering 100 in the From Amount field displays 62.50 in the To Amount field. If you enter 130 in the To Amount field, NetSuite updates the exchange rate to 0.7692307692307693 (100/130). The G/L impact is in base currency, USD 100.
    

Important:

If the bank account currencies differ, one account must be in the base currency.

#### To enter a funds transfer: {#procedure_N1548113}

1.  Go to _Transactions > Bank > Transfer Funds_.
    
2.  In the **From Account** field, select the source account containing the funds you want to transfer.
    
    The account balance and currency appear next to the **From Account** field.
    
3.  In the **To Account** field, select the target account to receive the funds.
    
    The account balance and currency appear next to the **To Account** field. The exchange rate between the two account currencies displays below.
    
4.  Select the posting period for the transfer.
    
    The period must be open.
    
5.  Accept or select the date in the **Date** field.
    
6.  In the top **Amount** field, enter the amount to transfer from the **From Account**, in that account's currency.
    
    The second **Amount** field displays the amount to be transferred into the **To Account**, after currency translation.
    
7.  Enter a memo if needed.
    
8.  Enter a department, class, or location if needed.
    
9.  Click **Save**.
    

The transfer is complete, and the bank account balances update automatically.

### Related Topics

-   [Transferring Funds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1547981.html)
-   [Deleting Funds Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159441881294.html)
-   [Transferring Funds to Non-Bank Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548225.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

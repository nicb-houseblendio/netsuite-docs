---
id: "chapter_N1550803"
type: "chapter"
title: "Bank Data Import"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Bank Data Import"
parent: "preface_4289362044"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1550803.html"
anchors: []
sha256: "bfcbb5059bf2af33b7bdc338cb43ad8b1d6fca3bb1487e01bff66f421be47328"
---

-   Bank or credit card data for reconciliation and matching
    
-   Corporate card expense data for expense reporting
    

You can set up automatic or manual imports in either case.

-   **Automatic import** - If you have the Administrator role, you can use the Format Profile page to set up daily automatic imports. For more information, see [Automatic Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157895109986.html).
    
-   **Manual import** - Download the financial statement file from your financial institution, and then import it into NetSuite from the Upload File page. You can import a file using the parser and configuration settings from an existing format profile. If you're importing data for reconciliation, you can also use NetSuite's default parser functionality. See [Manual Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157895093957.html).
    

If your role has the Import Online Banking File permission, you can use the Statement File Import feature. For details, see [Permissions for Banking Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156289552348.html).

The data source determines the number of transactions you can import. However, unless you're using the Bank Feeds SuiteApp or AMEX Corporate Card Integration SuiteApp, you should not exceed 10,000 transactions per import.

When importing data for bank or credit card reconciliation, the data source also determines the number of financial institution accounts you can link in a format profile. When configuring an automatic import without using the Bank Feeds SuiteApp, you should try to link no more than 500 accounts. For a manual import, you should not link more than 2,500 accounts.

Note:

There is no suggested limit on the number of employee accounts you can link when importing corporate card expense data for expense reporting.

If an import is going to exceed these suggested limits, you need to create multiple format profiles to make parallel imports easier. Otherwise, you may start to notice performance issues.

The number of the following can affect import performance for bank or credit card reconciliation:

-   General ledger accounts
    
-   General ledger transactions
    
-   Active reconciliation rules
    

To learn how many banking transactions you can import and how many accounts you can link with the Bank Feeds SuiteApp, see [Bank Feeds SuiteApp Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158436030865.html).

To see how many American Express corporate card transactions you can import with the AMEX Credit Card Integration SuiteApp,see [American Express Integration for Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159122395131.html).

When you import data for bank or credit card reconciliation, NetSuite uses reconciliation rules to automatically match your imported bank lines to account transactions. All imported bank lines that can't be matched by the system are available for manual matching on the Match Bank Data page. You can reconcile matched transactions on the Reconcile Account Statement page. For more information, see [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html).

Note:

All imported bank lines with a positive amount also appear and can be processed on the Automated Cash Application page. With the Automated Cash Application feature, you can automatically generate a batch of customer payments in NetSuite and apply them to open invoices. The system then automatically matches and clears the generated customer payments. For details, see [Automated Cash Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2164712765.html).

When you import corporate card charges for expense reporting, NetSuite stores them in the Imported Employee Expenses list. Add your imported charges to expense reports. For more information, see [Creating Expense Reports With Imported Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_159502517274.html).

This section includes the following topics:

-   [Automatic Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157895109986.html)
    
-   [Manual Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157895093957.html)
    
-   [Bank Import Error Codes (Reference)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0106063237.html)
    
-   [Viewing Imported Banking Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494957464.html)
    
-   [Deleting Imported Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3747858087.html)
    

### Related Topics

-   [Permissions for Banking Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156289552348.html)
-   [Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1542225.html)
-   [Checking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1543613.html)
-   [Transferring Funds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1547981.html)
-   [Company Credit Cards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1548363.html)
-   [Financial Institution Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538509582.html)
-   [Automated Cash Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2164712765.html)
-   [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html)
-   [Bank Account Reconciliation and Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1552053.html)
-   [Bank Feeds SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158079179132.html)
-   [Auto Bank Statement Import SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159296303155.html)
-   [Bank Statement Parsers SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1566294502.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

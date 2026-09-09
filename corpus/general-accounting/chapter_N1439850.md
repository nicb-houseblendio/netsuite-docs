---
id: "chapter_N1439850"
type: "chapter"
title: "Chart of Accounts Management"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Chart of Accounts Management"
parent: "preface_3710627041"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html"
anchors: []
sha256: "b2fd6e01bb299936e9e831f4d3cc94a9644ab27c857a3e495ed0ab5c0dca72db"
---

One of the first tasks you must complete before you can begin managing accounting in NetSuite is to set up a chart of accounts (COA). You can use the CSV Import Assistant to import account information from another system, or you can manually create account records in NetSuite. Your chart of accounts provides a set of destinations for posting transactions, and categorizes these transactions for tracking and reporting purposes.

If you use NetSuite OneWorld and have an administrator role or have the Set Up Company permission, you can set up accounting contexts at _Setup > Company > General Preferences._. An accounting context can be a one-to-one relationship between a country's local GAAP (Generally Accepted Accounting Principles) reporting requirements and a statutory chart of accounts (COA). It can also be a unique relationship that meets your company's specific needs. Accounting contexts are useful when users prefer to work in a local GAAP context, rather than in the consolidated context with one centralized COA. Accounting contexts are also useful if you have Multi-Book Accounting provisioned in your account. You can set an accounting context specific for your secondary book and use it for your secondary book reports. For more information, see [Accounting Contexts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4640155582.html). When one accounting context exists, users can select their preferred accounting context at _Home > Set Preferences_. When users select an accounting context, all transactions including system-generated transactions post to the defined COA account name and number. For information about user preferences, see [General Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N475661.html).

If Multi-Book Accounting is provisioned in your account, you can create accounts for specific secondary accounting books. Secondary accounting book specific accounts are filtered for your view when you make book specific secondary book transactions. Accounts that are not available in the primary accounting book don't appear at book generic transactions. For information about book generic and book specific transactions, see [Book-Generic and Book-Specific Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3862676046.html).

Account types are used to organize data in account registers and other financial reports.

-   Income statement account types include Cost of Goods Sold, Expense, Income, Other Expense, and Other Income.
    
-   Balance sheet account types include Accounts Payable, Accounts Receivable, Bank, Credit Card, Deferred Expense, Deferred Revenue, Equity, Fixed Asset, Long Term Liability, Other Asset, Other Current Asset, Other Current Liability, and Unbilled Receivable.
    
-   Cash flow statement account types include the net of Income and Other Income, Accounts Payable, Accounts Receivable, Equity, Fixed Asset, Long Term Liability, Other Asset, Other Current Asset, Other Current Liability, and Unbilled Receivable.
    
-   Statistical accounts, part of the Advanced Financial module, enable your financial team to track non-monetary data and then use that information in reports and income statements. Financial users can examine the non-monetary data to view its relationship with the financial activity of your organization. For more information, see [Using Statistical Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3841945149.html).
    

Note:

When you enable some accounting features, the system automatically generates an account specific to those features. If your chart of accounts already contains an account by the same name as that of a system-generated account created through feature enablement, the system-generated account name is appended with '(system)' and the default account type is selected. For example, you have created an A/R account type named Unbilled Receivable. You enable the Advanced Revenue Management feature. The system automatically generates the Unbilled Receivable (System) account under the account type Unbilled Receivable and uses this system account for unbilled receivable reclassification. For a list of feature-specific, system-generated accounts, see [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html).

You can create a hierarchy of accounts within each account type by defining subaccount relationships on account records. Careful attention to account typing, naming, and numbering when you set up your chart of accounts results in more useful reports. In addition, organize your account hierarchies, naming, and numbering to simplify the future addition of new accounts.

NetSuite enables you to create an account record solely for reporting purposes. These accounts are called summary accounts and are useful when you want to create a non-posting, inactive parent account that has active child accounts. New summary accounts that are not in NetSuite OneWorld can't have an opening balance, but you can convert an existing account with a transaction balance into a summary account. In this case, you can't post additional transactions to the account. Summary accounts appear with their children in the chart of accounts list. You can't merge a summary account into another account.

For financial statements such as income statements (profit and loss statements) and balance sheets, you can also use account names or numbers to further customize your data presentation.

Important:

If you want to use numbers as well as names to identify accounts, enable the related accounting preference in your account at _Setup > Accounting > Accounting Preferences_. For more information, see [Chart of Account Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440268.html).

#### To set up your chart of accounts, complete the following steps.

1.  Create NetSuite account records.
    
    Note:
    
    Your user role must have both ADMI\_ACCOUNTING and LIST\_ACCOUNT permissions to access _Setup > Accounting > Manage G/L > Chart of Accounts_.
    
    -   Import account information from another system. See:
        
        -   [Chart of Accounts Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N357847.html)
            
        -   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
            
    -   Create new accounts manually in NetSuite. See [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).
        
    
    You can enter opening balances for new accounts as needed. For more information, see [Entering Opening Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1441761.html).
    
2.  Review the Chart of Accounts.
    
    After you create account records, they appear in the Chart of Accounts list. Any new accounts you create later also appear in the list automatically. For more information, see [Viewing the Chart of Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442506.html).
    
    After you set up your chart of accounts, you can make changes as needed. For more information, see [Making Changes to Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442743.html).
    
    Note:
    
    In NetSuite Japan edition, the system automatically adds default Japanese accounts to your chart of accounts upon creation of a Japanese subsidiary in NetSuite OneWorld. The Japanese accounts are based on the Japanese Industrial Standard (JIS) X 0406:1984.
    

For information about financial tracking and reporting, see the following help topics:

-   [Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1508800.html)
    
-   [Accounting-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1519116.html)
    
-   [Financial Statements Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html)
    

### Related Topics

-   [Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3947502870.html)
-   [Setting Up Historical Balances in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442160.html)
-   [NetSuite Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1379709.html)
-   [Accounting Features and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1383640.html)
-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html)
-   [Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1508800.html)
-   [Accounting-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1519116.html)
-   [Sequential Liability SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158408768320.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

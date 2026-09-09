---
id: "chapter_N1395057"
type: "chapter"
title: "Currency Management"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management"
parent: "preface_3710627041"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html"
anchors: []
sha256: "53fbfbce3704ec8ed88812ff6d4e2191c0fb26cab58b23988aed8d15099a7289"
---

If you use the same currency for all of your business transactions, you set the Currency Locale during setup on your Company Information page. These topics about currency management don't apply to your account. For more about the Company Information page, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).

If your business uses more than one currency, you can enable the Multiple Currencies feature. This feature provides support for transactions with customers and vendors that use currencies other than your primary currency. You should review this topic and others in this section before you enable the feature. You can't disable the feature after you create transactions and records that rely upon it.

If you conduct business in foreign currencies and foreign countries, you may need to follow the accounting principles and reporting requirements of other countries. Your accountants or auditors should know these principles and requirements, and you should seek their advice. If you use non-compliant accounting practices, over time, it could materially affect the valuation of transactions and account balances originally recorded in foreign currencies.

Your company's primary currency, its functional currency, is called the **base currency** in NetSuite. Subsidiaries in NetSuite OneWorld can have different base currencies from the parent subsidiary and from each other. The currencies used in transactions with customers and vendors, other than the base currency, are referred to as **foreign currencies** or **transaction currencies**.

After you enable the **Multiple Currencies** feature, complete the additional setup covered in [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html) and its subtopics, as follows:

-   Create currency records for the different currencies you want to use in your transactions and for your subsidiaries if you use NetSuite OneWorld. See [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html).
    
-   Select the base currency for your company. If you use NetSuite OneWorld, you select the base currency for each subsidiary. If you also use the Multi-Book Accounting feature, you select the base currency for each subsidiary and accounting book combination. See [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html).
    
-   Assign currencies to customers, vendors, and other entities. For NetSuite OneWorld, you assign subsidiaries to the entities, and the currency is assigned with the subsidiary. See [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).
    

For the next part of your setup, you need to establish the **currency exchange rates** to apply to transactions in your account. The Currency Exchange Rates list includes the exchange rates between each base currency and its foreign currencies. You can set and update exchange rates manually or automatically using the Currency Exchange Rate Integration feature. For instructions, see [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html) and its subtopics.

If you have subsidiaries with different base currencies, NetSuite maintains a list of **consolidated exchange rates** in addition to the Currency Exchange Rates list. NetSuite uses the rates in the Consolidated Exchange Rates list for reporting purposes. Consolidated exchange rates translate between the base currency of a subsidiary and its parent or grandparent subsidiary for each accounting period. You should update these rates before you close each period. For details and instructions, see [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html) and its subtopics.

Changes in exchange rates between your base currency and the foreign currencies used in transactions cause a corresponding change in the transactions' base currency valuations. These changes in base currency valuations (**foreign currency revaluation**) impact the general ledger. NetSuite automatically revalues transactions that close during each accounting period and posts the variance to the realized gain/loss account. The month-end revaluation process posts variances open transactions, foreign-currency accounts, and non-denominated accounts to the unrealized gain/loss account. With the Foreign Currency Variance Mapping feature, you can map foreign currency variances to other accounts according to rules you create.

For details and instructions, see [Foreign Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409370.html) and its subtopics.

### Related Topics

-   [NetSuite Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1379709.html)
-   [Accounting Features and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1383640.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)
-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1523373090.html)
-   [Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1508800.html)
-   [Accounting-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1519116.html)
-   [Sequential Liability SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158408768320.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1383904"
type: "section"
title: "Accounting-Related Features"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Features and Preferences > Accounting-Related Features"
parent: "chapter_N1383640"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1383904.html"
anchors: ["bridgehead_N1384034", "bridgehead_N1384440", "bridgehead_N1384702"]
sha256: "a2bc68cb2758fab5ec2ee5eba43d0aad9312381619562cdc8500e599ac3adf64"
---

The records and transactions you can use in your NetSuite account depend on the accounting features you've enabled. You can enable or disable features at _Setup > Company > Enable Features_ if you're are an account administrator or have the Enable Features permission. After you've enabled features, you can set up related records needed to manage accounting in NetSuite. For details about all of the features on the Enable Features page, see [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html).

SuiteGL features let you customize general ledger processes to meet your specific business needs. With these features, you can change line-level general ledger impact of transactions, set up custom transaction types with unique general ledger capabilities, and create customized classifications to improve reporting and analytics. For details, see [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html).

The next sections cover accounting-related features that aren't listed on the Accounting subtab on the Enable Features page. Each section is named after the subtab where the feature appears on Enable Features page. For more details about accounting features, see [Accounting Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N233872.html).

-   [Company](#bridgehead_N1384034)
    
-   [Transactions](#bridgehead_N1384440)
    
-   [Employees](#bridgehead_N1384702)
    

## Company {#bridgehead_N1384034}

The following accounting-related features are available on the Company subtab of the Enable Features page.

| **Field** | **Description** |
| --- | --- |
| Multiple Currencies | Lets you use foreign currencies for sales and purchase transactions, and handles exchange rate fluctuations. This feature also lets you work with both customers and vendors who use multiple currencies in doing business with you. After qualifying revaluation transactions, NetSuite generates the Realized Gain/Loss, Unrealized Gain/Loss, Unrealized Matching Gain/Loss, Rounding Gain/Loss accounts. Depending on the year when your NetSuite account was set up, you may also have the Exchange Rate Variance account. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) for details. |
| Currency Exchange Rate Integration | Automatically updates currency exchange rates from your chosen provider one time a day. When you enable this feature, you must agree to the Notice that appears. NetSuite stores the user ID and time stamp of account changes in system notes. To choose an exchange rate provider, how to obtain exchange rates, and anchor currencies, go to _Setup > Accounting > Preferences > Accounting Preferences_ > General subtab > Exchange Rate Integration. For more information, see [Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html#bridgehead_4314469559) and [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html). |

## Transactions {#bridgehead_N1384440}

The following accounting-related features are available on the Transactions subtab of the Enable Features page.

Many of these features create system-generated accounts when you enable them. These accounts are listed in the descriptions. For a full list of system-generated accounts, see [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html).

| **Field** | **Description** |
| --- | --- |
| Sales Orders | Lets you track customer orders and convert them into invoices and cash sales. When you enable this feature, NetSuite creates the Sales Orders account. See [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html) for details. |
| Return Authorizations | Lets you track customer returns. When you enable this feature, NetSuite creates the Return Authorizations account. See [Customer Return Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302852.html) for details. |
| Purchase Orders | Lets you track orders to vendors. When you enable this feature, NetSuite creates the Purchase Orders account. See [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html) for details. |
| Vendor Return Authorizations | Lets you track returns to vendors. When you enable this feature, NetSuite creates the Vendor Return Authorizations and Purchases Returned Not Credited accounts. See [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html) for details. |
| Advanced Billing | Lets you invoice sales over time or by contract term, based on defined schedules. See [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html) for details. |
| Credit Card Payments | Lets you accept customer credit card payments. When you enable this feature and Customer Access, NetSuite creates the Unapproved Customer Payments account. See [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html) for details. |
| PayPal Integration | Lets you accept PayPal payments from Web store customers. See [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html) for details. |

## Employees {#bridgehead_N1384702}

The following accounting features are available on the Employees subtab of the Enable Features page.

Most of these features create system-generated accounts when you enable them. These accounts are listed in the descriptions. For a full list of system-generated accounts, see [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html).

| **Field** | **Description** |
| --- | --- |
| Payroll | Lets you process payroll and print paychecks. When you enable this feature, NetSuite creates the Payroll Adjustments account. See [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html) for details. |
| Paycheck Journal | Lets you integrate NetSuite with external payroll systems, create custom payroll solutions with SuiteScript and SOAP web services, and track employees' payroll data in NetSuite. See [Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N969418.html) for details. |
| Direct Deposit | Lets you authorize of electronic funds transfers from your accounts to employees' accounts. When you enable this feature, NetSuite creates the Failed ACH Transactions account. See [About Direct Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N945815.html#chapter_N956015) for details. |
| Expense Reports | Lets you track and bill employee expenses. When you enable this feature, NetSuite creates the Unapproved Expense Reports, Advances Paid, and Accounts Payable accounts. See [Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907845.html) for details. |
| Purchase Requests | Lets you use purchase requests to add an approval process for purchase orders. See [Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2393987.html) for details. |
| Employee Commissions | Lets you automate employee compensation processes. When you enable this feature, NetSuite creates the Commissions Payable account. See [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html) for details. |

### Related Topics:

-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html)
-   [Setting Up Accounting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391837.html)
-   [Setting Up Employee Related Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1394576.html)
-   [Accounting Features and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1383640.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

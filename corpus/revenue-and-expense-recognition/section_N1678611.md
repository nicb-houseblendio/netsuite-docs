---
id: "section_N1678611"
type: "section"
title: "Enabling the Revenue Recognition Feature"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Setting Up the Revenue Recognition Feature > Enabling the Revenue Recognition Feature"
parent: "section_N1678353"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678611.html"
anchors: ["procedure_N1678635"]
sha256: "4f3d25824ca550355dc827cd8e0a0aeb63554cc4df09a1211ea4323dd0c9b33b"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For the equivalent information for Advanced Revenue Management (Essentials), see [Enabling the Advanced Revenue Management (Essentials) Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4331936670.html).

To use the Revenue Recognition feature, the Accounting Periods feature must be enabled because accounting periods are used for revenue recognition schedules. Accounting periods must be set up for the complete range of time covered by your revenue recognition schedules. Also, revenue recognition requires one or more deferred revenue accounts.

#### To enable Revenue Recognition: {#procedure_N1678635}

1.  Go to _Setup > Company > Setup Tasks > Enable Features (Administrator)_.
    
2.  Click the **Accounting** subtab, ensure the **Accounting Periods**, **Revenue Recognition**, and any other desired revenue feature boxes are checked.
    
3.  Click **Save**.
    
4.  Ensure that one or more Deferred Revenue accounts are set up as needed.
    
    NetSuite automatically adds a default account with a type of Deferred Revenue to the Chart of Accounts because at least one account of this type is required for the feature. You can create additional Deferred Revenue type accounts as needed. For each item that requires revenue recognition, you designate a Deferred Revenue type account where revenue is posted according to the generated schedule.
    
    To view the automatically created account or to create additional accounts, go to _Lists > Accounting > Chart of Accounts_.
    
5.  Go to _Setup > Accounting > Manage Accounting Periods_, and ensure that accounting periods are set up for the range of time your revenue recognition schedules covers.
    
    For example, if you're going to create schedules that extend 3 years ahead, you need to set up accounting periods through that time.
    

### Related Topics

-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Setting Revenue Recognition Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678834.html)
-   [Enabling Auto-Numbered Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679074.html)
-   [Defining Expense Categories for Billable Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679290.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)
-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

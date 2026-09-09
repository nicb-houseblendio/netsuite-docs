---
id: "section_N1766842"
type: "section"
title: "Enabling the Amortization Feature"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Setup for Amortization > Enabling the Amortization Feature"
parent: "section_N1766651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766842.html"
anchors: ["procedure_N1766870"]
sha256: "fad97554e30ad09f82d10e0945a94443eb0106bffd20def41f0b63467258bbac"
---

To use the Amortization feature, the Accounting Periods feature must be enabled because accounting periods are used for amortization schedules. Accounting periods must be set up for the complete range of time covered by your amortization schedules. In addition, amortization requires one ore more deferred expense accounts.

The Amortization feature also may be used in conjunction with the Revenue Recognition feature and other revenue features.

#### To enable amortization: {#procedure_N1766870}

1.  Go to _Setup > Company > Setup Tasks > Enable Features (Administrator)_.
    
2.  Click the **Accounting** subtab, ensure the **Accounting Periods**, **Amortization**, and any other desired feature boxes are checked, and click **Save**.
    
3.  Ensure that one or more deferred expense accounts are set up as needed.
    
    NetSuite automatically adds a default account with a type of Deferred Expense to the Chart of Accounts because at least one account of this type is required for the feature. You can create additional Deferred Expense type accounts as needed. For each item that requires amortization, you designate a Deferred Expense type account where expenses are posted according to the generated schedule.
    
    To view the automatically created account or to create additional accounts, go to _Lists > Accounting > Chart of Accounts_.
    
4.  Ensure that accounting periods are set up for the range of time your amortization schedules will cover, at _Setup > Accounting > Manage Accounting Periods_.
    
    For example, if you're going to create schedules that extend three years ahead, you need to set up accounting periods through that time
    

### Related Topics

-   [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html)
-   [Setting Amortization Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767069.html)
-   [Enabling Auto-Numbered Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767306.html)
-   [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

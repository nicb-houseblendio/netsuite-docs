---
id: "section_N1812226"
type: "section"
title: "Tax Control Accounts Overview"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Control Accounts Overview"
parent: "chapter_N1805198"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html"
anchors: []
sha256: "c6de84e6205c6ee3f3ae7f2d6935671972540f39e295b17215b30ea1a699ab46"
---

Tax control accounts are accounts in your general ledger or chart of accounts. These are where amounts for indirect taxes such as sales tax and VAT are posted.

Tax control accounts are used to define tax types, and tax types are used to define tax codes. Tax codes in your transaction records determine how much tax is applied to each line item on your transactions.

If the Advanced Taxes feature is enabled in your NetSuite account, tax control accounts are linked to a nexus or country to more effectively manage tax postings.

In NetSuite, the tax control accounts are either set up by default, or set up for you by Professional Services. An administrator can create new tax control accounts if needed.

You can use multiple tax control accounts to track your sales tax liability and add more detail to your financial statements. For example, for US customers, you can create tax control accounts for each tax jurisdiction and assign them to their respective tax codes.

You can choose to separate your sales VAT and purchase VAT. For example, for UK customers, you can use an Output VAT account to track VAT for sales, and an Input VAT account to track VAT you can reclaim.

Some users prefer to see the total balance due at any time. In this case, use a single account to consolidate all your VAT or GST entries.

Examples of tax control accounts are shown in the related topic, [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).

To create a tax control account, see [Creating a Tax Control Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812423.html).

To remove restrictions for tax control accounts on tax types, see [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html).

Warning:

If you inactivate a tax control account, you won't be able to select the tax codes associated with it when you create or edit transactions. Any default tax codes linked to it will also be invalid. Be sure to update default tax codes on all affected records such as:

-   Nexuses
    
-   Item records
    
-   Customer records
    
-   Vendor records
    

You can also reactivate the tax control account to make the tax codes available again.

### Related Topics

-   [Creating a Tax Control Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812423.html)
-   [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

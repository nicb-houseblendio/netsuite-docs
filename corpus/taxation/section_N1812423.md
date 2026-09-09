---
id: "section_N1812423"
type: "section"
title: "Creating a Tax Control Account"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Control Accounts Overview > Creating a Tax Control Account"
parent: "section_N1812226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812423.html"
anchors: ["procedure_N1812432"]
sha256: "92e62c5956da52c442b0d9b203c93087ad126d8d1866dfdc21c593db64c556b6"
---

Note:

Tax types and tax codes are created separately. Changing the tax control account on the tax type record doesn't automatically update the tax control account shown on the tax code record. Transactions post tax to the tax control account shown on the tax code record. Editing the tax code record updates the tax control account fields.

#### To create a tax control account: {#procedure_N1812432}

1.  Go to _Setup > Accounting > Taxes > Tax Control Accounts_.
    
2.  If you're using NetSuite OneWorld, select a nexus.
    
3.  Enter the name of the tax control account.
    
4.  Enter a description for the tax control account.
    
5.  Click **Save**.
    

After you create a tax control account, you can select it on tax type and tax code records in the Tax Account field. Tax liability for the tax code is applied to the tax control account selected on the item record.

You can view the tax liability for each tax control account on your balance sheet and other financial reports.

Warning:

If you inactivate a tax control account, you won't be able to select the tax codes associated with it when you create or edit transactions. Any default tax codes linked to it will also be invalid. Be sure to update default tax codes on all affected records such as:

-   Nexuses
    
-   Item records
    
-   Customer records
    
-   Vendor records
    

You can also reactivate the tax control account to make the tax codes available again. For information about how to delete accounts and how to make accounts inactive, see [Deleting Accounts and Making Accounts Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1444958.html)

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

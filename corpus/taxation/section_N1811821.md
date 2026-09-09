---
id: "section_N1811821"
type: "section"
title: "Creating a Tax Type"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Types Overview > Creating a Tax Type"
parent: "section_N1810558"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1811821.html"
anchors: ["procedure_N1811845"]
sha256: "8f26a4413603b2d2b4bea3cc2192175a06c31972b0f629a1fe1fef75b5748d92"
---

By default, tax types use tax control accounts for posting tax amounts. You can remove this restriction if you'd rather use another account from your chart of accounts as your posting account for tax. For more information, see [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html).

#### To create a tax type: {#procedure_N1811845}

1.  Go to _Setup > Accounting > Taxes > Tax Types_.
    
2.  If you're using NetSuite OneWorld, select the country from the Tax Types page.
    
3.  On the New Tax Type page, enter a name or abbreviation for this tax type.
    
4.  Enter a description for this tax type.
    
5.  Check the **OSS** box if this tax type is for tracking VAT on B2C digital services based on the customer's country. The OSS tax type is tracked separately from normal VAT.
    
    Note:
    
    The OSS box only shows if you've enabled the EU One Stop Shop feature in your account. For more information, see [EU One Stop Shop (OSS)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4163851800.html).
    
6.  In the **Liability/Sales Tax Account** field, select the tax control account where NetSuite posts tax collected on sales.
    
7.  In the **Asset/Purchase Tax Account** field, select the tax control account where NetSuite posts tax on purchase transactions.
    
    Note:
    
    For US, there's no asset/purchase tax account.
    
8.  Click **Save**. When you apply a tax code of this type to a transaction, NetSuite posts the tax to the proper tax control account.
    

Important:

Tax types and tax codes are created separately. Transactions post tax to the tax control account shown on the tax code record. If you change the tax control account on the tax type, it doesn't automatically update the tax control account on the tax code. You need to also edit and save any tax code records that share that tax type.

### Related Topics

-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

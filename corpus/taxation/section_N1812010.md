---
id: "section_N1812010"
type: "section"
title: "Removing Restrictions for Tax Control Accounts"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Types Overview > Removing Restrictions for Tax Control Accounts"
parent: "section_N1810558"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html"
anchors: ["procedure_N1812050"]
sha256: "9dff6930479680d3361f8b4fc0bf7701ea08351568ef0ae404fc71b5ec633bc4"
---

Note:

This feature is available for all nexuses, except US and Canada.

In certain countries, companies are required to record tax as an expense. For example, in Brazil, inventory transfers are taxable, and because the calculated tax isn't recoverable, the tax has to be treated as a business expense. In other countries, companies are required to use income accounts initially when posting taxes. For example, under the European travel industry's margin scheme, VAT on purchases is treated as part of cost of goods sold, and tracked separately on the income statement.

On the Set Up Taxes page for a nexus, the **Only Use Tax Control Accounts on Tax Types** preference is enabled by default. If you turn off this preference, you can create a tax type record and use any account from your chart of accounts as your posting account for tax. Note that you can't use the same account for both sales and purchases. After setting up the tax type, you must select it on the appropriate tax code records. To turn this preference back on, make sure no tax types are linked to regular accounts.

Tax amounts posted to income or expense accounts are shown on the general ledger, balance sheet, and income statement reports. If you want to use the Pay Tax Liability feature in NetSuite, you'll need to manually move this tax from the income or expense account to the tax liability account.

#### To remove restrictions for tax control accounts: {#procedure_N1812050}

1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
    1.  Click the subtab of the country nexus.
        
    2.  On the Set Up Taxes page, clear the **Only Use Tax Control Accounts on Tax Types** box.
        
    3.  Click **Save**
        
2.  Go to Setup > Accounting > Tax Types > New..
    
    1.  Click the country nexus.
        
    2.  On the Tax Type page, enter a name for the new tax type.
        
    3.  Select the income or expense account from your chart of accounts as your posting account for tax.
        
    4.  Click **Save**
        
3.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
    1.  Click the country nexus.
        
    2.  On the Tax Code page, select the tax type that you created in Step 2.
        
    3.  Enter or select values in required fields to complete the Tax Code record.
        
    4.  Click **Save**.
        
        When this tax code is applied to a transaction, NetSuite posts the tax to the income or expense account defined on the tax type.
        

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

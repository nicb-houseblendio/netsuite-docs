---
id: "section_N1796705"
type: "section"
title: "Setting Default Tax Items on Customer Records"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Enabling and Setting Up Taxation Features > Setting Default Tax Items on Customer Records"
parent: "chapter_N1794679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796705.html"
anchors: ["procedure_N1796728"]
sha256: "862c1ef5236652966a6f1106d64cd28e3fe1c6b8bcf1edee7c5a01c5ee98e60f"
---

After you have set up your tax codes, you can set a default tax code on a customer record.

For example, you can set a default tax code that defines a customer as VAT-exempt or GST-exempt. Charities and nonprofit organizations are usually exempt from tax.

This default tax code will be automatically filled on all transaction forms related to this customer. However, you can override this on the transaction form.

Selecting anything other than the default 'blank' selection will override the tax engine lookup for that customer on transactions and will always use the selected tax code.

Note:

Default tax code is automatically selected on transactions only if the tax code is available in Tax Code dropdown field. Tax codes in dropdown field are filtered based on the transaction nexus.

#### To set tax items on customer records: {#procedure_N1796728}

1.  Go to Lists > Relationships > Customers.
    
2.  Click the Edit link of the customer record, or click **New** to create a new customer.
    
3.  Click the **Financial** subtab.
    
4.  In the **Tax Item** field, select a default tax code for this customer.
    
5.  Click **Save**.
    

Warning:

When you inactivate a tax control account, any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes on the affected customer records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).

### Related Topics

-   [Tax Setup Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795438.html)
-   [Enabling Taxation Features in Accounts Without Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795648.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Tax Rounding Preferences on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4259667651.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

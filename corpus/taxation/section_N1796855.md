---
id: "section_N1796855"
type: "section"
title: "Setting Default Tax Items on Vendor Records"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Enabling and Setting Up Taxation Features > Setting Default Tax Items on Vendor Records"
parent: "chapter_N1794679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796855.html"
anchors: ["procedure_N1796867"]
sha256: "5b730deddbf5464580c55736cb174c90b6359e6fc12da7f5421cefb451918afb"
---

If you use the Australia, Canada, Japan, U.K., or International edition of NetSuite, you can set a default tax code for vendors. This tax code is applied by default on purchase orders and vendor bills.

Note:

If you use NetSuite OneWorld and the vendor is shared with multiple subsidiaries, you can select a tax code that is associated with any of the secondary subsidiaries assigned to the vendor. For more information, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

#### To set a default vendor tax code: {#procedure_N1796867}

1.  Go to Lists > Relationships > Vendors.
    
2.  Click the Edit link of the vendor record, or click **New** to create a vendor if it isn't yet in the system.
    
3.  In non-OneWorld accounts, click the **Financial** subtab.
    
    In OneWorld accounts, click the **Subsidiary** subtab.
    
4.  In the **Tax Code** field, select the tax code you want applied to purchase orders and bills placed for this vendor.
    
5.  Click **Save**.
    

Important:

The default tax code you assign to a vendor must be available on purchase transactions, otherwise you will be unable to select this tax code on purchase orders or bills for that vendor. Make sure that the **Available On** field of the Tax Code record (Setup > Accounting > Tax Codes) is set to **Purchase Transactions** or **Both**.

Warning:

When you inactivate a tax control account, any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes on the affected vendor records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).

### Related Topics

-   [Tax Setup Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795438.html)
-   [Enabling Taxation Features in Accounts Without Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795648.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Setting Tax Rounding Preferences on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4259667651.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

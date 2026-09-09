---
id: "section_N2085546"
type: "section"
title: "Setting Default Withholding Tax Codes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Setting Default Withholding Tax Codes"
parent: "chapter_N2078886"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html"
anchors: ["bridgehead_N2085573", "procedure_N2085586", "bridgehead_N2085632", "procedure_N2085645", "bridgehead_N2085691", "procedure_N2085705"]
sha256: "0c190c485f9b253ba26fea876a2ac9ab9657162c789e9a2d66182652d530b830"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

After setting up your withholding tax preferences, tax types, tax codes, and tax groups, you can associate default withholding tax codes to items, customers, and vendors, so they're selected automatically in transactions.

Warning:

When setting default tax codes on item, customer, and vendor records, keep in mind that if you inactivate a tax control account in the future, any default tax codes linked to it will become invalidated. When this happens, remember to change the default tax codes on the affected item, customer, and vendor records to make sure invalid tax codes aren't used in transactions. Alternatively, you can re-activate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).

## Setting Default Withholding Tax Codes on Item Records {#bridgehead_N2085573}

As a buyer, you can associate a default withholding tax code with an item. In a transaction, NetSuite applies the customer's default withholding tax code if they have one, otherwise, it uses the item's default withholding tax code.

#### To set a default withholding tax code on an item record: {#procedure_N2085586}

1.  Go to Lists > Accounting >Items.
    
2.  Click the **Edit** link of an item record, or click **New** to create an item.
    
3.  Click the **Accounting** subtab.
    
4.  In the **WH Tax Code** field, select the withholding tax code that should apply to this item by default on transactions.
    
5.  Click **Save**.
    

## Setting Default Withholding Tax Codes on Vendor Records {#bridgehead_N2085632}

As a buyer, you can associate a default withholding tax code with a vendor. NetSuite applies the vendor's default withholding tax code on purchase orders and vendor bills.

#### To set a default withholding tax code on a vendor record: {#procedure_N2085645}

1.  Go to Lists > Relationships > Vendors.
    
2.  Click the **Edit** link of the vendor record, or click **New** to create a vendor.
    
3.  Click the **Financial** subtab.
    
4.  In the **WH Tax Code** field, select the withholding tax code that you want to apply by default to purchase orders and bills created for this vendor.
    
5.  Click **Save**.
    

## Setting Default Withholding Tax Codes on Customer Records {#bridgehead_N2085691}

As a seller, you can set a default withholding tax code for a customer, so when you receive payments on open invoices from that customer, the correct withholding tax code is already selected. If a customer doesn't have a default withholding tax code, NetSuite uses the item's default withholding tax code on the transaction.

#### To set a default withholding tax code on a customer record: {#procedure_N2085705}

1.  Go to Lists > Relationships > Customers.
    
2.  Click the **Edit** link of the customer record, or click **New** to create a customer.
    
3.  Click the **Financial** subtab.
    
4.  In the **WH Tax Code** field, select the withholding tax code that you want to apply by default to invoices and cash sales created for this customer.
    
5.  Click **Save**.
    

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

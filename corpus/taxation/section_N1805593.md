---
id: "section_N1805593"
type: "section"
title: "Tax Codes Overview"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Codes Overview"
parent: "chapter_N1805198"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html"
anchors: []
sha256: "844d7c5fd14c1aa44a0c36461616d8bdc5c5230a1596ce7a832eeef644ee7d2c"
---

For most countries, tax codes are set up automatically when you set up your NetSuite account, or add a nexus. Your account administrator can create more tax codes if needed.

If you have the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) installed in your account, when you add a new country nexus, the VAT/GST tax codes for that nexus are automatically provisioned. The SuiteApp only creates tax codes for countries it supports, because those tax codes are used to generate tax reports. For more information, see [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) and [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html).

Review your tax codes to make sure the rates and properties are correct. To view existing tax codes in your NetSuite account, go to _Setup > Accounting > Taxes > Tax Codes_. You can create, edit, inactivate, or delete tax codes.

Tax codes determine how much tax is applied to each line item on your transaction records. A tax code represents the following:

-   a tax that you collect from your customers located in a specific geographic area
    
-   a tax that you pay to a taxing authority on behalf of your customers
    
-   a tax rate for one location, to be paid to one tax authority
    
-   a tax that is applied only to certain types of transactions
    

Tax codes that can be applied to one transaction can be combined in a tax group. For example, for a specific US state, combine city tax and state tax into one tax group. When you create an invoice for a sale in that state, you can then select the tax group. For information, see [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html).

You can associate a tax code with a customer. See [Setting Default Tax Items on Customer Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796705.html).

You can link a tax code to an inventory item and nexus, if each nexus applies a different tax rate for the same item. To do this, you must create a tax schedule. Tax schedules let you assign the right tax codes to an item based on the country or nexus it applies to. For example, graphic design services are taxable in New York, but not Florida. After the tax schedule is created, you can select it on the item record. For information, see [Creating Tax Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804737.html).

If you don't have Advanced Taxes enabled in your account, you can set a default tax code on an item record. If you have Advanced Taxes enabled, you can associate a tax schedule with an item record instead. See [Setting Tax Codes or Tax Schedules on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797005.html).

If you use the UK or International Edition of NetSuite, you can set a default tax code for vendors. See [Setting Default Tax Items on Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796855.html).

If you run a web store, you can select a default tax code to be used for a transaction when NetSuite can't find a predefined tax code in your customer's record or in your inventory item record. To do this, go to _Setup > Accounting > Taxes > Set Up Taxes_. Select a tax code or tax group in the **Default Tax Code** field.

You can still change the tax code on individual transaction records.

For more information, see the Related Topics list.

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html)
-   [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html)
-   [Adding Custom Fields to Tax Code Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807644.html)
-   [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html)
-   [Inactivating or Deleting Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1808226.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)
-   [Creating Tax Codes - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856762.html)
-   [Creating Tax Codes - United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2026362.html)
-   [Creating Tax Codes - Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1834295.html)
-   [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

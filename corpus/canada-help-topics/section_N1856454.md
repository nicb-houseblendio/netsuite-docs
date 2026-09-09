---
id: "section_N1856454"
type: "section"
title: "Setting Tax Preferences for Canada"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Tax Topics For Accounts Without SuiteTax > Setting Tax Preferences for Canada"
parent: "section_156941156434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html"
anchors: []
sha256: "b70fcd4b0ccbdbda2cfb6c8fef15dc9ca6300c3c28a785cdccff3b1250d9b7ed"
---

You can set tax preferences at _Setup > Accounting > Taxes > Set Up Taxes_.

The following preferences are available when configuring tax nexuses in Canada.

-   **Enable Tax Lookup on Sales and Purchases** - This box is checked by default to enable NetSuite to determine appropriate tax codes to use on transaction forms. Clear this box if you don't want NetSuite to determine the correct tax code based on the customer's shipping address. If you use SuiteScript to query third party tax services, clear this box. For more information about the sales tax code lookup for Canada, see [Enabling Canada Tax Lookup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857418.html).
    
-   **Print Tax Code Summary on Sales Forms** - This box is checked by default to include a summary of the taxes paid per tax code on printed transaction forms such as estimates, sales orders, and sales invoices. The tax code summary is shown only if two or more tax codes are used on the transaction. Tax codes with 0% rate are not shown. The tax code summary shows the tax code names. Be sure to name your tax codes as you would like them to appear on printed forms.
    
    Clear this box if you don't want your printed forms to include a summary of taxes per tax code.
    
    If you want to show only one HST tax code line at the bottom of transaction forms, use a customized transaction form so you can edit its tax total label:
    
    1.  Customize a transaction form.
        
    2.  Click the **Printing Fields** subtab.
        
    3.  Click the **Footer** subtab.
        
    4.  Check the **Tax Total** box.
        
    5.  Click **Save**.
        
    
    Make sure you choose your preferred PDF layout for transaction type forms. To set your transaction form PDF layout preferences, go to _Customization > Forms > Transaction Form PDF Layouts_. If the **Preferred** box for **Transaction Layout with Tax Summary** is checked, NetSuite shows the tax summary as a separate element at the bottom of the form, above the totals. If you choose any of the standard or classic transaction type layouts, NetSuite shows the tax summary in the main body of the form as part of the columns element. For more information about transaction form PDF layouts, see [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html).
    
-   **Record PST Separately on Purchases** - Check this box to track Provincial Sales Tax (PST) separately from a purchased item's value. This enables you to report PST assets or liability separately from an item's cost. If this box is checked, the value of PST from the vendor return authorization is tracked on PST on Purchases. Previously, it was tracked on PST Expenses. Clear this box if you want PST to be applied to the value of the items purchased. If this box is clear, then when a purchase order is received, the item's rate on the item receipt includes PST. Subsequently, when the purchase order is billed, the item's rate on the vendor bill is calculated as the rate on the item receipt minus the PST amount on the purchase order. Note that if the item's rate on the item receipt is modified, the amounts on the bill will be incorrect, so they must be modified as well.
    
-   **Tax Code for Out-of-Province Sale** - This tax code is used if the province on a customer's shipping address does not match an existing tax code, or if the customer is exempt from paying Provincial Sales Tax (PST). Select the **CA-GST only** tax code.
    
-   **Tax Code for International Sale** - This tax code is used for orders placed by international customers. Select the CA- **Zero** (zero-rated) tax code.
    
-   **Default Tax Code** - Select a default tax code to use if no tax code has been predefined for the customer or items.
    
    Note:
    
    On purchase transactions, the default tax code value isn't populated in the **Tax Code** field. This occurs when no tax code was previously defined on the vendor record and on the item level.
    
    Important:
    
    The **Default Tax Code** field is mandatory. In a OneWorld account, if you click **Save** and the system prompts you to enter a value for the **Default Tax Code** field, there may be a nexus where a default tax code has not yet been selected. Look for this nexus and provide the missing information, and then click **Save**.
    
    Warning:
    
    When you inactivate a tax control account, any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes on the affected nexuses, item records, customer records, and vendor records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
    
    Note:
    
    Canada specific form does not show per-line tax amounts, as there can be multiple rates (for GST/HST and PST) and therefore multiple tax amounts. Total taxes per tax type are shown in summary.
    
-   **Province, Preferred GST/HST Agency, and Preferred PST Agency** - Select each province's tax agencies from the dropdown.
    

If you have Advanced Taxes enabled in your account, the list of provinces appears under the **Tax** subtab. On the **Field Naming** subtab, you can edit the field names displayed on forms and in columns on search results, lists, and reports. See [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

### Related Topics

-   [Creating Tax Codes - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856762.html)
-   [Creating Tax Groups - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857206.html)
-   [Viewing Canadian Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1860262.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Processing Goods and Services Tax (GST) Refunds - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859567.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

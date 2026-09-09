---
id: "section_N1832322"
type: "section"
title: "Setting Tax Preferences for Australia"
branch: "australia-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Australia Help Topics > Australia Tax Topics > Setting Tax Preferences for Australia"
parent: "chapter_N1832106"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1832322.html"
anchors: []
sha256: "4cbdd84456aab6e6c20b2f8ef8c5d01e5cdeff6e5209c82c2e3cc656fb04e146"
---

The following preferences are available when configuring tax for nexuses in Australia.

-   **Enable Tax Lookup on Sales and Purchases** - This box is checked by default to enable NetSuite to determine appropriate tax codes to use on sales and purchases. Clear this box if you do not want NetSuite to determine the correct tax code based on the shipping address of the customer or vendor. If you use SuiteScript to query third party tax services, clear this box.
    
-   **Print Tax Code Summary on Sales Forms** - Check this box if you want to include a summary of the taxes paid per tax code on printed transaction forms such as estimates, sales orders, and sales invoices. The tax code summary is shown only if two or more tax codes are used on the transaction.
    
    If you check this box, make sure you choose your preferred PDF layout for transaction type forms.
    
    To set your transaction form PDF layout preferences, go to _Customization > Forms > Transaction Form PDF Layouts_.
    
    If the Preferred box for Transaction Layout with Tax Summary is checked, NetSuite shows the tax summary as a separate element at the bottom of the form, above the totals. If you choose any of the standard or classic transaction type layouts, NetSuite shows the tax summary in the main body of the form as part of the columns element. For more information about transaction form PDF layouts, see [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html).
    
-   **Foreign Trade** - Check this box if your company conducts trade with foreign companies or individuals.
    
    Note:
    
    When Foreign Trade preference is off, out of district charge Tax Codes won't be visible in the Tax Codes list.
    
-   **Tax Reporting Cash Basis** - Check this box if your company reports its tax liability on a cash basis rather than an accrual basis.
    
-   **Display ABN Field in Web Store** - Check this box to allow customers to enter their Australian Business Number when checking out of your Web store.
    
-   **Tax Code for International Sale** - Choose the default tax code for orders placed by international customers.
    
-   **Default Tax Code** - Choose the default tax code the system will use in your transactions if no tax code has been predefined for the customer or items.
    
    Important:
    
    The **Default Tax Code** field is required. In a OneWorld account, if you click **Save** and the system prompts you to enter a value in the **Default Tax Code** field, you may have one or more nexuses where a default tax code has not yet been selected. Look for this nexus and supply the missing information, and then click **Save**.
    
    Warning:
    
    When you inactivate a tax control account, then any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes on the affected nexuses, item records, customer records, and vendor records. Alternatively, you can re-activate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
    
-   **Tax Code Lists Include** - Select whether you want tax codes, tax groups or both to appear on transactions. The Tax Code Lists Include preference does not apply to journals.
    
-   **Preferred Tax Agency** - Select the tax agency to which you pay Goods and Services Tax.
    

If you have Advanced Taxes enabled in your account, the **Preferred Tax Agency** field appears in the **Tax** subtab. A **Field Naming** subtab is also provided so you can edit the field names displayed on forms and in columns on search results, lists, and reports. See [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

### Related Topics

-   [Creating Tax Codes - Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1834295.html)
-   [Australia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3802804453.html)
-   [Using Wine Equalization Tax (WET)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3830143961.html)
-   [Accounting for Goods and Services Tax (GST) - Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1833730.html)
-   [Setting Up Your Business Activity Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1834047.html)
-   [Viewing Australian Goods and Services Tax (GST) Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1837720.html)
-   [Australia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1832106.html)
-   [Australia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595666.html)
-   [Shipping Integration with Australia Post](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274389015.html)
-   [Setting Up Australia-specific Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540889422.html)
-   [Australia Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540887347.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

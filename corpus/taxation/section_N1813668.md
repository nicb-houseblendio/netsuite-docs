---
id: "section_N1813668"
type: "section"
title: "Setting Tax Preferences"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Setting Tax Preferences"
parent: "chapter_N1813074"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html"
anchors: ["procedure_N1813704", "bridgehead_4851529115"]
sha256: "a693b64f7635c63168b78579091de0b6495cc5469dbdd814cf1de04452cf18aa"
---

The following preferences are available for VAT/GST nexuses only. For US, see [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html), and for Canada, see [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html).

#### To set tax preferences for a nexus: {#procedure_N1813704}

1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
2.  If you have more than one nexus, click the tab for the nexus that you want to configure.
    
3.  **Enable Tax Lookup on Sales and Purchases** - This box is checked by default to enable NetSuite to determine appropriate tax codes to use on sales and purchases. Clear this box if you don't want NetSuite to determine the correct tax code based on the shipping address of the customer or vendor. If you use SuiteScript to query third party tax services, clear this box.
    
4.  **Print Tax Code Summary on Sales Forms** - Check this box if you want to include a summary of the taxes by tax rate on printed transaction forms such as Estimates, Sales Orders, and Sales Invoices. The tax code summary is shown only if two or more tax codes are used on the transaction.
    
    If you check this box, you must choose your preferred PDF layout for transaction type forms. To set your transaction form PDF layout preferences, go to _Customization > Forms > Transaction Form PDF Layouts_. If the **Preferred** box for Transaction Layout with Tax Summary is checked, NetSuite shows the tax summary as a separate element at the bottom of the form, above the totals. If you choose any of the standard or classic transaction type layouts, NetSuite shows the tax summary in the main body of the form as part of the columns element. For more information about transaction form PDF layouts, see [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html).
    
5.  **Only Use Tax Control Accounts on Tax Types** - This box is checked by default. If you disable this preference, you can create a tax type record on which you can select any account from your chart of accounts as your posting account for tax. After setting up the tax type, you must select it on the appropriate tax code records. For more information, see [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html).
    
6.  **Foreign Trade** - Check this box if your company conducts trade with foreign companies or individuals. If this box is checked, the system creates the Export tax code for the nexus.
    
7.  **Tax Reporting Cash Basis** - Check this box if you submit your tax returns on a cash basis, rather than invoice or accrual basis, to the tax authority.
    
8.  **Display Tax Registration Number Field in Web Store** - Check this box to enable customers to enter their tax identification numbers when checking out of your Web store. (The label shown for this field depends on the specific name of a country's VAT registration number or Company registration number, as appropriate.)
    
9.  **Default Tax Code** - Choose the default tax code that the system should use in your transactions if no tax code has been predefined for the customer or items.
    
    Important:
    
    The **Default Tax Code** field is required for all nexuses. In a OneWorld account, if you click **Save** and the system prompts you to enter a value in the **Default Tax Code** field, you may have one or more nexuses where a default tax code has not yet been selected. Look for this nexus and supply the missing information, and click **Save**.
    
    Warning:
    
    When you inactivate a tax control account, any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes on the affected nexuses, item records, customer records, and vendor records. Alternatively, you can re-activate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
    
10.  **Tax Code for Exports** - Select the default tax code for orders placed by international customers. For EU countries, this applies if the nexus is part of the EU and the customer is outside the EU.
     
11.  **Tax Code for Imports: Service Items** - Select the default tax code for service items purchased from vendors outside the country, or outside the EU if the nexus is an EU member country. This code will be used to show Reverse Charge tax on tax reports.
     
     Note:
     
     Reverse Charge reporting on imports currently does extend to Canada, Australia, and Japan.
     
12.  **Tax Code for Imports: Non-Service Items** - Select the default tax code for non-service items purchased from vendors outside the country, or outside the EU if the nexus is an EU member country. This code will be used to show Reverse Charge tax on tax reports.
     
     Note:
     
     Reverse Charge reporting on imports currently does extend to Canada, Australia, and Japan.
     
13.  **Tax Code Lists Include** - Choose whether you want tax codes, tax groups, or both to appear on transactions. The Tax Code Lists Include preference does not apply to journals.
     
14.  **Respect Discount Item Tax Preference** - This preference is used with the Apply Before Sales Tax preference on a Discount Item record.
     
     For information about the **Respect Discount Item Tax Preference** box for the U.S., see [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html).
     
     For information about the **Respect Discount Item Tax Preference** box for Brazil, China, and India, see [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html).
     
15.  **Preferred Tax Agency** - Select the tax agency that you pay taxes to.
     
     If you have Advanced Taxes enabled in your account, the **Preferred Tax Agency** field appears under the **Tax** subtab. On the Field Naming subtab, you can edit the field names displayed on forms and in columns on search results, lists, and reports. See [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).
     
16.  Set the tax rounding levels, methods, and precision settings for this nexus. See [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html).
     

## Example of Set Up Taxes Page with Multiple Nexuses {#bridgehead_4851529115}

![Example of Set Up Taxes page with multiple nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/SetUpTaxes.png)

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Creating Tax Codes - Other Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Setting Tax Preferences for Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1832322.html)
-   [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html)
-   [Setting Up Consumption Tax - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1934652.html)
-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

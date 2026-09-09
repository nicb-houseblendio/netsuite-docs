---
id: "section_N2038835"
type: "section"
title: "Setting U.S. Tax Preferences"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Setting U.S. Tax Preferences"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html"
anchors: ["bridgehead_4283726578", "procedure_N2039308"]
sha256: "5344480b670ef01edb30b2876289c61b40209e692d88a51f8d5b0ff59524cf58"
---

You can set U.S. sales tax preferences at _Setup > Accounting > Taxes > Set Up Taxes_.

The following preferences are available when configuring tax for nexuses in the United States.

-   **Enable Tax Lookup on Sales Transactions** - Clear this box if you don't want NetSuite to determine the correct tax code for customers based on their shipping addresses.
    
    For example, if you use SuiteScript to query third party tax services, then clear this box.
    
-   **Customers Default to Taxable** - Check this box if you want new customers to be charged tax by default.
    
    If you don't check this box, you can mark customers as taxable by checking the **Taxable** box on customer records. Charities and nonprofit organizations are usually not taxable. See [Entering Financial Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1078064.html).
    

In NetSuite U.S. edition accounts without Advanced Taxes, a customer isn't taxable only if the following conditions are true:

-   The **Taxable** box isn't checked.
    
-   The **Tax Item** field is blank on the customer record.
    

Previously, on the customer record, if the **Tax Item** field has a value, the system ignores it if the **Taxable** box isn't checked.

Similarly, the system ignores any tax codes or tax schedules selected on the item record or transaction record for that customer.

In 2012.2, a change in the tax lookup for U.S. edition NetSuite accounts removed the values in the **Tax Item** field on customer records in which the Taxable box isn't checked. If you are using the **Tax Item** field for purposes other than tax lookup, manually set the **Tax Item** field back to its original value. If **Tax Item** field has a value, the tax lookup returns that value instead of **not taxable** even if the **Taxable** box isn't checked. For example, you can set the **Tax Item** field to Avalara even if the **Taxable** box isn't checked.

-   **Items Default to Taxable** - Check this box if you want items to be taxable be default. If you choose not to check this box, you can mark items as taxable on transaction records.
    
-   **Charge Out of District Sales Taxes** - Check this box if you want NetSuite to determine the proper tax rate for customers with shipping addresses outside of your tax district.
    
    If you don't check the **Charge Out of District Sales Taxes** box, and there is no default tax item set on the customer record, then the system uses the home tax code for the corresponding state. If there is no home tax code, then the system uses the default tax code for the United States.
    
    If the **Charge Out of District Sales Taxes** box is checked, only the tax codes for nexuses assigned to the subsidiary will be available in transactions. A sales transaction isn't taxable if the nexus isn't assigned to the subsidiary, even if the customer is taxable or the item is taxable in the customer's state. Be sure to add appropriate nexuses to your subsidiary records.
    
-   **Per-Line Taxes on Transactions** - Check this box if you want to assign taxes to transaction line items. This enables you to charge different tax rates for items on the same transaction. Each time you add a line item to a sales transaction, you must select the appropriate tax code or tax group in the **Tax** column. You can add taxes to line items on the **Billable Items**, **Billable Expenses**, and **Billable Time** subtabs.
    
    If this box isn't checked:
    
    -   NetSuite applies the same tax code or tax group to the entire transaction.
        
    -   You can only specify whether an individual line item is taxable or not.
        
    -   Tax fields for shipping and handling are not available.
        
-   **Charge Sales Tax on Store Orders** - Select one of the following:
    
    -   **Always** - Charge sales tax on every web store order.
        
    -   **Never** - Omit sales tax on web store orders.
        
    -   **Per Customer Basis** - Charge sales tax on web store orders based on the **Taxable** box on customer records.
        
-   **Default Tax Code** - Select the tax code or group to use in the following situations:
    
    -   The customer's zip code does not match a tax code or tax group in the system.
        
    -   The **Charge Out of District Sales** box isn't checked and the business' zip code does not match a tax code or tax group in the system.
        
    
    If no sales tax items exist for the customer's ship to state, there is no tax at all and the default tax code won't be used.
    
    Important:
    
    The **Default Tax Code** field is required. If you are using a OneWorld account, the system prevents you from saving the Set Up Taxes page if a nexus does not have a value in the **Default Tax Code** field. Look for the nexus with the missing information by clicking each country nexus subtab. Select the default tax code for the nexus, and click **Save**.
    
    Warning:
    
    Tax codes associated with inactive tax control accounts are not available for selection when you create or edit a transaction record. Therefore, existing default tax codes associated with the inactive tax control account will no longer be valid. When you inactivate a tax control account, be sure to change the default tax codes on the affected nexuses, item records, customer records, and vendor records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
    
-   **Print/Email Tax Label Format** - This field is hidden if the **Per-Line Taxes on Transactions** box is checked. You can modify this value to customize the **Tax Total** field label on printed and emailed transaction forms.
    
    The following parameters are supported:
    
    -   **{item}** - Tax code
        
    -   **{rate}** - Tax rate, as a percentage, that is associated with the tax code
        
    -   **{label}** - Label for the **Tax Total** field. The default label is **{item}**. You can change the tax total label. After the tax total label is changed, this change is reflected in the PDF, regardless of the **Per-Line Taxes on Transactions** setting. See [Changing the Tax Total Label](#bridgehead_4283726578).
        
    
    The default format is **{label} ({item} {rate})**, for example:
    
    **Tax (Alameda County 9.75%)**.
    
-   **Tax Code Lists Include** - Select whether you want tax codes, tax groups or both to appear on transactions. The Tax Code Lists Include preference does not apply to journals.
    
-   **Respect Discount Item Tax Preference**
    
    -   If this box is checked, transaction level discount is applied after tax, only if the **Apply Before Sales Tax** box isn't checked on the discount item.
        
    -   If this box isn't checked, transaction level discount is applied always before tax.
        
-   **State, Preferred Tax Agency, and Home Code** - Select each state's tax agency and home tax code from the dropdown:
    
    -   **Preferred Tax Agency** - The tax agency to which you pay the taxes collected on transactions
        
    -   **Home Tax Code** - Tax code to use for sales that you don't ship to another location
        
    
    If the Advanced Taxes feature is enabled in your account, the list of states appears under the **Tax** subtab. On the **Field Naming** subtab, you can edit the field names displayed on forms and in columns on search results, lists, and reports. See [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).
    

## Changing the Tax Total Label {#bridgehead_4283726578}

You can change the label for the **Tax Total** field. This field appears on transactions forms for printing and for sending by email.

#### To change the Tax Total label: {#procedure_N2039308}

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  For custom forms, select the **Edit** link next to the form name. If you want to create a custom form, click the **Customize** link next to the form name.
    
3.  Click the **Printing Fields** subtab, and click the **Footer** subtab.
    
4.  Edit the label of the **Tax Total**.
    
5.  Click **Save**.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Adding or Deleting a U.S. State Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4283733632.html)
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
-   [U.S. Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042330.html)
-   [Importing the State Sales Tax Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041195.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

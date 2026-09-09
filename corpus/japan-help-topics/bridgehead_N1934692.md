---
id: "bridgehead_N1934692"
type: "bridgehead"
title: "Tax Preferences for Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Tax Topics > Setting Up Consumption Tax - Japan > Tax Preferences for Japan"
parent: "section_N1934652"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1934692.html"
anchors: ["procedure_N1934700"]
sha256: "0049d6ce07187c9bf334b9110bf2d98e7731ec9e764c8922eef69ebdf4f343d8"
---

To set up taxes in your account, do these steps.

#### To set company-wide consumption tax preferences: {#procedure_N1934700}

1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
2.  If you've more than one tax nexus, click the **Japan** subtab.
    
3.  **Enable Tax Lookup on Sales and Purchases** - This box is checked by default to enable NetSuite to determine appropriate tax codes to use on sales and purchases. Clear this box if you don't want NetSuite to determine the correct tax code based on the shipping address of the customer or vendor. If you use SuiteScript to query third party tax services, clear this box.
    
4.  **Print Tax Code Summary on Sales Forms** - Check this box if you want to include a summary of the taxes paid per tax code on printed transaction forms such as estimates, sales orders, and sales invoices. The tax code summary is shown only if two or more tax codes are used on the transaction.
    
    If you check this box, make sure that you choose your preferred PDF layout for transaction type forms.
    
    To set your transaction form PDF layout preferences, go to _Customization > Forms > Transaction Form PDF Layouts_.
    
    If the **Preferred** box for **Transaction Layout with Tax Summary** is checked, NetSuite shows the tax summary separately at the bottom of the form, above the totals. If you choose any of the standard or classic transaction type layouts, NetSuite shows the tax summary in the main body of the form in the columns. For more information about transaction form PDF layouts, see [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html).
    
5.  **Foreign Trade** - Check this box if your company conducts trade with foreign companies or individuals.
    
6.  **Tax Reporting Cash Basis** - Check this box if your company reports its tax liability on a cash basis rather than an accrual basis.
    
7.  **Display Tax Registration Number Field in Web Store** - The label for this field varies depending on the specific name of a country's business tax identification number. Check this box to enable customers to enter their tax identification numbers when checking out of your web store.
    
8.  **Tax Rounding Level** - Specify the tax rounding level for this nexus:
    
    -   If you select **Item Line Level**, tax is rounded per line.
        
    -   If you select **Transaction Level**, the rounding is applied at the tax total level, using this formula: round (Subtotal x Tax Rate) = Tax Total.
        
    
    For more information about tax rounding level, see [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html).
    
9.  **Tax Code for International Sale** - Choose the default tax code for orders placed by international customers.
    
10.  **Default Tax Code** - Choose the default tax code the system will use in your transactions if no tax code has been predefined for the customer or items.
     
     Important:
     
     The **Default Tax Code** field is required. NetSuite OneWorld prevents you from saving the Set Up Taxes page if a nexus doesn't have a value in the **Default Tax Code** field. Look for the nexus with the missing information by clicking each country nexus subtab. Select the default tax code for the nexus, and click **Save**.
     
     Warning:
     
     Tax codes associated with inactive tax control accounts aren't available for selection when you create or edit a transaction record. Therefore, existing default tax codes associated with the inactive tax control account will no longer be valid. When you inactivate a tax control account, be sure to change the default tax codes on the affected nexuses, item records, customer records, and vendor records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
     
11.  **Tax Code Lists Include** - Select the tax codes to appear on transactions. The **Tax Code Lists Include** preference doesn't apply to journals.
     
     Warning:
     
     It's critical to specify the rounding precision and rounding method for tax values based on the requirements of your tax authority. Failure to do so can result in incorrect tax amounts being reported.
     
     Important:
     
     Currently, it isn't possible to specify the rounding precision or rounding method using CSV import, web service, or mass update. You must either specify these values on the Setup > Accounting > Setup Taxes page under the subtab for the country, or check the **Allow override rounding setting per Entity** box to specify rounding settings for each customer and vendor.
     
12.  In the **Tax Rounding Precision** field, you can select these values:
     
     -   1 and Below (default)
         
     -   10 and Below
         
     -   100 and Below
         
13.  In the **Tax Rounding Method** field, you can select these values:
     
     -   Round Down (default)
         
     -   Round Off
         
     -   Round Up
         
14.  To apply rounding precision to the Japanese Yen, check the **Apply rounding precision setting if currency precision is not 0** box. This setting also applies to other currencies that don't use decimal fractions.
     
     If the **Apply rounding precision setting if currency precision is not 0 box** is checked, NetSuite will round every value in the specified currency, which means this preference overrides all other rounding preferences. Consider these cases:
     
     -   If the **Apply rounding precision setting if currency precision is not 0** box is checked, and the **Tax Rounding Level** field is set to **Transaction Level**, the system ignores the transaction level rounding because the amount is already rounded based on the currency.
         
     -   If the **Apply rounding precision setting if currency precision is not 0** box is checked, and the **Allow override rounding setting per Entity** box is checked, the system ignores the rounding setting specified on the entity record.
         
15.  In the **Preferred Tax Agency** field, select the tax agency to which you pay tax.
     

If you've the Advanced Taxes feature enabled in your account, the **Preferred Tax Agency** field is shown on the **Tax** subtab. You can also use the **Field Naming** subtab to edit the field names displayed on forms, and in columns on search results, lists, and reports. See [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1816436"
type: "section"
title: "Creating Tax Codes - Other Nexuses"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Creating Tax Codes - Other Nexuses"
parent: "chapter_N1813074"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1816436.html"
anchors: ["procedure_N1816459", "bridgehead_N1816882"]
sha256: "a1f87047930fb551cf93f00d5362d8f4e342569ec17bff8aa7a4eb98a57c32fe"
---

Tax codes determine how much tax is paid on each transaction line item. Various tax code properties define a tax code. For more information, see the tax code tables in the country-specific tax topics.

The following steps are for creating a tax code for any country except the US, UK, and Canada.

#### To create a tax code for nexuses except US, UK, and Canada: {#procedure_N1816459}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  On the New Tax Code page, if your account has other subsidiaries or nexuses, click the country that you are making a tax code for.
    
3.  On the Tax Code page, enter values in the following fields and check the tax code properties that apply to the tax code:
    
    -   **Tax Code** - Enter the name or abbreviation for this tax code. This code appears in the Tax Code column on sales transactions.
        
    -   **Description** - Enter a description for this tax code.
        
    -   **Rate** - Enter the tax percentage charged on an item with this tax code.
        
    -   **Effective From** - Enter the date this tax code first goes into effect.
        
    -   **Valid Until** - Enter the last date this tax code is in effect.
        
    -   For OneWorld accounts:
        
        -   **Subsidiaries** - Select the subsidiaries that this tax code applies to.
            
        -   **Include Children** - Check this box if you want to include child subsidiaries.
            
    -   **EC Code** - For the European Union member states, check this box if this tax code is used for transactions with customers or vendors in the European Union.
        
    -   **Reverse Charge Code** - Check this box if your company receives or provides services that are subject to the Place of Supply rules (that is, purchaser is liable for VAT).
        
    -   **Notional Rate Derived From** - If this tax code is derived from another tax code, select the code you are basing this tax code on. This field applies primarily to the EU countries and the rate is applied to calculate intra-community B2B values for VAT reporting purposes only.
        
        Note:
        
        You can select a value for this field only if either the **EC Code** or **Reverse Charge Code** box is also checked.
        
    -   **Applies to Service Items** - Check this box if this tax code is used for transactions related to services and is subject to reverse charges.
        
    -   **Export** - Check this box if this tax code is used for transactions involving exporting of goods.
        
        Important:
        
        If you are an EU customer, carefully review your tax codes. In the EC Code tax codes provisioned by NetSuite (EC Code box is checked), you must clear the **Export** box. To edit a tax code, see [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html).
        
    -   **Exempt** - Check this box to indicate that whatever this tax code applies to is exempt from tax.
        
    -   **Default Code** - Check this box if you want this tax code selected by default on transactions.
        
    -   **Exclude From VAT Reports** - Check this box if you don't want transactions that have this tax code to be included in VAT reports.
        
    -   **Inactive** - Check this box to inactivate this tax code. Inactive tax codes don't show in lists on transactions and records.
        
    -   **Tax Agency** - Select the tax authority to whom you submit tax reports and remit payments.
        
        Default tax agencies are automatically set up when a subsidiary or nexus is created. If the tax agency does not appear in the dropdown list, you can create one. For more information, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
        
    -   **Tax Type** - Select the type of tax code (for example, **VAT**).
        
        When you select a tax type, the tax control accounts for this tax code type appear in the **Purchase Tax Account** field and the **Sales Tax Account** field.
        
        You can create new tax code types at _Setup > Accounting > Taxes > Tax Types (Administrator)_.
        
        For more information about tax types, see [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
        
    -   **Tax Exemption Reason** - For reverse charge, zero rate, and exempt tax codes, select the legal justification for the tax exemption.
        
        Note:
        
        This field is available if you are creating a tax code for Portugal.
        
    -   **Available On** - Select the types of transactions that this tax code can be applied to. You can select one of the following:
        
        -   **Purchase Transactions**
            
        -   **Sales Transactions**
            
        -   **Both**
            
    -   Check the boxes of the additional tax code properties that apply to this tax code, for example **Capital Goods**, **Government**, **Import**, **Reduced Rate**, etcetera.
        
    -   **GCC Member State** - Check this box if the tax code will be used in transactions with Gulf Cooperation Council (GCC) member states.
        
4.  Click **Save**.
    

Note:

Certain tax code properties are displayed only if you have installed the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html), and vary depending on the country that you are making tax codes for. NetSuite uses these tax properties to generate values on each field of [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html). For information, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

## Tax Code Example {#bridgehead_N1816882}

![Example of a Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/NewTaxCode.png)

### Related Topics

-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Paying Tax Liabilities - Non-U.S. Editions and Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817593.html)
-   [VAT and GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2050955.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)
-   [Creating a Tax Group (All Countries Except US and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

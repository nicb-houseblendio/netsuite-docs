---
id: "section_N2026362"
type: "section"
title: "Creating Tax Codes - United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom Tax Topics For Accounts Without SuiteTax > Creating Tax Codes - United Kingdom"
parent: "section_156922742495"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2026362.html"
anchors: ["subsect_1030044225", "bridgehead_N2026382", "bridgehead_N2028572", "procedure_N2028582"]
sha256: "9c43356977702eb942f8c4a28472cc2535dae0b440756317ad9b73d5db66906b"
---

Note:

This topic is for NetSuite accounts that use the International Tax Reports SuiteApp. If you have the SuiteTax feature enabled in your account, see [United Kingdom Tax Reporting Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157598390063.html).

Tax codes determine how much tax your company must bill and pay on each transaction line item. In the United Kingdom Edition, NetSuite provides default tax codes. However, you should review the codes to make sure that the properties on each are set correctly. You can edit the properties in the tax codes, rename the tax codes, or create new tax codes.

## Important Things to Note {#subsect_1030044225}

-   The International Tax Reports SuiteApp only supports 139 unique tax codes per tax period for each country.
    
-   You can use more than 139 tax codes for each country if these tax codes are not used in the same tax period.
    

## United Kingdom Tax Codes {#bridgehead_N2026382}

The following table shows the tax properties required to correctly generate the United Kingdom VAT100 provided by the International Tax Reports SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

For information about notional rates in EU B2B transactions and VAT reports, see [EU Notional VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489598173.html).

Important:

Please consult HMRC for the current tax rates.

On the New Tax Code or Edit Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the United Kingdom VAT100, see [What goes into each box - United Kingdom VAT100 report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2030237.html).

| Tax Code | Description | Property | Rate | Notional Rate | Available On |
| --- | --- | --- | --- | --- | --- |
| E-GB | Exempt | Exempt | 0% | \- | Both (Sales and Purchases) |
| ER-GB | Reduced rate EC code for intra-community goods between Northern Ireland and EU Member States | Effective from January 1, 2021 EC Code | 0% | R-GB | Both (Sales and Purchases) |
| ES-GB | Standard rate EC code for intra-community goods between Northern Ireland and EU Member States | Effective from January 1, 2021 EC Code | 0% | S-GB | Both (Sales and Purchases) |
| ESSN-GB | EC code for non-taxable intra-community purchases (services) from EU Member States to Northern Ireland | Effective from January 1, 2021 EC Code Applies to Service Item Non taxable | 0% | \- | Sales |
| ESSP-GB | EC code for intra-community purchases (services) from EU Member States to Northern Ireland | Effective from January 1, 2021 EC Code Applies to Service Item | 0% | S-GB | Purchases |
| ESSS-GB | EC code for intra-community sales (services) from Northern Ireland to EU Member States | Effective from January 1, 2021 EC Code Applies to Service Items | 0% | S-GB | Sales |
| EZ-GB | Zero rate EC code for intra-community goods between Northern Ireland and EU Member States | Effective from January 1, 2021 EC Code | 0% | Z-GB | Both (Sales and Purchases) |
| I-GB | Purchase of supplies outside of the EU | Import Reverse Charge Code | 0% | S-GB | Purchases |
| IPA1-GB | Postponed import VAT on goods purchased from EU and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Import VAT | 0% | S-GB | Purchases |
| IPA2-GB | Postponed import VAT on goods purchased from EU and non-EU countries | Effective from January 1, 2021 Reverse Charge Code Import VAT Reduced Rate | 0% | R-GB | Purchases |
| IV-GB | 100% VAT bill | Import VAT | 0% | \- | Purchases |
| O-GB | International exports | Export | 0% | \- | Sales |
| R-GB | Reduced rate | \- | 5% | \- | Both (Sales and Purchases) |
| R1-GB | Reduced rate 12.5% | Effective from October 1, 2021 | 12.5% | \- | Both (Sales and Purchases) |
| RC-GB | Reverse charge | Reverse Charge Code | 0% | S-GB | Both (Sales and Purchases) |
| RC1-GB | Reverse charge | Reverse Charge Code | 0% | R-GB | Both (Sales and Purchases) |
| RCS-GB | Purchase of services from non-EU suppliers | Reverse Charge Code Applies to Service Items | 0% | S-GB | Purchases |
| RCS1-GB | Purchase of services from non-EU suppliers | Reverse Charge Code Applies to Service Items | 0% | R-GB | Purchases |
| S-GB | Standard rate | \- | 20% | \- | Both (Sales and Purchases) |
| Z-GB | Zero rate | \- | 0% | \- | Both (Sales and Purchases) |

Notional rates are used in the EU for reporting purposes only. They have no monetary value. To create a tax code, see [Creating a Tax Code - United Kingdom](#bridgehead_N2028572).

Important:

When entering an import VAT bill, a 100% VAT bill, you can enter the value either in the **Amount** field **OR** the **VAT Amount** field at the item line level. Whichever method you choose, this net amount or tax amount is correctly reflected in the computation of the value in Box 4 of the United Kingdom VAT100 Report. The drilldown for this tax code merely shows which field you entered the VAT in.

## Creating a Tax Code - United Kingdom {#bridgehead_N2028572}

#### To create a United Kingdom tax code: {#procedure_N2028582}

1.  Go to _Setup > Accounting > Taxes > Tax Codes > New_.
    
2.  Select the **United Kingdom (GB)** Country Code to go to the Tax Code page.
    
3.  Complete the fields on the Tax Code page:
    
    -   **Tax Code** - Enter the name or an abbreviation for this tax code.
        
    -   **Description** - Enter text that describes this tax code.
        
    -   **Rate** - Enter the tax percentage that is charged on an item with this tax code.
        
    -   **Effective From** - Enter the date this tax code first goes into effect.
        
    -   **Valid Until** - Enter the last date this tax code is in effect.
        
    -   **Subsidiaries** - Select a subsidiary if you are using a OneWorld account.
        
    -   **Include Children** - Check this box to apply the tax code to the children of the selected subsidiary if you are using a OneWorld account.
        
    -   **EC Code** - Check this box if this tax code is used for transactions with customers or vendors in the European Union.
        
    -   **Applies to service items** - Check this box if this tax code applies to services.
        
    -   **Reverse Charge Code** - Check this box if this tax is a reverse charge.
        
    -   **Notional Rate Derived From** - If this is an EC tax code, select the code and rate this new tax code is based on.
        
    -   **Export** - Check this box if this tax code is used in transactions involving exports.
        
    -   **Exempt** - Check this box if this tax code is used for tax-exempt transactions.
        
    -   **Default Code** - Check this box to make this the default tax code.
        
    -   **Exclude from VAT Reports** - Check this box if you don't want this tax code to appear on reports.
        
    -   **Inactive** - Check this box if you don't want to make this tax code available now.
        
    -   **Tax Agency** - Select the tax agency that this tax is paid to. You can set up vendor records for tax agencies. For more information, see [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
        
    -   **Tax Type** - Select the tax type for this tax code. When you select a tax type, the tax control accounts for this tax type appear in the Purchase Tax Account and Sales Tax Account fields. You can create new tax types at Setup > Accounting > Taxes > Tax Types > New. For more information about Tax Types, see [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
        
    -   **Purchase Tax Account** - When you select the Tax Type, NetSuite populates the Purchase Tax Account and Sales Tax Account fields with the appropriate accounts for the selected tax type.
        
    -   **Sales Tax Account** - When you select the Tax Type, NetSuite populates the Purchase Tax Account and Sales Tax Account fields with the appropriate accounts for the selected tax type.
        
    -   **Available on** - Select the types of transactions that this tax code can be applied to.
        
    -   **Non-Taxable** - Check this box if this tax code will be used to identify transactions that are not subject to the tax law.
        
4.  Click **Save**.
    
    When you create sales or purchase transactions, you can apply this tax code to line items.
    
    To create an acquisition tax code, see [Creating Acquisition Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817104.html).
    

### Related Topics

-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Creating Acquisition Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817104.html)
-   [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html)
-   [Inactivating or Deleting Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1808226.html)
-   [VAT and GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2050955.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

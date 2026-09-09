---
id: "section_N1983994"
type: "section"
title: "Singapore Tax Codes"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Singapore Tax Codes"
parent: "chapter_N1981261"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html"
anchors: ["bridgehead_N1984063", "bridgehead_1524617492", "procedure_1524617492", "procedure_1524617704"]
sha256: "1721f8f7b0268143151cd230f7342ef8733aa94951bd9cb4010ff341b344de9b"
---

Tax codes determine how much tax is due for each transaction line item. For NetSuite to calculate correct values on transaction records and tax reports, you must ensure that the tax codes for Singapore are set up correctly.

For more information about tax codes, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html).

## Tax Code Table for Singapore {#bridgehead_N1984063}

The following table shows the tax properties required to correctly generate the Singapore tax reports and tax audit files provided by the International Tax Reports SuiteApp and the Tax Audit Files SuiteApp. The tax code names or letters presented in the table are suggested names or default system preferences. You can rename the tax codes. Tax reports identify transactions by looking at the tax code properties, not the tax code names.

On the New Tax Code page, check the boxes of the properties that apply to the tax code. For more information about tax code properties, see [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html).

To understand how NetSuite uses the tax codes to get the values for the Singapore GST F5 Return, see [What goes into each box - Singapore GST F5 Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987905.html).

Note:

Tax type for the following tax codes should be set to GST\_SG. This tax type is already provided in your NetSuite account.

| Tax Code | Description | Rate | Notional Rate | Property | Purchase Tax Account | Sales Tax Account | Available On | Effective From | Valid Until |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| DS8-SG | Supplies required to be reported under the GST legislation Note: If you already have an existing Singapore tax codes in your account, you must manually edit the DS-SG tax code and check the Deemed Supply box. | 8% | \- | Deemed Supply | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| DS9-SG | Supplies required to be reported under the GST legislation Note: If you already have an existing Singapore tax codes in your account, you must manually edit the DS-SG tax code and check the Deemed Supply box. | 9% | \- | Deemed Supply | \- | GST on Sales | Sales | January 1, 2024 | \- |
| EP-SG | Purchases relating to residential properties or certain financial services | 0% | \- | Exempt Exclude from VAT Reports | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| ES33-SG | Exempt supplies made under Regulation 33 | 0% | \- | Exempt | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| ESN33-SG | Exempt supplies that are not covered under Regulation 33 | 0% | \- | Exempt | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| IM8-SG | Goods imported into Singapore | 8% | \- | Import | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| IM9-SG | Goods imported into Singapore | 9% | \- | Import | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| ME-SG | Goods imported under the Major Exporter Scheme and Third Party Logistics Scheme | 0% | \- | Import Export | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| NR-SG | Goods and services purchased from non-GST registered supplier/trader | 0% | \- | Exempt Exclude from VAT Reports | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| OP-SG | Purchase of goods outside the scope of GST | 0% | \- | Exclude from VAT Reports | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| OS-SG | Out of scope supplies | 0% | \- | Exclude from VAT Reports | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| SR8-SG | Standard rate | 8% | \- | Default | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SR9-SG | Standard rate | 9% | \- | Default | \- | GST on Sales | Sales | January 1, 2024 | \- |
| SRCA8-C-SG | Customer accounting supply accountable by the customer on supplier's behalf Note: If you already have an existing Singapore subsidiary or nexus in your account, you must create these tax codes manually. For more information about how to edit and create tax codes, see [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html). | 0% | SR8-SG | Reverse Charge Purchaser Issued Invoice | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SRCA9-C-SG | GST-exclusive value of the sold prescribed goods Note: If you already have an existing Singapore subsidiary or nexus in your account, you must create these tax codes manually. For more information about how to edit and create tax codes, see [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html). | 9% | SR9-SG | Reverse Charge Purchaser Issued Invoice | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| SRCA8-S-SG | GST-exclusive value of the sold prescribed goods Note: If you already have an existing Singapore subsidiary or nexus in your account, you must create these tax codes manually. For more information about how to edit and create tax codes, see [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html). | 8% | SR8-SG | Reverse Charge | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SRCA9-S-SG | GST-exclusive value of the sold prescribed goods Note: If you already have an existing Singapore subsidiary or nexus in your account, you must create these tax codes manually. For more information about how to edit and create tax codes, see [Editing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807882.html) and [Creating Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1807199.html). | 9% | SR9-SG | Reverse Charge | \- | GST on Sales | Sales | January 1, 2024 | \- |
| SRLVG8-SG | Own supply of low value goods | 8% | \- | Nonresident | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SRLVG9-SG | Own supply of low value goods | 9% | \- | Nonresident | \- | GST on Sales | Sales | January 1, 2024 | \- |
| SROVR8-LVG-SG | Supply of low value goods accountable by the redeliverer or electronic marketplace on behalf of third-party suppliers | 8% | \- | Applies to Digital Services Nonresident | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SROVR8-RS-SG | Supply of remote services accountable by the electronic marketplace under the Overseas Vendor Registration Regime | 8% | \- | Applies to Digital Services Applies to Service Items Nonresident | \- | GST on Sales | Sales | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SROVR9-LVG-SG | Supply of low value goods accountable by the redeliverer or electronic marketplace on behalf of third-party suppliers | 9% | \- | Applies to Digital Services Nonresident | \- | GST on Sales | Sales | January 1, 2024 | \- |
| SROVR9-RS-SG | Supply of remote services accountable by the electronic marketplace under the Overseas Vendor Registration Regime | 9% | \- | Applies to Digital Services Applies to Service Items Nonresident | \- | GST on Sales | Sales | January 1, 2024 | \- |
| SRRC8-SG | GST on imported services and low value goods by way of reverse charge | 8% | SR8-SG | Reverse Charge Applies to Service Items Import | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| SRRC9-SG | GST on imported services and low value goods by way of reverse charge | 9% | SR9-SG | Reverse Charge Applies to Service Items Import | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| TX8-E33-SG | Regulation 33 exempt supplies | 8% | \- | \- | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX9-E33-SG | Regulation 33 exempt supplies | 9% | \- | \- | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| TX8-N33-SG | Non-Regulation 33 exempt supplies | 8% | \- | Exempt | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX9-N33-SG | Non-Regulation 33 exempt supplies | 9% | \- | Exempt | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| TX8-RE-SG | Residual input tax | 8% | \- | Exempt | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX9-RE-SG | Residual input tax | 9% | \- | Exempt | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| TX8-SG | Goods, services or both purchased from GST registered suppliers | 8% | \- | \- | GST on Purchases | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX8CA-SG | GST-exclusive value of the purchased prescribed goods | 8% | TX8-SG | Reverse Charge | GST on Purchases | GST on Sales | \- | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX8CA2-SG | Goods, services or both purchased from GST registered suppliers Note: You must create this tax code manually. To create this tax code, see [Singapore Customer Accounting Tax Codes](#bridgehead_1524617492). | 8% | TX8-SG | Reverse Charge Input Tax | Deferred GST on Purchases | GST on Sales | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX8CA3-SG | Goods, services or both purchased from GST registered suppliers Note: You must create this tax code manually. To create this tax code, see [Singapore Customer Accounting Tax Codes](#bridgehead_1524617492). | 8% | TX8-SG | Reverse Charge Input and Output Tax | Deferred GST on Purchases | Deferred GST on Sales | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| TX9-SG | Goods, services or both purchased from GST registered suppliers | 9% | \- | \- | GST on Purchases | \- | Purchases | January 1, 2024 | \- |
| TX9CA-SG | Goods, services or both purchased from GST registered suppliers | 0% | TX9-SG | Reverse Charge | GST on Purchases | GST on Sales | Purchases | January 1, 2024 | \- |
| TX9CA2-SG | Goods and/or services purchased from GST registered suppliers Note: You must create this tax code manually. To create this tax code, see [Singapore Customer Accounting Tax Codes](#bridgehead_1524617492). | 0% | TX9-SG | Reverse Charge Input Tax | Deferred GST on Purchases | GST on Sales | Purchases | January 1, 2024 | \- |
| TX9CA3-SG | Goods and/or services purchased from GST registered suppliers Note: You must create this tax code manually. To create this tax code, see [Singapore Customer Accounting Tax Codes](#bridgehead_1524617492). | 0% | TX9-SG | Reverse Charge Input and Output Tax | Deferred GST on Purchases | Deferred GST on Sales | Purchases | January 1, 2024 | \- |
| UNDEF\_SG | Used when NetSuite cannot determine the appropriate tax code for a transaction | 0% | \- | Exclude from VAT reports | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| ZP-SG | Zero rated purchases | 0% | \- | \- | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |
| ZR-SG | Zero rated | 0% | \- | Export | GST on Purchases | GST on Sales | Both (Sales and Purchases) | \- | \- |

Note:

Tax type for the following tax code should be set to Disallowed GST\_SG. To create this tax type, see [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html).

| Tax Code | Description | Rate | Property | Purchase Tax Account | Sales Tax Account | Available On | Effective From | Valid Until |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BL-SG | GST incurred but disallowed | 7% | Exempt | GST Input Disallowed | \- | Both (Sales and Purchases) | \- | December 31, 2022 |
| BL8-SG | GST incurred but disallowed | 8% | Exempt Exclude from VAT Reports | GST Input Disallowed | \- | Purchases | January 1, 2023 | December 31, 2023 Note: You must manually edit this tax code to set the Valid Until date. |
| BL9-SG | GST incurred but disallowed | 9% | Exempt Exclude from VAT Reports | GST Input Disallowed | \- | Purchases | January 1, 2024 | \- |

## Singapore Customer Accounting Tax Codes {#bridgehead_1524617492}

You must create the following new Customer Accounting tax codes:

Important:

You must install the Tax Audit Files, International Tax Reports, and Supplementary Tax Calculation SuiteApps to generate Customer Accounting transactions through the Singapore IRAS Audit File (IAF).

-   TX8CA2-SG
    
-   TX8CA3-SG
    

#### To create the TX8CA2-SG tax code: {#procedure_1524617492}

1.  Go to Setup > Accounting > Taxes > Tax Codes > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Check the **Reverse Charge Code** and **Post Notional Tax Amount** boxes.
    
4.  Provide the following information:
    
    -   **Tax Code**: TX8CA2-SG
        
    -   **Tax Type**: GST\_SG
        
    -   **Deferred**: Input Tax
        
    -   **Notional Tax Debit Account**: Deferred GST on Purchases SG
        
    -   **Notional Tax Credit Account**: GST on Sales SG
        
5.  Click **Save**.
    

Important:

Input tax (GST on Purchases SG) is excluded from the GST F5 return and IRAS Audit File (IAF) when the **TX8CA2-SG** tax code is used. Only the Output tax (GST on Sales SG) is reported. To record the input tax (GST on Purchases SG), you must create a journal entry upon receipt of the tax invoice. To create journal entry, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

#### To create the TX8CA3-SG tax code: {#procedure_1524617704}

1.  Go to Setup > Accounting > Taxes > Tax Codes > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Check the **Reverse Charge Code** and **Post Notional Tax Amount** boxes.
    
4.  Provide the following information:
    
    -   **Tax Code**: TX8CA3-SG
        
    -   **Tax Type**: GST\_SG
        
    -   **Deferred**: Input and Output Tax
        
    -   **Notional Tax Debit Account**: Deferred GST on Purchases SG
        
    -   **Notional Tax Credit Account**: Deferred GST on Sales SG
        
5.  Click **Save**.
    

Important:

The **TX8CA3-SG** tax code does not report output tax (GST on Sales SG) or input tax (GST on Purchases SG) in the GST F5 return. It also excludes these taxes from the IRAS Audit File (IAF). To record the input and output tax, create a journal entry when you receive the tax invoice. To create journal entry, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

### Related Topics

-   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html)
-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)
-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)
-   [Singapore Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html)
-   [Singapore GST Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987604.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

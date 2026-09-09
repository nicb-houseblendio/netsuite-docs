---
id: "chapter_N1791910"
type: "chapter"
title: "Tax Accounting Overview"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Tax Accounting Overview"
parent: "preface_3710626699"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html"
anchors: ["bridgehead_N1792407", "bridgehead_N1793558", "bridgehead_4222598063", "bridgehead_N1793584", "bridgehead_N1793662", "bridgehead_N1793728", "bridgehead_N1793844", "bridgehead_N1793953"]
sha256: "102545cb0298626a99c1e8dabd501a6fe4a0fb7c6377457fcce2093e2aa5b1b0"
---

Note:

The topics in this section cover the legacy tax solution in NetSuite. Check these help topics if you're using a NetSuite account without the SuiteTax feature.

SuiteTax provides more flexibility to support country-specific needs and changing tax laws for calculation and reporting. For more details about the differences between Legacy Tax and SuiteTax, see [Differences between SuiteTax and Legacy Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0315035511.html).

NetSuite helps you track, calculate, and pay different taxes based on the sale or purchase of products and services. Read the following tax topics to see how to enable and use NetSuite's tax features.

## Setting Up Tax Features {#bridgehead_N1792407}

To see what tax features you can enable, read these topics:

-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html) - Describes what you must set up in your account to enable NetSuite to track taxes.
    
-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html) - Describes how to set up and use tax periods.
    
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html) - Describes the advanced taxes feature and how to enable it in your NetSuite account.
    
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html) - Describes how to set up tax codes, tax groups, tax types, tax control accounts. For most countries, NetSuite provides the basic tax setup when you get an account or set up a nexus. You'll still need to set up those tax items, add details, and check they're correct.
    
-   [EU One Stop Shop (OSS)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4163851800.html) - Describes how you can charge the appropriate tax on B2C sales of digital services based on the VAT rate of the customer's EU member state.
    
-   [Taxation Features Provided by SuiteApps from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740493324.html) - provides links to information about International Tax Reports, Tax Audit Files, and Withholding Tax SuiteApps, and how to enable them
    

## VAT/GST Support on Intercompany Journal Entries {#bridgehead_N1793558}

If your business has multiple subsidiaries, use Intercompany Journal Entries to record the tax impact of transactions between them. You don't have to manually post individual entries for each subsidiary.

You can transfer an item or asset between subsidiaries, even if they have different nexuses or tax rates. Intercompany journal entries post to both the source and destination subsidiaries in a single transaction, and NetSuite automatically posts the tax values to the right accounts.

For information about intercompany journal entries, see [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html).

## Tax Amounts on Transactions {#bridgehead_4222598063}

-   **Changing the shipping address**\- Changing the shipping address on a transaction can affect the tax total and reporting. Depending on your tax setup, changing the shipping address might change the nexus and tax codes, too.
    
-   **Using multiple shipping routes** - If you want to use multiple shipping routes on a transaction, see [Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263041.html).
    
-   **Changing a tax code** - You can change the tax code on a transaction line. To see how tax is recalculated when the tax code changed when you do this, check [Recalculating Line Item Amounts When the Tax Code Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4222571547.html).
    
-   **Tax amount rounding** -If an item quantity has decimals (like in software sales), you might notice the tax amount doesn't round up as expected. This is not a defect.
    
    Rounding differences happen because the tax amount comes from the rounded amount and rounded gross amount.
    
    Here's how the system calculates gross and tax amounts in this case:
    
    amount = round(quantity \* rate)
    
    gross\_amount = round(quantity \* rate \* tax\_rate)
    
    tax\_amount = gross\_amount - amount = round(quantity \* rate \* tax\_rate) - round(quantity \* rate)
    
    In other words, gross\_amount = amount + tax\_amount.
    
    One consequence is that when the amount increases, the gross never decreases. The tax amount can decrease or stay the same, as you can see below. This ensures you can get any gross amount value, which matters more than the tax amount alone.
    
    **Example**
    
    Here's an example using a 15% tax rate:
    
    | Quantity | Rate | Amount | Rounded | Gross Amount | Rounded | Tax Amount |
    | --- | --- | --- | --- | --- | --- | --- |
    | 1.33331 | 150.0 | 199.9965 | 200.00 | 229.995975 | 230.00 | 30.00 |
    | 1.33330 | 150.0 | 199.9950 | 200.00 | 229.994250 | 229.99 | 29.99 |
    | 1.33329 | 150.0 | 199.9935 | 199.99 | 229.992525 | 229.99 | 30.00 |
    

## Taxes on Discounts {#bridgehead_N1793584}

For information about applying taxes on discounts on your transactions, check these topics:

-   [Applying Sales Tax or VAT to Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817936.html)
    
-   [Taxing Transactions with a Contingent/Volume Discount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029417.html)
    
-   [Recording VAT on Prompt Payment Discounts on Sales Invoices for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225129843.html)
    
-   [Recording VAT on Prompt Payment Discounts on Purchases for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225131687.html)
    

## Nondeductible Input Tax {#bridgehead_N1793662}

For information about nondeductible input tax and recording it in the general ledger, see these topics:

-   [Recording Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822590.html)
    
    -   [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html)
        
    -   [Applying Nondeductible Input Tax on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1823395.html)
        

## Tax Reporting {#bridgehead_N1793728}

NetSuite offers tax reporting for VAT, GST, and withholding tax. For information, check these topics:

-   [U.S. Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042330.html) - for information about US sales tax reports
    
-   [Viewing Canadian Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1860262.html) - for information about Canadian GST/HST and PST reports
    
-   [Viewing Australian Goods and Services Tax (GST) Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1837720.html) - for information about Australian GST reports
    
-   [United Kingdom Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2026020.html) - for information about the UK VAT 100 tax return and online submission of tax reports to Her Majesty's Revenue and Customs (HMRC)
    
-   [VAT and GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2050955.html) - for information about country-specific VAT/GST reports, EU Sales Lists, Intrastat Reports, and saved reports for purchases and sales by tax code
    
-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html) - for information about audit files that you can submit to tax authorities
    
-   [Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2078886.html) - for information about tracking and reporting withholding tax
    

## Paying Tax Liabilities {#bridgehead_N1793844}

NetSuite can also help you pay tax liabilities. For information about posting tax journal entries and preparing tax payments, read these topics:

-   [Paying Tax Liabilities - Non-U.S. Editions and Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817593.html)
    
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
    
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
    
-   [Accounting for Goods and Services Tax (GST) - Australia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1833730.html)
    
-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)
    
-   [Accounting for Creditable Withholding Tax - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1960490.html)
    

## Country-specific Tax Topics {#bridgehead_N1793953}

For information about general international and country-specific tax topics, read the following:

-   [General International Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1813074.html)
    
-   [Australia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1832106.html)
    
-   [Austria Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1823604.html)
    
-   [Belgium Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1839485.html)
    
-   [Bulgaria Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1846363.html)
    
-   [Canada Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1856070.html)
    
-   [Chile Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1865199.html)
    
-   [Colombia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1867954.html)
    
-   [Cyprus Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1873007.html)
    
-   [Czechia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1874317.html)
    
-   [Denmark Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1885300.html)
    
-   [European Union (EU) Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4138676838.html)
    
-   [Finland Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1888576.html)
    
-   [France Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1890188.html)
    
-   [Germany Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1897534.html)
    
-   [Indonesia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1918792.html)
    
-   [Ireland Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1926430.html)
    
-   [Italy Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1931995.html)
    
-   [Japan Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1934076.html)
    
-   [Kenya Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1938961.html)
    
-   [Luxembourg Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156862264625.html)
    
-   [Malaysia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4228472831.html)
    
-   [Mexico Tax Topics (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1940317.html)
    
-   [Netherlands Tax Topics In Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1942820.html)
    
-   [New Zealand Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1947563.html)
    
-   [Norway Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1948317.html)
    
-   [Peru Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1949362.html)
    
-   [Philippines Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1950898.html)
    
-   [Poland Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1967656.html)
    
-   [Portugal Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1970643.html)
    
-   [Romania Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1978514.html)
    
-   [Serbia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1980213.html)
    
-   [Singapore Tax Topics for Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1981261.html)
    
-   [Slovakia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1989528.html)
    
-   [Slovenia Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1992349.html)
    
-   [South Africa Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1995074.html)
    
-   [South Korea Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1995977.html)
    
-   [Spain Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1999169.html)
    
-   [Sweden Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2004566.html)
    
-   [Switzerland Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2009888.html)
    
-   [Taiwan (Province of China) Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2010868.html)
    
-   [Thailand Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2018510.html)
    
-   [Türkiye Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2021231.html)
    
-   [Ukraine Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2022755.html)
    
-   [United Kingdom Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156922742495.html)
    
-   [United States Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2038572.html)
    
-   [Uruguay Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2035552.html)
    
-   [Viet Nam Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2047227.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

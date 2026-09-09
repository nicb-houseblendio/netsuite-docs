---
id: "section_N1810558"
type: "section"
title: "Tax Types Overview"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Types Overview"
parent: "chapter_N1805198"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html"
anchors: ["bridgehead_N1810639", "bridgehead_N1810881", "bridgehead_N1811193", "bridgehead_N1811487"]
sha256: "34dd69c5c7698c92bac77f61e9f19ba53f430e9bb8d9a784f4e1a536d7a20720"
---

A tax type determines where the tax paid or collected is tracked on the balance sheet. The balance sheet account where NetSuite posts collected or paid tax is called the tax control account.

In NetSuite, the tax types may already be set up by default, or set up for you by Professional Services. When you add a subsidiary in a new country, tax types for that country become available automatically. An administrator can create new tax types if needed.

Note:

Changes made to tax types are captured in system notes. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

The definition of a tax type includes the tax type's tax control accounts. This is how NetSuite tracks taxes on the balance sheet. But, in some countries, companies have to record tax on income or expense accounts in the general ledger, balance sheet, and income statement reports. On the Set Up Taxes page for a VAT/GST nexus, you can turn off the Only Use Tax Control Accounts on Tax Types preference. When it's turned off, you can post tax amounts to any account in your chart of accounts, if you've created a tax type record that uses this account, and you've set up a tax code that uses the new tax type. For more information, see [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html).

Tax types are used to define tax codes. If you have the Advanced Taxes feature enabled, tax types are also linked to a country. When defining a tax code, available tax types depend on the selected country. For example, when creating a tax code for the United States, the dropdown list for the Tax Type field includes Sales Tax. If you're creating a tax code for the United Kingdom, available tax types will include VAT.

A transaction record includes information about the tax code or tax group. The tax code or group holds the information about the tax type. The tax type holds the information about the tax control account.

A tax type is associated with a nexus. To create a tax type, see [Creating a Tax Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1811821.html).

## Examples of tax types and tax control accounts (Australia) {#bridgehead_N1810639}

Tax Type Name: GST

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| Australia | GST Collected | GST Paid |

Tax Type Name: LCT

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| Australia | LCT Collected | LCT Paid |

## Examples of tax types and tax control accounts (Canada) {#bridgehead_N1810881}

Tax Type Name: PST

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| QC | PST Payable QC | PST Expenses QC |
| ON | PST Payable ON | PST Expenses ON |

Tax Type Name: GST/HST

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| QC | GST/HST Payable | GST/HST on Purchases |
| ON | GST/HST Payable | GST/HST on Purchases |

## Examples of tax types and tax control accounts (United States) {#bridgehead_N1811193}

Tax Type Name: State

| Nexus | Liability/Sales Tax Account |
| --- | --- |
| CA | Sales Tax Payable CA |
| GA | Sales Tax Payable GA |
| NY | Sales Tax Payable NY |

Tax Type Name: Transit

| Nexus | Liability/Sales Tax Account |
| --- | --- |
| CA | Sales Tax Payable CA |
| GA | Sales Tax Payable GA |
| NY | Sales Tax Payable NY |

## Examples of tax types and tax control accounts (International) {#bridgehead_N1811487}

Tax Type: VAT

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| Taiwan (Province of China) | VAT on Sales | VAT on Purchases |

Tax Type Name: GST

| Nexus | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| Singapore | GST on Sales | GST on Purchases |

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Creating a Tax Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1811821.html)
-   [Removing Restrictions for Tax Control Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812010.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

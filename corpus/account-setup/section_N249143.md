---
id: "section_N249143"
type: "section"
title: "Formatting for Dates, Numbers, Phone Numbers, and Time"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Set Company Preferences > Formatting for Dates, Numbers, Phone Numbers, and Time"
parent: "section_N242860"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N249143.html"
anchors: ["subsect_0221024321", "subsect_0221031552", "subsect_0221033825"]
sha256: "21cccf2ed87f40c022c9bc112736c4298aa7c0ee4a6790eb5a77e05957cbb05d"
---

You can use the default formatting for dates, numbers, phone numbers and time, or override them at the company, subsidiary, or user level.

To change the default settings at each level, go to:

-   **Company -** _Setup > Company > General Preferences_.
    
-   **Subsidiary -** _Setup > Company > Classifications > Subsidiaries_. When you edit the subsidiary, you can find the date format in the Preferences > General subtab.
    
-   **User -** _Home > Set Preferences_. The date format is in the formatting section.
    

## Formatting Dates {#subsect_0221024321}

The default date format is M/D/YYYY. You can also select the format of abbreviated and full dates. The abbreviated date format appears on reports, forms, and data entry pages.

Note:

By default, users can override the date formats you select. If you don't want that, go to _Setup > Company > General Preferences_. On the **Overriding Preferences** subtab, clear the **Allow Override** box next to **Date Format** or **Long Date Format**.

The following table shows some date formats and how March 5, 2025 would look in each one.

| Date Format | Example |
| --- | --- |
| M/D/YYYY | 3/5/2025 |
| D/M/YYYY | 5/3/2025 |
| D-Mon-YYYY | 5-Mar-2025 |
| D.M.YYYY | 5.3.2025 |
| DD/MM/YYYY | 05/03/2025 |
| DD-MONTH-YYYY | 05-March-2025 |

Note:

Not all date formats are available in every locale.

## Formatting Numbers {#subsect_0221031552}

Set the Number Format and Negative Number Format to specify how numbers display on the screen.

The Number Format provides the following format options for thousands separators and decimal places:

-   **Thousands separator -** Comma, period, space, and reverse comma.
    
-   **Decimal places -** Comma and period.
    

You can show negative numbers with a minus sign or in parentheses.

-   **Minus sign -** -100
    
-   **Parentheses -** (100)
    

Note:

The following guidelines apply to number formatting:

-   Number format preferences don't apply to exports, SOAP web services, SuiteScript, or CSV imports.
    
-   Currency format settings apply to amounts on reports and printed transactions.
    
-   Values with a currency symbol, such as €123,45 or $123.45, use the currency format, not the number format.
    
-   On the screen, foreign currency amounts use the currency format. Base currency amounts in columns on transactions forms and subtabs follow the number format preferences.
    

## Formatting Time {#subsect_0221033825}

NetSuite supports both the 12-hour and 24-hour clocks. The following time format options are available:

| Date Format | Example |
| --- | --- |
| hh:mm AM/PM | 08:00 PM |
| hh:mm (24 hours) | 20:00 |
| hh-mm AM/PM | 08-00 PM |
| hh-mm (24 hours) | 20:00 |

### Related Topics

-   [Set Company Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N242860.html)
-   [NetSuite Preference Levels Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243257.html)
-   [Setting General Account Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243797.html)
-   [Overriding Company Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N246888.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

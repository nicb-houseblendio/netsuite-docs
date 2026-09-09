---
id: "section_N435556"
type: "section"
title: "Requirements for Inventory Worksheet CSV File Data"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Simple Imports > Single Inventory Worksheet Import > Requirements for Inventory Worksheet CSV File Data"
parent: "section_N434282"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N435556.html"
anchors: ["bridgehead_N435622", "bridgehead_3705049959", "bridgehead_N436437"]
sha256: "b67b627f9c014edcf815a2b82c045745d40ce76a33c578a37848ecec2102b622"
---

Your inventory worksheet CSV file should include both header and line-level data. Each row of the CSV file represents a transaction line, with repeated header field values, and a different item, new quantity, and new value for each line.

For more information, see:

-   [Inventory Worksheet Field Details](#bridgehead_N435622)
    
-   [Using IDs Instead of Names for Items](#bridgehead_3705049959)
    
-   [Example Inventory Worksheet CSV File](#bridgehead_N436437)
    

## Inventory Worksheet Field Details {#bridgehead_N435622}

The following tables provide details about the fields supported in a CSV file used for an inventory worksheet import.

Important:

A CSV file that contains different values for a header-level field is considered invalid. The same header-level field values must be included in each row, or all header fields must be blank after the first row. Or, you can omit header fields from the CSV file, and instead set default values for them on the Import Assistant Field Mapping page. See [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).

| Header Field | **Notes** |
| --- | --- |
| Adjustment Account | Usually an expense account for inventory adjustments. This field is required and should match the name of an existing account at _Lists > Accounting > Accounts_. If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, values should include both account number and name, such as **11000 Accounts Payable**. Number-only values, such as **11000**, also are supported. Name-only values, such as **Accounts Payable**, aren't supported when this preference is enabled. If this preference isn't enabled, name-only values should be used. Note that account names may be non-hierarchical, even for sub-accounts. |
| Class | Must match the name of an existing class at _Setup > Company > Classes_. Most CSV imports require the use of the full hierarchical name, but inventory worksheet import supports the use of the simplified name. For example, both **Headquarters : Executive** and **Executive** are supported. |
| Date | Required. Default value provided if CSV file doesn't include this field. |
| Department | Must match the name of an existing department at _Setup > Company > Departments_. Most CSV imports require the use of the full hierarchical name, but inventory worksheet import supports the use of the simplified name. For example, both **Marketing : Marcom** and **Marcom** are supported. |
| Location | Required if the Multi-Location Inventory feature is enabled. Must match the name of an existing location at _Setup > Company > Locations_. Most CSV imports require the use of the full hierarchical name, but inventory worksheet import supports the use of the simplified name. For example, for location name, both **California : Los Angeles** and **Los Angeles** are supported. |
| Memo | Provides a detailed description displayed in the transaction detail list and other reports. Maximum length = 4000. |
| Posting Period | An error is returned if a closed period is specified. |
| Reference # | Used to track adjustments. This number appears on register and account detail reports. Maximum length = 45. Default value provided if CSV file doesn't include this field. Note that if you provide a value that is already in use, an error occurs. |
| Subsidiary | Required for OneWorld accounts. Must match the name of an existing subsidiary at _Setup > Company > Subsidiaries_. Most CSV imports require the use of the full hierarchical name, but journal entry import supports the use of the simplified name. For example, both **EMEA : Germany** and **Germany** are supported. |
| Transaction Order | Required. Must use one of the following values:
-   **First transaction in day** - posts the worksheet at the beginning of the day and doesn't include additional inventory transactions entered during that day for this worksheet.
-   **Last transaction in day** - posts the worksheet at the end of the day and includes all inventory transactions entered during that day for this worksheet.

 |

Each line in the CSV file should include a different value for each line-level field.

| Line-Level Field | Notes |
| --- | --- |
| Item | Required. Item to be adjusted. Must match an existing item at _Lists > Accounting > Items_. You can't reference the same item in multiple lines. Note: By default item names should be used as values for this field, but you can also choose to use internal ID or external ID values. See [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html). |
| New Qty | Required. The new total quantity on hand for the item. |
| New Value | Required. The new value for the new quantity of item in stock. |

## Using IDs Instead of Names for Items {#bridgehead_3705049959}

By default, the Import Assistant expects the values in the Item column of your CSV file to match the names of existing items in the system. You have the option of setting up the import to expect either internal ID or external ID values instead.

-   The internal ID is a NetSuite system-assigned ID number. To display internal ID values on NetSuite forms, go to _Home > Set Preferences_. Click the General subtab, and in the Defaults section, check Show internal IDs. When this preference is enabled, a list displays the IDs as one of the columns.
    
-   The external ID is an ID number used by an external system. A record has an external ID only if the user created one when bringing the record into NetSuite.
    

To set the Item field to use ID instead of name values, click its edit icon on the Field Mapping page, and in the popup, select either Internal ID or External ID.

![Choose Reference Type field options in the Default Value or Reference Type window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/InvWorkRefType_2014_2.png)

## Example Inventory Worksheet CSV File {#bridgehead_N436437}

The following table illustrates a sample CSV file containing data for an inventory worksheet. Columns A-J contain header-level data, whereas columns K-M contain line-level data. Notice that the header-level fields include values only in the first row.

| A | B | C | D | E | F | G | H | I | J | K | L | M |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Date | Posting Period | Reference # | Adjustment Account | Subsidiary | Department | Class | Location | Memo | Transaction Order | Item | New Qty | New Value |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 7/22/2011 | \- | \- | 10100 Uncat Exp | USA | \- | \- | East Coast | July Cycle | Last Transaction in Day | Kid Sport Lunch Box | 120 | 1200.00 |
| \- | \- | \- | \- | \- | \- | \- | \- | \- | \- | Medium Cooler | 255 | 5100.00 |
| \- | \- | \- | \- | \- | \- | \- | \- | \- | \- | Small Icepack | 125 | 500.00 |
| \- | \- | \- | \- | \- | \- | \- | \- | \- | \- | Large Icepack | 180 | 1080.00 |
| \- | \- | \- | \- | \- | \- | \- | \- | \- | \- | Multicolor Snack Bag | 60 | 480.00 |
| \- | \- | \- | \- | \- | \- | \- | \- | \- | \- | Kid Flower Lunch Box | 85 | 850.00 |

For more information about adjusting inventory, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).

### Related Topics

-   [Single Inventory Worksheet Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434282.html)
-   [Using the Inventory Worksheet Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

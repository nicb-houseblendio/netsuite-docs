---
id: "section_N364491"
type: "section"
title: "Custom List Sublist Data"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Customization Import Type > Custom List Import > Custom List Sublist Data"
parent: "section_N363830"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N364491.html"
anchors: ["bridgehead_N364534", "bridgehead_3705043200"]
sha256: "51de3cfd4f9330680de32dda75ed1da2979e4f152e43fe7f4d201ce56c432945"
---

You can import data for two sublists - [Custom List Values](#bridgehead_N364534) and [Custom List Translation](#bridgehead_3705043200).

This topic describes these sublists in more detail. See also [Custom List CSV Multiple File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N365834.html) for tips on organizing CSV files that include sublist data.

## Custom List Values {#bridgehead_N364534}

The Custom List Values sublist specifies the options, or values, to be displayed in the custom list. For example, in a custom list named 'Sizes,' sublist values might be 'small,' 'medium,' and 'large.' The sublist fields are described in the following table.

This sublist is selectively updatable based on the ID field.

| Field | Notes | Required? |
| --- | --- | --- |
| Abbreviation | Available only if the Matrix Items feature is enabled for your account (at _Setup > Company > Enable Features_ > Items & Inventory). You can use this field to add an abbreviation for each [Custom List Values](#bridgehead_N364534) in your list. If, after the import, you review the newly imported record in the UI, note that the Abbreviation field shows up only if [Matrix Option List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html#bridgehead_N364181) is set to Yes for this particular custom list. However, even if you import abbreviations when setting Matrix Option List to No, the system saves your abbreviations, and they can be displayed later. | No |
| ID | This field - which is the key for the sublist - is automatically generated and read only. Do **not** attempt to populate this field with a value of your own choosing. Attempts to do so are generally ignored and in some cases (if you use illegal characters) result in errors that halt your import. You should use this field only when attempting to selectively update a record in the sublist using the automatically generated value for the field. This field is **not** related to the [ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html#bridgehead_N364115) field that's available to be mapped as a body field when SuiteScript is enabled. | No, but if you're trying to selectively update the sublist, you must include a mapping for the ID of those records you want to modify. |
| Inactive | A value of No means that the value displays as an option in your custom list. A value of Yes means the value is hidden. | No, but if you don't include a mapping for this field, the system uses the default value, which is No. |
| Translation: (Language) | Available when both of the following are true:
-   The Multi-Language feature is enabled for your account (at _Setup > Company > Enable Features_).
-   You have added one or more languages to the Languages subtab at _Setup > Company > General Preferences_.

For each language listed on the Languages subtab, the Import Assistant mapping page offers a corresponding **Translation: (Language)** field. For each sublist record, you can use these fields to add translations for the corresponding entry in the [Custom List Values](#bridgehead_N364534) column for this sublist record. | No |
| Value | The value, or option, to be shown in the custom list. For example, for a list of colors, values might be 'red,' 'blue,' and 'green.' | Yes |

## Custom List Translation {#bridgehead_3705043200}

The Custom List Translation sublist lets you add translations for the name of the sublist. For you to use this sublist, both of the following must be true:

-   The Multi-Language feature has been enabled (at _Setup > Company > Enable Features_).
    
-   You have added one or more languages to the Languages subtab at _Setup > Company > General Preferences_.
    

This sublist is selectively updatable based on the Language field.

| Field | Notes | Required? |
| --- | --- | --- |
| Language | Use this field to identify the language of the translation. This field is also the key for the sublist. | Yes. This field is not marked as required on the mapping page, but if you try to import data to this sublist and fail to map a value for Language, the import fails. |
| Name | The translation of the [Name](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html#bridgehead_N364194) body field that corresponds with the locale you entered for this sublist record. | No |

For general information about translations for custom lists, see [Adding Translations for Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852517.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)

### Related Topics

-   [Custom List Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363830.html)
-   [Custom List Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html)
-   [Custom List CSV Multiple File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N365834.html)
-   [Custom List CSV Single File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157890910739.html)
-   [Common Errors When Importing Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N369759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

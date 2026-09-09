---
id: "section_N363990"
type: "section"
title: "Custom List Body Fields"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Customization Import Type > Custom List Import > Custom List Body Fields"
parent: "section_N363830"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363990.html"
anchors: ["bridgehead_N364115", "bridgehead_N364155", "bridgehead_N364168", "bridgehead_N364181", "bridgehead_N364194", "bridgehead_N364248", "bridgehead_N364281", "bridgehead_N364306"]
sha256: "38c829bfed20dbf0ad6f860081168af2015c536b3170befdc7623adbf3c4b46d"
---

The following custom list body fields are available for mapping:

-   [ID](#bridgehead_N364115)
    
-   [Inactive](#bridgehead_N364155)
    
-   [Internal ID](#bridgehead_N364168)
    
-   [Matrix Option List](#bridgehead_N364181)
    
-   [Name](#bridgehead_N364194)
    
-   [Owner](#bridgehead_N364248)
    
-   [Show options in order entered](#bridgehead_N364281)
    

## ID {#bridgehead_N364115}

The field labeled 'ID' on the Import Assistant mapping page corresponds to the `scriptId` element in `customization.xsd`. It is neither the Internal ID nor an External ID.

Important:

The Custom List record doesn't support the External ID field.

![Custom List ID field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CustomListIDField.png)

The ID field is available only if Client SuiteScript and Server SuiteScript have been enabled at _Setup > Company > Enable Features_, on the SuiteCloud subtab.

The ID value must be unique.

Note:

The system adds the prefix `customlist` to whatever value you enter. For example, if you enter `_listColors`, the system saves the ID as `customlist_listColors`. This value can be used as an identifier for the record.

## Inactive {#bridgehead_N364155}

A value of Yes makes the list unavailable to be selected as the List/Record of a new custom field. The default is No.

## Internal ID {#bridgehead_N364168}

This field is available for mapping only if the import has a data handling option of Update, or Add or Update.

## Matrix Option List {#bridgehead_N364181}

This field is available only if the Accounting Matrix Items feature has been enabled at _Setup > Company > Enable Features_, on the Items & Inventory subtab. When the value is Yes, the system can display abbreviations for each value in the list. The default is No.

## Name {#bridgehead_N364194}

The value for Name shows up in the form you use to create a new custom field, as a choice in the List/Record dropdown list (unless you have chosen a value of Yes for the custom list's [Inactive](#bridgehead_N364155) field, which hides the list name from this view). The Name is **not** the user-facing label that ultimately appears on the custom form next to the list. (That label is the value you enter for the Label field on the custom field record.)

The illustration below shows where the name of the custom list appears when you create a new custom field, in this example, 'List A' in the List/Record dropdown list.

![List of days highlighted on the Custom Entity Field page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CustomList_CustomField_2014_2.png)

The Name field is required, and its value must be unique.

## Owner {#bridgehead_N364248}

If you don't create a mapping for Owner, the system identifies you as the owner. The mapping page doesn't indicate you're mapped as owner, but the import sets you as the owner for all imported records. If you don't want to be set as owner, create a mapping that sets the Owner field to another user or to null.

## Show options in order entered {#bridgehead_N364281}

A value of Yes places your custom list's values (which are defined by the [Custom List Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N364491.html#bridgehead_N364534) sublist) in the order they're listed in the CSV import file. A value of No places the values in alphabetical order.

If you don't create a mapping for this field, the import sets the value to Yes. The mapping page doesn't indicate that this default is being chosen, but you can see it on the resulting record after the import.

## For more details {#bridgehead_N364306}

For further details about fields that can be mapped, see the SOAP Schema Browser's [custom list](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customlist.html) reference page. However, note that the Convert to Custom Record field is not currently supported in the Import Assistant. With that exception, you can use the field definitions in the SOAP Schema Browser as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)

### Related Topics

-   [Custom List Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363830.html)
-   [Custom List Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N364491.html)
-   [Custom List CSV Multiple File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N365834.html)
-   [Custom List CSV Single File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157890910739.html)
-   [Common Errors When Importing Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N369759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

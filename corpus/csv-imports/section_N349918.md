---
id: "section_N349918"
type: "section"
title: "Assign Default Values during Field Mapping"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Four Field Mapping > Assign Default Values during Field Mapping"
parent: "section_N347418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html"
anchors: ["bridgehead_N349950", "bridgehead_N350018"]
sha256: "b8b14fca8910e49fbe3b8f8b4777192674d1f12e9a529ab4479dbf2a60d9691d"
---

The Import Assistant automatically populates some dependent field values when related field values are set, in the same manner that many dependent field values are automatically populated in the user interface.

You can also set default values for required fields on the Import Assistant's Field Mapping page. This gives every imported record the same value for that field. For example, when importing new leads, you might set the lead status to 'LEAD-New' by default.

To set a default value for a field on the Field Mapping page

1.  Click the edit icon in its row to open a popup.
    
    ![Edit icon on the Import Assistant Mapping page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/NSN_Import_Assistant.png)
2.  Choose **Provide Default Value**, and select a value from the dropdown or popup list.
    
    ![Default Value pop up window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/NSN_Import_Default_Value.png)
    
    Note:
    
    Whether the list of available values is a dropdown or popup list depends on the number of values and your setting for Maximum Entries in Dropdowns at _Home > Set Preferences_.
    

Even if you set a default value for fields in a sublist, no sublist data gets imported unless you map at least one field for that sublist. For more information about working with sublists, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Using Dependent Field Values as Defaults {#bridgehead_N349950}

When you click the edit icon for a dependent field, meaning a field with available values that vary according to the value selected for another field, the list does not filter values in the same manner that they are filtered in the user interface. These cases are most likely to occur in OneWorld accounts, for fields that are dependent on subsidiary values.

For example, in a OneWorld account, available tax code values for a transaction item vary according to the customer, and to the customer's associated subsidiary. In the user interface, the Tax Code field dropdown list filters the listed tax codes to only those that are valid. In the Import Assistant, the Default Value field lists all tax codes without any filtering.

Consider default values for dependent fields carefully. Because the Default Value does not filter the values for these fields, you may inadvertently select an invalid value. For example, you could select a tax code value that is not valid for some of the customers or subsidiaries listed in your CSV file. This type of invalid value can cause validation errors when you attempt to complete the Field Mapping step.

If a dependent field is not required, you have the option of entering values in the user interface after the import is complete.

## Assign a Default Value for the Primary Sales Rep Field {#bridgehead_N350018}

For Customer, Lead, or Prospect records added through CSV import, values for Primary Sales Rep do not default to be the user performing the import, so the Field Mapping page is a good place to specify a default value for this field. This behavior differs from the NetSuite user interface, where the user entering data on the form is the default for Primary Sales Rep.

### Related Topics

-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html)
-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)
-   [Required Fields on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349431.html)
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

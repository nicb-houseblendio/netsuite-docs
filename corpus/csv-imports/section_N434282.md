---
id: "section_N434282"
type: "section"
title: "Single Inventory Worksheet Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Simple Imports > Single Inventory Worksheet Import"
parent: "section_N433480"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434282.html"
anchors: ["bridgehead_N434301", "bridgehead_N434423", "bridgehead_N434440"]
sha256: "15c1368dc100fa30f27debf0617f5922177b91bec339e9631be09bb0085ded18"
---

In the NetSuite user interface, you can use the Inventory Worksheet form to make adjustments to the levels of inventory items in stock. On this form, you need to manually enter general information as well as changes to the quantity and value of each inventory item to be adjusted.

The Single Inventory Worksheet Import provides an alternative that you can use to create a new inventory worksheet in NetSuite. With this import, you can submit inventory adjustment data in a CSV file that can be built from a system-provided template. For inventory worksheets with many lines, this import can be significantly faster than data entry in the Inventory Worksheet form.

This type of import can be used for adjustments that are required after physical inventory counts. Another use case for this import is to reset stock quantity and value at the end of the NetSuite implementation phase.

## Inventory Worksheet Import Limitations {#bridgehead_N434301}

Review the following limitations to decide whether this import would be useful for you:

-   Each import can create one new inventory worksheet. You can't use the inventory worksheet import to update an existing NetSuite inventory worksheet or to create multiple inventory worksheets at one time.
    
-   Each inventory worksheet import can import data for one combination of class, department, location, and, if applicable, subsidiary values. You must do multiple import jobs to import data for multiple classes, departments, locations, or subsidiaries.
    
-   The inventory worksheet import currently doesn't support the import of bin information.
    
-   Like the inventory worksheet form in the user interface, this import is best suited if you're using average costing. The import, like the UI form, ignores LIFO and FIFO, so doesn't preserve that history.
    
-   The inventory worksheet import shares other limitations of the inventory worksheet form, including:
    
    -   New quantity values are exclusive of previous stock totals.
        
    -   Adjustments to lot numbered items, serial numbered items, and inactive items aren't supported.
        
    -   A change to the quantity of an assembly item changes the quantity of the assembly only; it doesn't change the quantity of individual member items.
        
-   Import is supported for inventory worksheets with up to 1,000 lines. However, poor performance results during import and in the user interface for inventory worksheets with over 1,000 lines, and these large inventory worksheets may not be editable in the user interface. Note that 1,000 lines aren't always processed by the import. If the timeout limit is reached during the import process, some records aren't processed. In this case, try the import with fewer than 1,000 lines.
    
-   You can't save field mappings for an inventory worksheet import.
    

## Permission for Inventory Worksheet Import {#bridgehead_N434423}

You need the Adjust Inventory Worksheet and Import CSV File permissions to import an inventory worksheet.

By default, only account administrators have the Adjust Inventory Worksheet permission. This permission isn't assigned to any standard roles. This permission can be added to a custom role that can be assigned to users who perform this type of import.

## How to Do an Inventory Worksheet Import {#bridgehead_N434440}

-   For details about the interface for importing an inventory worksheet, see [Using the Inventory Worksheet Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434577.html).
    
-   For tips to help you set up your CSV file for an inventory worksheet import, see [Requirements for Inventory Worksheet CSV File Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N435556.html).
    
-   For information about making inventory adjustments, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).
    

### Related Topics

-   [Simple Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

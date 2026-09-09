---
id: "section_N375476"
type: "section"
title: "Importing Related Items Groups"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Related Items Groups"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html"
anchors: []
sha256: "f5ad4635cc303af6681264d6d2cef282005c8e60cd928312138bd53f38451b62"
---

Related items groups are defined for items in Web stores to cross-sell items that complement each other. The Import Assistant supports the import of related item sublist data for item records when the Web Site feature is enabled.

On the Import Assistant Field Mapping page, you must map two fields for the Related Items sublist: Item and Type.

The Item field represents the item name that appears in the browser, whereas the Type field indicates the NetSuite type of relation, for example File Cabinet Item, Information Item, Item, Presentation Category Item.

-   To see available values for the Type field, create a new item in the browser, go to the Related Items subtab, and click the List button for the Item field. The top of the popup displays a dropdown list of available values for the Type field.
    
-   You can include Type values in your CSV files and select a default value for Type on the Field Mapping page by clicking the edit icon.
    
    ![Item and Type fields mapping example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/RelItemType.png)
    
    In the Default Value popup, select a default Type value (File Cabinet Item, Information Item, Item, or Presentation Category) from the dropdown list next to the Provide Default Value option.
    

![Default Value popup list.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/RelItemTypeSelect.png)

Note the following:

-   For an import job that includes large numbers of related item records, you should upload multiple CSV files.
    
-   Import of related items isn't supported for Non-Inventory Item for Purchase, Service Item for Purchase, or any Other Charge Item imports.
    

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

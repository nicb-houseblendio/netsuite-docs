---
id: "section_N370727"
type: "section"
title: "Item Record Types that Can Be Imported"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Item Record Types that Can Be Imported"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html"
anchors: []
sha256: "81fcf51051d8e16167c83cab9cee351840e2836a5963d1bb86b227d94a29df41"
---

The Items import type provides the ability to import the following NetSuite items record types, as shown in the Record Type dropdown list on the first page of the Import Assistant.

-   Assembly/BOM Item
    
    -   Lot Numbered Assembly/BOM Item
        
    -   Serialized Assembly/BOM Item
        
-   Description Item
    
-   Discount Item
    
-   Inventory Item (Not supported in NetCRM), including:
    
    -   Lot Numbered Inventory Item
        
    -   Serialized Inventory Item
        

Important:

For OneWorld accounts, the import of inventory item historical data dated prior to the date of the OneWorld upgrade in your account isn't supported. To maintain accurate inventory information, you should import only data that is dated later than the OneWorld upgrade and initial Multi-Location Inventory distribution.

-   Item Group
    
-   Kit/Package Item
    
-   Markup Item
    
-   Non-Inventory Item, including:
    
    -   for Purchase
        
    -   for Resale
        
    -   for Sale
        
-   Other Charge Item, including:
    
    -   for Purchase
        
    -   for Resale
        
    -   for Sale
        
-   Payment Item
    
-   Service Item, including:
    
    -   for Purchase
        
    -   for Resale
        
    -   for Sale
        
-   Subtotal Item
    

Note:

You can use the Import Assistant to import matrix options for Inventory Item, Non-Inventory Item, and Service Item imports, but you need to use the NetSuite user interface to set up possible matrix options as custom lists and custom item fields before you can complete an import of matrix item options. For information about importing matrix options for items, see [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html). For general information about matrix items in NetSuite, see [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html).

For details about fields that can be mapped in item records, refer to the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html), which includes a reference page for supported item types. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

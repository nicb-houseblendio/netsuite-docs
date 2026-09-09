---
id: "section_N433181"
type: "section"
title: "Site Category Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Website Import Type > Site Category Import"
parent: "section_N433102"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433181.html"
anchors: ["bridgehead_N433306", "bridgehead_N433342"]
sha256: "2e00abf470dfab779c0e3dd60aae5ac7155e6beb2e50a7b0a6bd12f01fe3fc47"
---

The site category import lets you add or update website categories in NetSuite. These categories are used to organize information and items for sale on your website. Each category must be associated with a presentation tab to be displayed in a website. Presentation tabs are the building blocks, or pages, in a website.

Supported fields for this import mostly match the fields on the Site Category page available at _Commerce > Site Builder > Categories > New_, including the following:

-   Category - name of the site category (required)
    
-   Site - the site where the category should be used (required when the Multiple Sites feature is enabled)
    
-   Subcategory of - the tab or category where this category is grouped
    
-   Display in Web Site - indicating whether the category should be displayed
    

For details about fields that can be mapped in the site category record, see the SOAP Schema Browser's [site category](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/sitecategory.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

Review the following guidelines for site category imports:

-   [Supported Site Category Sublist Data Import](#bridgehead_N433306)
    
-   [Importing Updates to Site Category Records](#bridgehead_N433342)
    

## Supported Site Category Sublist Data Import {#bridgehead_N433306}

The site category import supports the import of information and items to be included in each category, as Presentation Items sublist data. The records in this sublist can be File Cabinet items, information items, items to be sold on the website, or subcategories.

To import values for multiple presentation items per category, format your CSV file with repeating columns for the Presentation Items sublist fields (such as Item1, Type1, Item2, Type2, Item3, Type3), and map multiple instances of this sublist on the Import Assistant Field Mapping page. (Click the + sign next to the sublist to add mappable instances.)

![Import Assistant for site category import.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/sitecategory.png)

## Importing Updates to Site Category Records {#bridgehead_N433342}

If you need to import updates to existing site category records, use an identifier of internal ID or external ID to prevent duplication of records.

-   If you select the **Update** data handling option, you can use Category as an identifier to match records and perform updates.
    
-   If you select the **Add or Update** data handling options, no Category lookups are performed, so in the absence of internal ID or external ID, multiple records with the same category name may be added.
    

Note:

The site category import doesn't support the definition of an audience for categories to be published internally to an intranet or to specific set of individuals. If necessary, you can define an audience for a category on its record within NetSuite after the import.

### Additional Information

-   [Site Builder Tabs & Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2595349.html)

### Related Topics

-   [Website Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433102.html)
-   [Commerce Category Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512587491.html)
-   [CMS Page Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1560800028.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

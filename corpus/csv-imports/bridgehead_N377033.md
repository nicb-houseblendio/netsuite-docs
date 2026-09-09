---
id: "bridgehead_N377033"
type: "bridgehead"
title: "Tips for Matrix Items Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Matrix Options for Items > Tips for Matrix Items Import"
parent: "section_N375701"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N377033.html"
anchors: []
sha256: "25bb841f9d8436180a43bc05f8a05793621fac0cdbd0e1902aca6af40e204f6e"
---

-   When you select matrix options for a parent in the NetSuite user interface, child matrix items are created automatically. The CSV import process is different. Each parent matrix item and each child matrix item must be added or updated individually, and the CSV file should include a separate line for each parent matrix item and child matrix item. Otherwise, the rules for creation of matrix items in the NetSuite user interface generally also apply to matrix items imports.
    
-   Each child matrix item can have separate pricing data.
    
-   A limit of 2000 child matrix items are permitted for each parent matrix item.
    
-   You can use the Import Assistant to add child matrix items to existing parent matrix items. Use the Subitem of field to store the value of the parent matrix item for each child.
    
-   The following limitations apply to updates of matrix items with the Import Assistant:
    
    -   You can't change matrix option values for existing child matrix items.
        
    -   You can't change the parent matrix item (Subitem of value) for existing child matrix items.
        
    -   You can't change the matrix type value for existing matrix items.
        
    -   Unlike in the user interface, matrix items imports can't update child matrix items as a group in the parent item record. Each child matrix item record must be updated individually.
        
    -   Otherwise, the fields that you can update with matrix items imports are the same as those you can update manually in the user interface. For information, see [Editing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2229497.html).
        
-   You can't use the Import Assistant to delete matrix options.
    
-   In the user interface, child matrix items inherit Units Type field values from parent matrix items. However, items imports set Units Type field values separately on parent and child matrix items. You should map this field for both parent and child items and include values for both in CSV import files. Also note that Stock Units, Purchase Units, and Sale Units values are on Units Type values.
    
-   When you're using a CSV import for populating the facet field values, make sure that the facet field values are the same for the child matrix items. If the facet field values are not the same or they're missing for the child matrix items, the facet filter might not work as expected. This issue is observed only when you use non-matrix options as facet fields.
    

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Item Types that Support Matrix Options Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375858.html)
-   [Prerequisites for Importing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375963.html)
-   [Setting Up Custom Lists and Item Fields for Matrix Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376031.html)
-   [Setting Up Your CSV File for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376239.html)
-   [Mapping Fields for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376956.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

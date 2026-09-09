---
id: "section_N354236"
type: "section"
title: "Editing a Saved Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Working with Saved CSV Imports > Editing a Saved Import"
parent: "section_N353796"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html"
anchors: ["procedure_N354248"]
sha256: "6a72a2f0f2e1d118e3d99cb07e8733d236c3ed9ef68fb57a2e2bf081ebd20e91"
---

You might find a saved import map that is close to what you need for your import. You can edit this saved import mapping to run your import instead of creating a new import map.

#### To edit a saved import for reuse: {#procedure_N354248}

1.  Go to _Setup > Import/Export > Saved CSV Imports_.
    
2.  On the Saved CSV Imports page, find the import map you want to edit and click its link in the Name column. This action starts the Import Assistant.
    
3.  In the Import Assistant, make any changes you need, as described in [Step One Scan & Upload File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343532.html), [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html), [Step Three File Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347303.html), and [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html).
    
    Note:
    
    You can't remove a previously mapped required field from a saved import.
    
4.  On the Save Mapping & Start Import page, review the Import Map Name.
    
    -   If you want your changes to overwrite the existing saved import map, and to maintain the same name, don't change the name here.
        
    -   If you want to give the import map a different name, change it here.
        
    -   If you want to edit the description, do it here.
        
    
    Note:
    
    If the Multi-Language feature is enabled, you'll see a separate page to enter translations for the import name and description. If you change the name or description, remember to update the translations too See [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html).
    
5.  Review the options available under the Save button in the lower right corner of the Import Assistant:
    
    -   To overwrite the existing import map, click **Save**, or click **Save & Run**.
        
    -   To make a new import map, click **Save As**, or click **Save As & Run**. Be sure to give the import map a new name.
        
6.  You can use SuiteCloud Development Framework (SDF) to manage saved CSV import maps as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).
    
    You can use the Copy to Account feature to copy an individual saved CSV import map to another of your accounts. When you open a saved CSV import map in the Import Assistant, a clickable **Copy to Account** option is available in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).
    

### Related Topics

-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)
-   [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html)
-   [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html)
-   [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html)
-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

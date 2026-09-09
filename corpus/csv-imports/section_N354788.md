---
id: "section_N354788"
type: "section"
title: "Translating Import Map Name and Description"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Working with Saved CSV Imports > Translating Import Map Name and Description"
parent: "section_N353796"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html"
anchors: ["procedure_N354837"]
sha256: "82472691823836073361e20a7b1d5dcc17607273282caffdc0dbdc0f03348544"
---

If the Multi-Language feature is enabled in an account, saved import owners and account administrators can define translations for saved CSV imports' names and descriptions so they match the language of the NetSuite user interface.

When you switch the NetSuite UI to another language, the translated import names and descriptions show up on the Saved CSV Imports page.

Before you can translate import map names and descriptions, you must select translation languages at _Setup > Company > General Preferences_, on the Languages subtab. For details, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).

Note:

The Languages subtab at _Setup > Company > General Preferences_ lists both system-supported languages that can be used for the NetSuite user interface (and are available at _Home > Set Preferences_), and additional languages that can used for website translations only (and are not available at _Home > Set Preferences_). You should only enter translations for role names in system-supported languages, because these are the only languages that can be displayed in the user interface.

When you've set the languages, you can add translations in the CSV Import Map Translation dialog from the Saved CSV Imports page.

Important:

It is not possible to translate in the UI saved imports you have uploaded through SDF.

#### To define translations for a saved CSV import map: {#procedure_N354837}

1.  Go to _Setup > Import/Export > Saved CSV Imports_.
    
2.  On the Saved CSV Imports page, click **Translate** for the import.
    
    ![Translate field on the Saved CSV Imports page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/SavedImportTranslateLink.png)
    
    Important:
    
    This link is only available if you are the owner of a saved import or an account administrator.
    
3.  In the **CSV Import Map Translation** dialog, enter translations for the name and click **Done**, enter translations for the description and click **Done**, and click **Save**.
    
    ![CSV Import Map Translation window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/SavedImportTranslateDialog.png)
    -   You can return to this page as needed to edit translations later.
        
    -   You also can edit the original Name and Description values on this page. (Be sure to edit related translations after you edit an original value.)
        
    -   In the Name and Translation fields in the CSV Import Map Translation page you can enter up to 64 characters.
        

### Related Topics

-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)
-   [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html)
-   [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html)
-   [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

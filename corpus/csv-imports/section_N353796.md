---
id: "section_N353796"
type: "section"
title: "Working with Saved CSV Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Working with Saved CSV Imports"
parent: "chapter_N343158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html"
anchors: ["procedure_N353812"]
sha256: "ddfc3129c03f96562f7273347f0757b45069fabeccc000938ecc0da47845ccdf"
---

The Import Assistant can save import settings so that you can reuse them for later jobs. You can review mappings for your previously completed import jobs on the Saved CSV Imports page. If you are an administrator, you can review mappings for all previously completed import jobs in your account.

#### To work with a previously saved CSV import: {#procedure_N353812}

1.  Go to _Setup > Import/Export > Saved CSV Imports_.
    
2.  The Saved CSV Imports page shows all the saved import mappings you can access, including ones you've saved as well as those saved by others that include you in the audience.
    
3.  This page includes the following columns:
    
    -   ID - unique internal ID for saved mapping
        
    -   Name - name given to the field mapping in the Import Assistant
        
    -   Translate - link to CSV Import Map Translation dialog (only in accounts where the Multi-Language feature is enabled)
        
    -   Field Map - link to popup view of field mappings
        
    -   Description - description entered in the Import Assistant
        
    -   Type - record type of field mappings
        
    -   Owner - user who created the field mapping in the Import Assistant, or another user selected in the Share Import dialog
        
    -   Created - date when mapping was first saved
        
    -   Script ID - unique ID defined on the Save Mapping & Start Import page, used to reference the import map in SuiteScript
        
        Note:
        
        By default, import jobs created before Version 2012 Release 2, when this field was added, do not have script ID values. Import jobs created as of that release or later default to a script ID of CUSTIMPORT. If a script ID is set, it is prefixed with CUSTIMPORT.
        
    -   Last Modified - date when mapping was last changed
        
    -   Access - indicator of whether mapping is private, shared, or public, and link to Share Import dialog
        
    -   Delete - button to delete mapping, available only if you are the owner
        
4.  On the Saved CSV Imports page, you can:
    
    -   Select from the Record Type list to display mappings for a single record type.
        
    -   Open the saved import in the Import Assistant to edit its settings or rerun it, by clicking the link in the Name column. See [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html).
        
    -   In accounts where the Multi-Language feature is enabled, enter translations for a saved import's name and description. See [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html).
        
    -   Review the import's mappings by clicking **View** in the Field Map column. A popup opens displaying the mapped source and target fields, helping you to identify the correct import without having to go through the pages of the Import Assistant.
        
    -   Make an import mapping available to other users, or define a different owner for it, by clicking the link in the Access column. For more information, see [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html).
        
    -   Delete a saved import mapping, by clicking the ![Delete button](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/DelButton.png) button in the Delete column. This button is available only for mappings that you own. Only an administrator can delete saved CSV imports owned by other users.
        
    -   Click the New button to start the Import Assistant and create another import job.
        

The popup available from the View link in the Field Map column looks like the following:

![Popup window showing the mapped source and target fields.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/fieldmap.png)

Note:

You can use SuiteBundler to include CSV import maps in customization bundles. See [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html).

Note:

The SuiteCloud Development Framework (SDF) supports saved CSV imports. You can create, modify, import, and export saved CSV imports, and move your saved CSV imports between accounts. For more information, see [savedcsvimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2642962146.html).

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html)
-   [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html)
-   [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html)
-   [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html)
-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2148181"
type: "section"
title: "Updating Asset Records Using CSV Import"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Updating Fixed Assets Management Records > Updating Asset Records Using CSV Import"
parent: "chapter_N2147919"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148181.html"
anchors: ["procedure_N2148228"]
sha256: "f3902d44585819b0cfe32108e4e5fda70846f99414dbfa0708194ae0fc7b1667"
---

You can use the CSV Import Assistant in NetSuite to update existing data in the Fixed Assets Management SuiteApp. If the updates affect the original cost, depreciation start date, or cumulative depreciation, then you may also need to update the original asset history records.

On the Fixed Assets Management System Setup page, you can set which roles can edit asset values. For more information, see [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html).

Important:

Before you import asset data, it's best to perform a test import. Create a test CSV file with a few assets and review the formatting to ensure that data is imported with correct values. Make sure the asset type in the CSV file matches exactly how it's set up in your NetSuite account.

Important:

To ensure that FAM bundle scripts run on newly imported assets, enable **Run Server Scripts on CSV Import** (Fixed Assets > Setup > System Setup) and **Run Server SuiteScript and Trigger Workflows** (Setup > Import/Export > CSV Import Preferences).

#### To update asset records using CSV import: {#procedure_N2148228}

1.  Prepare an import file by creating a custom view from the existing Fixed Asset list in NetSuite.
    
    1.  Go to Fixed Assets > Lists > Assets.
        
    2.  Click **Customize View**.
        
    3.  Set Criteria to filter the list as necessary.
        
    4.  Choose the fields to update and add them to the **Results** subtab of the new custom view.
        
        Important:
        
        The NetSuite Internal ID of the Asset is required to link the updated information to the correct asset.
        
    5.  Click **Preview**.
        
    6.  Click **Export - CSV** and save the CSV file.
        
2.  On Fixed Assets > Setup > System Setup, make sure that the **Run Server Scripts on CSV Import** box isn't checked. If this box is checked the **Cumulative Depreciation**, **Last Depreciation Date**, and **Last Depreciation Period** will be automatically set to 0 even if your import file includes the correct amounts. For more information, see [General Guidelines for Importing Fixed Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163350867712.html).
    
3.  Go to Setup > Import/Export > Import CSV Records. In the Import Assistant Step 1 - Scan & Upload CSV File screen:
    
    1.  From the **Import Type** list, select **Custom Records**.
        
    2.  From the **Record Type** list, select **FAM Asset**.
        
    3.  Select the CSV file to upload.
        
    4.  Click **Next**.
        
4.  In the Import Assistant Step 2 - Import Options screen:
    
    1.  Set Data Handling to **Update**.
        
    2.  From the **Custom Form** list, select **Standard FAM Asset Form**.
        
    3.  Click **Next**.
        
5.  In the Import Assistant Step 4 - Field Mapping screen:
    
    1.  Map the fields in your CSV file to the NetSuite fields.
        
        -   Set the Internal ID mapping type to **Internal ID**.
            
            ![Setting the Reference Type to Internal ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ImportCSVMappingInternalID.png)
        -   Review the CSV fields and NetSuite fields to ensure that all required fields are mapped.
            
    2.  Click **Next**.
        
6.  In the Import Assistant Step 5 - Save Mapping and Start Import screen:
    
    1.  Enter an Import Map Name and Description.
        
    2.  Click **Save & Run**.
        

### Related Topics

-   [Adding Alternate Depreciation Methods Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html)
-   [Manually Editing Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150682.html)
-   [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html)
-   [Updating Asset Records Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148181.html)
-   [Adding Alternate Depreciation Methods Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html)
-   [Manually Editing Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150682.html)
-   [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

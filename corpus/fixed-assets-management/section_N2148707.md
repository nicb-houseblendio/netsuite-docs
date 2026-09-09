---
id: "section_N2148707"
type: "section"
title: "Adding Alternate Depreciation Methods Using CSV Import"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Updating Fixed Assets Management Records > Adding Alternate Depreciation Methods Using CSV Import"
parent: "chapter_N2147919"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html"
anchors: ["procedure_N2148735"]
sha256: "86d7deb1e5eeda0cee838307ec379a009f6645954c79a921b0c06284e53a72d9"
---

You can use the CSV import Assistant in NetSuite to update alternate depreciation methods assigned to asset records.

Important:

Before you import asset data, it's best to perform a test import. Create a test CSV file with a few assets and review the formatting to ensure that data is imported with correct values.

#### To add alternate depreciation methods to asset records using CSV import: {#procedure_N2148735}

1.  Prepare an Import File by creating a custom view from the existing Fixed Asset list in NetSuite.
    
    1.  Go to Fixed Assets > Lists > Assets.
        
    2.  Click **Customize View**.
        
    3.  Set Criteria to filter the list as necessary.
        
    4.  Choose the fields to be updated and add them to the **Results** subtab of the new custom view.
        
        To see the necessary fields to be imported, read [Creating FAM Alternate Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2153972.html).
        
        Important:
        
        The Asset's NetSuite Internal ID is required to link the updated information to the correct asset.
        
    5.  Click **Preview**.
        
    6.  Click **Export - CSV** and save the CSV file.
        
2.  On Fixed Assets > Setup > System Setup, make sure that the **Run Server Scripts on CSV Import** box isn't checked. If this box is checked, the **Cumulative Depreciation**, **Last Depreciation Date**, and **Last Depreciation Period** will be set to 0 even if your import file includes the correct amounts. For more information, see [General Guidelines for Importing Fixed Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163350867712.html).
    
3.  Go to Setup > Import/Export > Import CSV Records. In the Import Assistant Step 1 - Scan & Upload CSV File screen:
    
    1.  From the **Import Type** list, select **Custom Records**.
        
    2.  From the **Record Type** list, select **FAM Alternate Depreciation**.
        
    3.  Select the CSV file to upload.
        
    4.  Click **Next**.
        
4.  In the Import Assistant Step 2 - Import Options screen:
    
    1.  Set Data Handling to **Add**.
        
    2.  Click **Next**.
        
5.  In the Import Assistant Step 4 - Field Mapping screen:
    
    1.  Map the fields in your CSV file to the NetSuite fields.
        
        -   Set the Internal ID mapping type to **Internal ID**.
            
            ![Setting the Reference Type to Internal ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ImportCSVMappingInternalID.png)
        -   Review the CSV fields and NetSuite fields to ensure that all required fields are mapped.
            
    2.  Click **Next**.
        
    
    **Example: CSV values**
    
    ![Sample CSV values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ImportAlternateDepreciationSampleCSV.png)
    
    **Example: Mapping**
    
    ![Sample field mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ImportAlternateDepreciationMapping.png)
6.  In the Import Assistant Step 5 - Save Mapping and Start Import screen:
    
    1.  Enter an Import Map Name and Description.
        
    2.  Click **Save & Run**.
        

### Related Topics

-   [Updating Asset Records Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148181.html)
-   [Adding Alternate Depreciation Methods Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html)
-   [Manually Editing Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150682.html)
-   [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html)
-   [Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862707730.html)
-   [Adding Tax Depreciation Methods to an Asset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141463.html)
-   [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html)

### Related Topics

-   [Updating Asset Records Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148181.html)
-   [Adding Alternate Depreciation Methods Using CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2148707.html)
-   [Manually Editing Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150682.html)
-   [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html)
-   [Field Changes That Trigger an Asset Reset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1201080802.html)
-   [Asset Reset Process Stages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1201080808.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

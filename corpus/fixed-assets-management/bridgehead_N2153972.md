---
id: "bridgehead_N2153972"
type: "bridgehead"
title: "Creating FAM Alternate Depreciation"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Creating Fixed Assets Management Records > Creating Asset Records Manually > Depreciation History Subtab > Creating FAM Alternate Depreciation"
parent: "bridgehead_N2154557"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2153972.html"
anchors: ["procedure_N2154012"]
sha256: "489532496a1abe739fbaf2b5ffee61c09c30cf7a8bafcd87911e59cbc6734e1d"
---

The Method sublist in the Depreciation History subtab lets you view each alternate method defined on the asset record, and add new ones.

Note:

The **Store History** box is checked by default.

#### To add alternate methods to a new asset record: {#procedure_N2154012}

1.  Go to Fixed Assets > Lists > Assets, and then click the **View** link of the asset.
    
2.  On the FAM Asset page, click the **Depreciation History** subtab, and then click **New FAM Alternate Depreciation**.
    
3.  Select field values. Most of the fields are automatically populated.
    
    Note:
    
    If the **Override Flag** is checked in the Alternate Method record, you can edit the **Depreciation Method**, **Convention**, **Asset Life**, **Financial Year Start**, and **Period Convention** fields when you add this tax method to an asset. For information about Alternate Method fields, see [Creating Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140809.html).
    
    -   **Alternate Method** - Select a tax method name from the list (or click the + icon) to open a New FAM Alternate Methods record and create a tax method. See [Creating Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140809.html).
        
        Note:
        
        The list shows only alternate methods that match the asset's **Subsidiary** on the **General** subtab.
        
    -   **Depreciation Method** - By default, this is set to the depreciation method defined in the selected Alternate Method.
        
    -   **Original Cost** - Sourced from the Asset record.
        
    -   **Current Cost** - Sourced from the Asset record.
        
    -   **Residual Value Percentage** - Sourced from the Asset record.
        
    -   **Residual Value (RV)** - Sourced from the Asset record.
        
    -   **Asset Life (AL)** - Sourced from the Alternate Method record.
        
    -   **Book Value (NBV)** - Sourced from the Asset Current Cost.
        
    -   **Cumulative Depreciation** - Set to zero by default.
        
    -   **Asset Status** - Select the status of this tax method.
        
4.  Under the **General** subtab, enter values for the following fields:
    
    -   **Subsidiary** - Sourced from the Asset record.
        
    -   **Depreciation Start Date** - Shows the date the tax method starts depreciating.
        
    -   **Depreciation End Date** - The expected end date of the asset's depreciation. By default, this is set to the asset's depreciation start date plus its useful life.
        
    -   **Last Depreciation Date** - The most recent depreciation date of this tax method.
        
    -   **Last Depreciation Amount (LD)** - The asset's most recent depreciation amount. This is set to zero by default.
        
    -   **Last Depreciation Period** - The period number (within the tax method's life) when the asset was last depreciated.
        
    -   **Depreciation Active** - Select whether the asset is active and included in depreciation processing. For assets related to a job, you can set depreciation to automatically start when the job completes. Default set by asset type.
        
    -   **Depreciation Rules** - Select from the following values:
        
        -   **Acquisition** - Asset depreciates in the same period it's activated.
            
        -   **Disposal** - Asset depreciates in its final period.
            
        -   **Pro-rata** - Asset depreciates proportionally for partial months in the acquisition and disposal periods, using a standard 30-day month.
            
        -   **Mid-month** - If the Depreciation Start Date falls within the first half of the month, then depreciation starts on the same month of the asset acquisition. Otherwise, depreciation starts on the month after the asset acquisition month.
            
    -   **Revision Rules** - Select how revaluations affect the asset.
        
        -   **Current Period** - The system recalculates depreciation to date and posts the difference between the calculated depreciation and the previously posted depreciation in the current period.
            
        -   **Remaining Life** - The revision affects only future depreciation calculations.
            
    -   **Financial Year Start** - Sourced from the Alternate Method record.
        
    -   **Annual Method Entry** - Select whether annual depreciation posts on the **Anniversary** (based on the depreciation start date) or the **Fiscal Year** (based on the last day of the fiscal year).
        
    -   **Convention** - Sourced from the Alternate Method record.
        
        Averaging conventions set how depreciation is handled in the asset's first year. Conventions are supported for alternate methods only, and default value is **None**. For monthly depreciation, the supported convention is **Mid-Month**. For annual depreciation, the supported conventions are **Half Year** and **Mid-Quarter**. If the convention is set to Mid-Quarter, the asset depreciates for half of the first quarter, no matter when it entered service.
        
        Note:
        
        If the Convention is **None**, the asset follows the depreciation rule set in the parent asset record. For details on the depreciation rules, see [General Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2151888.html).
        
    -   **Period Convention** - Sourced from the Alternate Method record.
        
    -   **Depreciation Period** - Sourced from the Depreciation Method record.
        
    -   **Prior Year NBV** - Sourced from the Asset Original Cost on the Asset record.
        
        The Prior Year Net Book Value is the asset's net book value for the selected tax method at the end of the previous fiscal year. The **Financial Year Start** field on the Alternate Method record determines the method's start and end of the year. The Prior Year NBV updates when the depreciated month for an Alternate Method (tax method) matches the **Financial Year Start** month. This captures the NBV as it stood for the financial year that ended.
        
    -   **Group Depreciation** - Sourced from the Alternate Method record.
        
    -   **Group Master** - You can check this box only if **Group Depreciation** is checked.
        
    -   **Allow Override** - Sourced from the Alternate Method record. If this box is checked, you can edit the Depreciation Method, Convention, Asset Lifetime, Financial Year Start, and Period Convention.
        
5.  Click **Add** to attach the alternate method to the asset. You can add as many tax methods as you need.
    
6.  Check **Store History** if you want to keep depreciation history records. Otherwise, clear the box.
    
    Important:
    
    Checking the **Store History** box affects the depreciation performance.
    
7.  Click **Save**.
    
    For more information about tax depreciation methods, see [Using Tax Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141684.html).
    

For more information about tax depreciation methods, see [Using Tax Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141684.html).

### Related Topics

-   [Creating Asset Records Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689339824.html)
-   [Depreciation History Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2154557.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

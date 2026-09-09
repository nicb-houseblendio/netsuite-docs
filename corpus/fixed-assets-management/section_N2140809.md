---
id: "section_N2140809"
type: "section"
title: "Creating Alternate Methods (Tax Depreciation Methods)"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > Alternate Methods (Tax Depreciation Methods) > Creating Alternate Methods (Tax Depreciation Methods)"
parent: "section_164862707730"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140809.html"
anchors: ["procedure_N2140829"]
sha256: "28c3120e9714032860f6b87ccbcdad50c24f572f0f76c2d75ff529a49b8b6046"
---

You can create multiple alternate methods of asset depreciation for tax reporting. You can also create a group tax depreciation method for a pool of assets.

#### To create a tax depreciation method: {#procedure_N2140829}

1.  Go to Fixed Assets > Setup > Alternate Methods > New.
    
2.  On the New FAM Alternate Methods record, provide values for the following fields:
    
    -   **Name** - Enter a name for this alternate method.
        
    -   **Description** - Enter a description for this alternate method.
        
    -   **Depreciation Method** - Select a depreciation method. You can create a new depreciation method if it's not available in the list. For more information, see [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html).
        
    -   **Convention** - Select the averaging convention to determine how depreciation is handled in the first year of an asset's depreciation. You can only use conventions with alternate methods, and by default, it's set to **None**. If you depreciate monthly, you can use the **Mid-Month** convention. If you depreciate annually, you can use the **Half Year** and **Mid-Quarter** convention. If the convention is set to **Mid-Quarter**, the asset starts depreciating for half of the first quarter, regardless of when it came into service during that period.
        
        Note:
        
        If the Convention is set to **None**, depreciation processing follows the depreciation rule in the parent asset record. For details on the depreciation rules, see [General Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2151888.html).
        
    -   **Asset Life** - Enter the asset's lifetime. Units are determined by the value of the Depreciation Period (monthly or annual) on the Depreciation Method.
        
    -   **Financial Year Start** - Select the first month of the financial year.
        
    -   **Subsidiary** - Select the subsidiaries for this alternate method. To select multiple subsidiaries, press and hold the Ctrl key and click each subsidiary.
        
        Important:
        
        To avoid issues with depreciation schedules, you must set a value for the subsidiary. Add any new subsidiary to applicable Alternate Depreciation Method and to the asset type's Other Method records.
        
    -   **Pool Flag** - Check this box to use this method to depreciate a group of assets. For more information, see [Group Tax Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2158836.html).
        
    -   **Override Flag** - Check this box to make the Depreciation Method, Convention, Asset Life, Financial Year Start, and Period Convention fields editable when this tax method is added to an asset record.
        
    -   **Derogatory Depreciation** - Check this box to use method to recognize the French Derogatory Depreciation method.
        
        Note:
        
        This option is available if the **Enable Derogatory Depreciation** preference is checked in the FAM System Setup page, and if the country or subsidiary of the tax method is set to France.
        
    -   **Period Convention** - Select the convention that is used to define a year:
        
        -   **12 months of 30 days each** - This convention is generally used in North America and Europe, and produces a more uniform monthly depreciation.
            
        -   **Exact number of days in a month, year has 365 days** - This convention is generally used in Australia and New Zealand and produces uneven depreciations within the year.
            
3.  Click **Save**.
    

The tax method that you created becomes available for selection in the **Alternate Method** field on the asset record's **Depreciation History** subtab.

For information about using group tax depreciation methods, see [Using Tax Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141684.html).

### Related Topics

-   [Fixed Assets Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126441.html)
-   [Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862707730.html)
-   [Viewing or Editing Alternate Methods (Tax Depreciation Methods)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141236.html)
-   [Adding Tax Depreciation Methods to an Asset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141463.html)
-   [Using Tax Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2141684.html)
-   [Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862696596.html)
-   [Creating Asset Records Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689339824.html)
-   [Asset Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2162621.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

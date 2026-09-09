---
id: "bridgehead_N2142565"
type: "bridgehead"
title: "Asset Type Other Methods Subtab"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > FAM Asset Types > Asset Type Other Methods Subtab"
parent: "section_164862669287"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142565.html"
anchors: ["procedure_N2142578"]
sha256: "e87c96651116691ad937eb1a209798becddae75354a7c38ec05e2da7b55c3fad"
---

Note:

The Other Methods subtab is available on the Asset Type record when the asset type has been created.

On the Other Methods subtab, you can assign default alternate depreciation (for analysis only) to the asset, with different asset lifetimes and residual values. This lets you track tax or corporate reporting methods on the asset. These values are calculated automatically during asset depreciation but don't generate financial transactions.

#### To add an alternate depreciation method to an asset type: {#procedure_N2142578}

1.  Go to Fixed Assets > Setup > Asset Type.
    
2.  Click the **View** or **Edit** link next to the asset type.
    
3.  On the Other Methods subtab, click **New FAM Default Alt Depreciation**.
    
4.  On the FAM Default Alt Depreciation page, select an **Accounting Book** and **Alternate Method**. The available methods include only those that you've set up in Fixed Assets > Setup > Alternate Methods.
    
    When you select an Alternate Method, the other fields are automatically populated:
    
    -   **Depreciation Method** - Sourced from Alternate Method record.
        
    -   **Convention** - Sourced from Alternate Method record.
        
        Averaging conventions determine how depreciation is handled in the first year of an asset's depreciation. You can only use conventions with alternate methods, and by default, it's set to None. If you depreciate monthly, you can use the **Mid-Month** convention. If you depreciate annually, you can use the **Half Year** and **Mid-Quarter** convention. If the convention is set to Mid-Quarter, the asset starts depreciating for half of the first quarter, regardless of when it came into service during that period.
        
        Note:
        
        If the Convention value is set to None, depreciation follows the depreciation rule selected in the parent asset record. For details on the depreciation rules, see [Asset Type General Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142208.html).
        
    -   **Asset Life** - Sourced from Alternate Method record.
        
    -   **Financial Year Start** - Sourced from Alternate Method record.
        
    -   **Period Convention** - Sourced from Alternate Method record.
        
    -   **Depreciation Period** - Sourced from Depreciation Method record.
        
    -   **Subsidiary** - Sourced from the Alternate Method record.
        
    -   **Residual Percentage** - Must be entered in the Other Methods of the Asset Type.
        
5.  Click **Save**.
    

### Related Topics

-   [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html)
-   [FAM Asset Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164862669287.html)
-   [Asset Type General Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142208.html)
-   [Asset Type Accounts Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142366.html)
-   [Asset Type Maintenance Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142485.html)
-   [Asset Type Lifetimes Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2142773.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

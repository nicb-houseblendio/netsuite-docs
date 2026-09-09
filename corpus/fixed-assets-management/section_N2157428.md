---
id: "section_N2157428"
type: "section"
title: "Asset Creation"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Creating Fixed Assets Management Records > Creating Asset Records from Transactions > Asset Creation"
parent: "section_164689333704"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2157428.html"
anchors: []
sha256: "66f94fc9da7d9de23cbb4b745f55594984bb909aa41a015dc8fe76dcdc4574e4"
---

The Asset Creation feature in the Fixed Assets Management SuiteApp lets you create assets without proposing them first.

When you use Asset Creation, you can specify the start and end dates of the transactions for which you want to create an asset. However, you won't be able to select individual transactions to generate asset records.

#### To create asset records:

1.  Go to Fixed Assets > Transaction > Asset Creation.
    
2.  On the Asset Creation page, enter values for the following fields:
    
    -   **Date Range** - Select a date range. The system calculates the start date based on the selected range and end date.
        
        Note:
        
        The system sets the date range to **Custom** if you change the Start Date or End Date.
        
    -   **Start Date** and **End Date** - Enter the date of the transactions for which you want to create an asset record. The search retrieves transactions dated within the specified range.
        
    -   **Subsidiary** - Select the subsidiary of the transactions that you want to create assets for.
        
    -   **Include Children** - Check this box to search transactions within the child subsidiaries of the selected subsidiary.
        
    -   **Asset Types** - In the Asset Types sublist, select one or more asset types.
        
        You can't add an asset type that has the same operating lease and account name as another asset type on the list.
        
        Note:
        
        The system proposes operating lease journals only for asset types tagged as **Operating Lease**.
        
3.  Click **Create Assets**.
    
    The system automatically creates asset records for every transaction that matches the filters and posts to the fixed asset general ledger accounts.
    
    You'll be redirected to the Process Status page, where you can track the asset creation's status. For more information, see [Asset Creation Process Stages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1120063923.html).
    

Asset Creation doesn't process assets that are already proposed. To create asset records for proposed assets, use the Generate Assets option (Fixed Assets > Transactions > Asset Proposal). For more information, see [Asset Proposal and Generation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2155572.html).

You can combine assets to create parent-child relationships between asset proposal records and to track them as a single asset. For more information, see [Multiple Asset Proposal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2157628.html).

Note:

Asset Creation no longer captures assets created from transactions that transfer assets across asset types. For more information, see [Restricting the Editing of Asset Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2150936.html).

### Related Topics

-   [Fixed Assets Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126441.html)
-   [Creating Asset Records Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689339824.html)
-   [Creating Asset Records from Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689333704.html)
-   [Asset Proposal and Generation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2155572.html)
-   [Multiple Asset Proposal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2157628.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

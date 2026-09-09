---
id: "section_N2157628"
type: "section"
title: "Multiple Asset Proposal"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Creating Fixed Assets Management Records > Creating Asset Records from Transactions > Multiple Asset Proposal"
parent: "section_164689333704"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2157628.html"
anchors: ["bridgehead_N2157656", "bridgehead_N2157683", "bridgehead_N2157711"]
sha256: "4029e05725ebae98f90f20f571243c5eeee1a238962f39e310c25ce506119d9b"
---

Within the Fixed Assets Management SuiteApp, the asset proposal process searches for new transactions and identifies potential assets. Sometimes, multiple components need to be combined and tracked as a single asset.

You can edit an asset proposal and select a parent proposal to create a parent-child relationship between proposal records.

#### To add a parent proposal to an asset proposal record:

1.  Go to Fixed Assets > Transactions > Manage Asset Proposal.
    
    Note the ID of the proposal record that you want to set as the parent.
    
2.  In the Proposed Assets sublist, click **Edit** next to the proposal you want to set as the child.
    
3.  In the **Parent Proposal** field, select the ID of the parent proposal record.
    
4.  In the **Asset Description** field, update the description to show this asset's relationship to the parent proposal.
    
5.  Click **Save**.
    
    You can also update the parent's description to describe the combined entity.
    
    ## Parent Proposal {#bridgehead_N2157656}
    
    ![images/ParentProposal.png](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ParentProposal.png)
    
    The child proposal record no longer appears on the Proposed Assets sublist. You can find the child proposal on the Subproposal tab of the parent proposal record.
    
    ## Child Proposal {#bridgehead_N2157683}
    
    ![Details of the child proposal record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/ChildProposal.png)
    
    When you generate assets from the parent proposal, the child proposal's value is added to the parent. The system creates a single asset record using the parent record's description and other details.
    
    ## Combined Asset Proposal {#bridgehead_N2157711}
    
    ![Details of the combined proposal record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FixedAssetsManagement/CombinedProposal.png)

### Related Topics

-   [Fixed Assets Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126441.html)
-   [Creating Asset Records Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689339824.html)
-   [Creating Asset Records from Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164689333704.html)
-   [Asset Proposal and Generation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2155572.html)
-   [Asset Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2157428.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

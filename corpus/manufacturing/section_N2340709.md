---
id: "section_N2340709"
type: "section"
title: "WIP and Inventory Costing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > WIP and Inventory Costing"
parent: "chapter_N2335392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340709.html"
anchors: ["bridgehead_N2340735", "bridgehead_N2340863", "procedure_N2340876", "procedure_N2340902"]
sha256: "002b26723389a32bb87aad4d11b9fb1bb636241f5f4bb5faf9643f889625d781"
---

Only assemblies using standard cost and average cost are compatible with the Manufacturing Work In Process (WIP) feature. Assembly component members can use LIFO/FIFO, standard, average, or actual costing. Assemblies using LIFO/FIFO/specific costing aren't compatible with this feature.

Standard cost assemblies have costs calculated based on the WIP account indicated for the order, not by date.

## Standard Cost Assembly Revaluations {#bridgehead_N2340735}

The standard cost of raw materials can change when a work order is still in process causing a change in the WIP valuation.

For example:

-   A bicycle wheel is made of the following component parts: rims, tires, and spokes.
    
    -   Rims cost $5.
        
    -   Tires cost $6.
        
    -   Spokes cost $7.
        
    -   The total bicycle wheel cost is $18.
        
-   When a work order is still in process, the standard cost of components changes to the following:
    
    -   Rims cost $4.
        
    -   Tires cost $5.
        
    -   Spokes cost $6.
        
    -   The total bicycle wheel cost is $15.
        
-   The change in the bicycle wheel cost from $18 to $15 requires the following WIP cost adjustment:
    
    -   (-1) for each component issued
        
    -   (-3) for each assembly taken out of the WIP location
        

When the standard cost for an inventory or assembly item in a location changes, note the following. NetSuite creates a separate standard cost revaluation transaction for each partially built work order. NetSuite creates standard cost revaluation transactions for each work order that doesn't have a status of Released or Built.

## Posting GL Lines for a WIP Assembly Completion with Backflush {#bridgehead_N2340863}

When you enter an assembly completion with backflush, you log the assembly completion and component consumption at the same time. This transaction posts to the general ledger as follows:

## Cost of the Assembly {#procedure_N2340876}

-   For an average cost item, an estimate of the last purchase price is used for the assembly posting.
    
-   For a standard cost item, the standard cost is posted.
    

## Cost of a Component {#procedure_N2340902}

-   For an actual cost item or average cost item, the average or actual cost from the warehouse location is posted.
    
-   For a standard cost item, the standard cost for component is posted.
    

Note:

If you use WIP, an average cost assembly item generates a variance based on the assembly cost and the component cost. If an adjustment needs to be made on the average cost based on the variance, you should use an inventory adjustment worksheet.

### Related Topics

-   [Enabling the WIP Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335702.html)
-   [Setting Default WIP Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607056275.html)
-   [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)
-   [Associating Components with Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4165324435.html)
-   [Entering a Completion for an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339540.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

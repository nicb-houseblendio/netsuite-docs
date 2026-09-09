---
id: "section_N2334515"
type: "section"
title: "Revision Control BOM Management"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Bill of Materials Member Control for Assembly Items > Setting Up BOM Control on Assembly Item Records > Revision Control BOM Management"
parent: "section_N2334154"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334515.html"
anchors: ["bridgehead_N2334682", "procedure_N2334697"]
sha256: "7a3babd021d68c71eec17f6e6393ccffd2932515f018663a0abe11e61ac118b9"
---

To manage the Bill of Materials (BOM) for assembly items, use Revision Control as your Effective BOM Control method. This method simplifies effective and obsolete date management. To use revision control, create revision records that define an effective date or an obsolete date. The revision records you assign to assembly members determine their effective and obsolete dates.

The Revision Control method enables you to set the effective or obsolete date for many items at one time by updating one revision record. When several items use a revision record, date changes can be made on the revision record rather than individually for many member items. Rather than changing the dates on every line item, you change only the effective or obsolete date in the revision record.

For assembly items that use Revision Control, create revision records to define effective and obsolete dates. The assembly effective and obsolete dates are determined by the assigned revision record.

Revision records can be created in two ways:

-   As individual records. For more information, see [Creating Revision Records for BOM Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335150.html).
    
-   From assembly record Members subtab. For more information, see [Setting an Assembly to Use Revision Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334812.html).
    

After a revision is assigned to an assembly member, you can enter a new work order and select the assembly. The correct revision defaults to based on the work order production date. The work order item list displays the correct set of member components based on the revision used.

-   If you select a new revision, the item list updates to show the correct member items.
    
-   If you change the date, NetSuite updates the revision to the one which is effective for that date.
    

To use only the assembly default revision, on the work order form, click Customize and then make the field not selectable

-   Edited revision record effective or obsolete dates are not retroactive. Previously entered transaction data using that revision remain unchanged.
    
-   BOMs created for individual assembly builds compare the transaction date to the effective and obsolete dates.
    
-   On an assembly unbuild, select a revision to determine the BOM. The default revision for an unbuild is based on the current date.
    
-   BOM costs using Standard Costing are based on the effective date shown on the planned standard cost rollup record.
    

Note:

If you use the Matrix Items feature, you cannot set the Effective BOM Control to Revision Control on a matrix parent item. However, you can set the Effective BOM Control to Revision Control on a matrix subitem.

## On Work Orders {#bridgehead_N2334682}

NetSuite automatically populates the work order effective revision based on the effective date. If you change the work order, NetSuite changes the components on the top level assembly based on the revision selected.

If you change the work order revision and the Build Subassembly box is checked, top-level components change based on the selected revision. The lower level components are determined based on the effective date.

## Demand Planning {#procedure_N2334697}

When demand increases for member items from a parent assembly, NetSuite reviews the work order start date to determine demand for those member items. For example, the Mountain Bike component items include the following:

-   Brake Item 1: has an effective date of 4/1/2020
    
-   Brake Item 2: has obsolete date of 3/31/2020
    

Demand for the item requires a work order to be created on 3/20 and one on 4/20. Therefore, the first work order uses the Member Item 2, and the second one will use Member Item 1. This is relevant if the member items are assemblies that need to have work orders created for them.

### Related Topics

-   [Using Effective Date BOM Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161589846245.html)
-   [Setting Up BOM Control on Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334154.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

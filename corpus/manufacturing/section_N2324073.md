---
id: "section_N2324073"
type: "section"
title: "Bill of Materials Inquiry"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items > Bill of Materials Inquiry"
parent: "chapter_N2319010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html"
anchors: ["procedure_N2324095", "bridgehead_4255954032"]
sha256: "361c8fa93c6efa8ce3bac9367f0c78d8d3d5309a60b81131746f3a0bc3ecc2e7"
---

If you use Assembly Items, the Bill of Materials (BOM) Inquiry enables you to see the build requirements for an assembly item. The BOM Inquiry displays the member components of the assembly, and the number of each component needed for each assembly.

For example, you can run BOM Inquiry to identify the materials needed to assemble a Mountain Bike. The inquiry shows that you need two wheels, one frame, one seat, and one handle bar. The inquiry also shows the sub-assembly (phantom assembly) components for each wheel: one rim, one hub, one, tube, one tire, and spokes.

Note:

Custom roles must specify access to view this inquiry. For more information, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

#### To run a Bill of Materials Inquiry: {#procedure_N2324095}

1.  Go to _Transactions > Manufacturing > Bill of Materials Inquiry_.
    
2.  Select the assembly you want to show a BOM for.
    
3.  If you use the multi-location inventory feature, select a **Location** to view data for that location.
    
    Required fields display a red asterisk (**\***).
    
    If you use Advanced BOM, see [Running a BOM Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498757236.html).
    
4.  Choose a level of detail:
    
    -   Check the **Top Level Only** box to show only the top level member items details (sub-assembly information isn't shown).
        
    -   Clear the **Top Level Only** box to show details about all levels of member items.
        
5.  In the **BOM Display Control** list, select **By Date** or **By Revision** to decide what to include in an assembly.
    
    Note:
    
    This field is available only when an assembly item uses Revision Control for its Effective BOM Control value.
    
    When assembly items use Effective Date as Effective BOM Control value, the **Date** field determines the date when querying components of the assembly item.
    
    Components are displayed based on the following criteria:
    
    -   Selected date is greater than or equal to the effective date.
        
    -   Selected date is less than or equal to the obsolete date.
        
    
    If an assembly item uses Revision Control, you can query the components either By Date or By Revision.
    
    -   If you select **By Date**, then follow the process described in step 5 above.
        
    -   If you select **By Revision**, in the **Revision** field, select a revision.
        
        The active components for the revision are displayed and the date field displays the revision effective date.
        

The inquiry displays all components used in a multi-level bill of materials structure, using a nested tree view.

The Bill of Materials Inquiry displays the following items:

| **Column Label** | **Explanation** |
| --- | --- |
| **Component Name** | The name of the Component as defined in the Item Name field |
| **Level** | Where the component appears on the BOM tree structure |
| **Component Yield** | Shows how much of this component is available for final assembly, after accounting for loss/scrap in the production process A yield factor of 0.9 means that 90% of the usage quantity of the component on a bill becomes part of the finished assembly. |
| **BOM Quantity per Assembly** | The quantity required for this assembly according to the BOM |
| **Quantity per Assembly** | The quantity required when component yield is taken into consideration |
| **Quantity per Top Level Assembly** | The total quantity of this component required to make the top-level assembly Top level items are typically finished products. For example, a Barbecue grill set. |
| **On Hand** | Number of items physically held at the specified location |
| **Available** | Uncommitted stock of item |
| **Back Ordered** | The quantity of any unfulfilled order or existing commitment for this component |
| **On Order** | The total quantity ordered of this component across all current work orders |

To display information stored in custom item fields for each component, click **Customize**.

## Export or Print a Bill of Materials Inquiry {#bridgehead_4255954032}

For more flexibility to work with data outside of NetSuite, you can print or export the results of a Bill of Materials Inquiry.

Click the printer icon at the top of the inquiry page to print or export (Excel or CSV) the inquiry results.

Note:

The data in the inquiry header (such as location and date) isn't exported. Only the table data resulting from the inquiry is exported. Only the columns shown on the query export page can be exported or printed.

For more information, see [Printing an Item Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323540.html) for an alternate way to view BOM details.

### Related Topics

-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Enabling Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319428.html)
-   [Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319594.html)
-   [Assemblies on Purchase Transactions, Web Sites, and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161487042976.html)
-   [Matrix Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4249789892.html)
-   [Phantom Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4714298883.html)
-   [Assemblies and Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2320172.html)
-   [Building Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html)
-   [Unbuilding Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321882.html)
-   [Marking Work Orders Built](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2322811.html)
-   [Printing an Item Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323540.html)
-   [Costed Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160730538.html)
-   [Printing Assembly Item Materials on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324339.html)
-   [Printing Assembly Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324547.html)
-   [Running the Component Where Used Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511882961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

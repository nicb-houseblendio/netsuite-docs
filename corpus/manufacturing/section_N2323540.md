---
id: "section_N2323540"
type: "section"
title: "Printing an Item Bill of Materials"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items > Printing an Item Bill of Materials"
parent: "chapter_N2319010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323540.html"
anchors: ["procedure_N2323875"]
sha256: "8e72f53d2683e5fe530f4e14defa4591b5a4af3c823babea2d1bc31bd38716b5"
---

A Bill of Materials (BOM) lists all the components of your assembly item, the assembly quantity, and the total quantity for each.

If one of the components of your assembly item is an assembly item, each item subcomponent appears. Each subcomponent displays the quantity needed for each subcomponent to complete the assembly.

For example, your assembly item contains four components-Item A, Item B, Item C, Item D. Item B is an assembly item made up of Widget 1 and Widget 2. Two of each widget are necessary for assembly of Item B. And two of Item B are needed to complete the parent assembly. The quantity needed to complete assembly Item B must be doubled to complete the parent assembly.

The following table displays the assembly bill of materials:

| Parent Assembly |
| --- |
| Name | Assembly Quantity | Total Quantity |
| --- | --- | --- |
| **Item A** | 1 | 1 |
| **Item B** | 2 | 2 |
| **Widget 1** | 2 | 4 |
| **Widget 2** | 2 | 4 |
| **Item C** | 5 | 5 |
| **Item D** | 1 | 1 |

#### To print a bill of materials for an assembly item: {#procedure_N2323875}

1.  Go to _Lists > Accounting > Items_.
    
2.  To open the **Filters** section, click the + icon.
    
3.  In the **Type** field, select **Assembly** to filter your item list to show assembly items.
    
4.  Click **View** next to the item you want to print the bill of materials (BOM) for.
    
5.  To print the BOM, click the **Print** icon.
    
6.  When the window containing your BOM opens, click the **Print** ![Print button icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Manufacturing/PrintButton.png) icon.
    
    You can also click **Export** in this window to open or save your BOM as a CSV file.
    

To learn another way to view BOM details, see [Bill of Materials Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html).

To learn how to print a bill of materials for work orders that you enter, see [Printing a Work Order Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331127.html).

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
-   [Bill of Materials Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html)
-   [Costed Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160730538.html)
-   [Printing Assembly Item Materials on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324339.html)
-   [Printing Assembly Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324547.html)
-   [Running the Component Where Used Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1511882961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2331127"
type: "section"
title: "Printing a Work Order Bill of Materials"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Work Orders > Printing a Work Order Bill of Materials"
parent: "chapter_N2328390"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331127.html"
anchors: ["procedure_N2331157", "procedure_N2331215", "bridgehead_N2331449"]
sha256: "1e150300b1afe51163495b838f2ff872c087727c0407db13d83e0c50f4ad097c"
---

For work orders you have entered, you can print a Bill of Materials (BOM). The BOM shows the types and quantities of items you need to complete the work order.

Following are the two ways to print a BOM.

#### Print from the work order: {#procedure_N2331157}

1.  Go to _Transactions > Manufacturing > Enter Work Orders > List_.
    
2.  Click **View** next to the work order.
    
3.  On the work order, click **Print BOM**.
    
    Only information from the header of the work order appears in the BOM. If you want to print assembly details of the work order, you must open the assembly item record and click **Print**.
    

#### Print from the print queue: {#procedure_N2331215}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Bill of Materials**.
    
3.  In the **Filter By** field, choose one of the following to filter the work orders shown:
    
    -   **Some Items Committed** - The list shows orders that have one or more items committed to be built.
        
    -   **All Items Committed** - The list shows orders that have all items committed to be built.
        
    -   **Ignore Item Availability** - The list shows all open orders regardless of the availability.
        
4.  Select a location to filter the list for orders for that location.
    
5.  Select a form to use for this print run.
    
    This field defaults to the preferred form, but you can choose a form you have previously customized.
    
    If you are printing packing slips and use the Advanced Shipping feature, you can also use a custom invoice form when printing packing slips. For example, you can customize an invoice form to show the item rate and amount, and the order total. Then, when you print the packing slip using the custom form, the packing slip shows the additional information.
    
    To customize a form, go to _Customization > Forms > Transaction Forms_. Click **Customize** next to the appropriate form.
    
6.  The **Documents in Queue** field shows the number of forms you have selected to print. This field updates as you check bills of materials to print.
    
7.  Check the **Allow Reprinting** box to reprint previously printed transactions.
    
    When you check this box, all documents appear at the bottom of the page in segments. Clear this box to allow documents to be printed only one time.
    
    Note:
    
    The work order tracks whether a bill of materials has been printed. It resets this flag whenever components are committed so that new top-level assemblies may be built.
    
8.  Click the **Select Order Number** field to enter or scan in transaction bar codes.
    
9.  Check the box in the **Print** column next to each order you want to print a bill of materials for.
    
10.  Click **Print**.
     

The bill of materials prints in two sections:

-   **Section One: Bill of Materials**
    
    This section is a complete list of all items needed to complete the build for the work order. It shows the specific items and the quantity needed for each, including components of assembly members.
    
-   **Section Two: Assembly Hierarchy**
    
    This section shows how many of each component are needed for each unit.
    

![Screenshot of a sample Bill of Materials.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Manufacturing/BOM.jpg)

## Print Instructions with the Bill of Materials {#bridgehead_N2331449}

If you print your BOM in PDF format, you can append the PDF file to print additional materials with the BOM. For example, you can print a diagram or instructions about the assembly process for the top level assembly item. For more information, see [Appending a PDF File to Print with the Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331613.html).

An alternative way to view and print the BOM is by using the [Bill of Materials Inquiry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2324073.html).

### Related Topics

-   [Two Types of Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161538863125.html)
-   [Enabling the Work Orders Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161538373436.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)
-   [Mass Creating Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330082.html)
-   [Marking Assemblies to Create Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330700.html)
-   [Planned Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3872474232.html)
-   [Component Yield Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727093231.html)
-   [Editing a Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331050.html)
-   [Appending a PDF File to Print with the Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331613.html)
-   [Building Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331860.html)
-   [Work Orders and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

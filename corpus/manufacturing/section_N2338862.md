---
id: "section_N2338862"
type: "section"
title: "Entering Work Order Issues"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Using WIP on Work Orders > Entering Work Order Issues"
parent: "section_N2337938"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html"
anchors: ["procedure_N2338916"]
sha256: "12757cab4e007e1abbba29f3473d3bc5079f19e4fb6d9e574a5081f7406d3f95"
---

When you use the Manufacturing Work In Process (WIP) feature, you must issue components to start work order processing. When you issue components, you are logging only the material consumption, not any work on the assembly process.

The work order issue indicates the material is consumed against the work. Issue assembly member components to track material consumption or log service against a work order.

After components are issued, the material value is recorded in the assigned WIP account. You can issue components for many work orders at one time.

If you use the Multiple Units of Measure feature, the issued component quantity is recorded in base units.

#### To bulk enter work order issues: {#procedure_N2338916}

1.  Go to _Transactions > Manufacturing > Issue Components_.
    
2.  If you use NetSuite OneWorld, select a **Subsidiary** from the list.
    
3.  Optionally select the following to filter the list of work orders:
    
    -   **Item**
        
    -   **Customer**
        
4.  Select the **Posting Period**.
    
5.  Select the **Date** for this issue transaction.
    
6.  Select a **Location** from the list.
    
    Location is displayed in the location field in the header of all work order issues.
    
7.  Select a **Filter By** option:
    
    -   **Some Items Committed** - Displays the committed quantity
        
    -   **All Items Fully Committed** - Displays the committed quantity
        
    -   **Ignore Commitment** - Displays the remaining quantity
        
8.  Check the **Issue** box next to all work orders you want to create issues for.
    
9.  Click **Submit**.
    
    After the page is submitted, the work order issues are generated for all marked orders.
    

After you issue components for an order, you can enter a work order completion against it to log the finished assemblies. For more information, see [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html).

### Related Topics

-   [Issuing Components for an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607524041.html)
-   [Entering Work Order Closes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

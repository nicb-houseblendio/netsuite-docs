---
id: "section_N2339540"
type: "section"
title: "Entering a Completion for an Individual Work Order"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Entering a Completion for an Individual Work Order"
parent: "chapter_N2335392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339540.html"
anchors: ["procedure_N2339550"]
sha256: "6cc4e08ccddb2e09b29a88d8c22fe043683441865a4ecd066429d010eb105505"
---

You can enter a completion for a single work order.

#### To enter individual work order completions: {#procedure_N2339550}

1.  Go to _Transactions > Manufacturing > Enter Work Orders > List_.
    
2.  Click **View** next to the work order you want to complete.
    
3.  Do one of the following:
    
    -   To create a work order completion without backflush, click the **Enter Completion** button.
        
        The completion records the number of assemblies completed against a work order. It doesn't record component consumption.
        
    -   To create a work order completion with backflush, click the **Enter Completion with Backflush** button.
        
        This records completion and component consumption.
        
        Important:
        
        If you use Manufacturing Routing and Work Centers, when you enter a completion with backflush, you must complete additional steps. See [Entering a Completion With Backflush](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607563571.html).
        
4.  On the **Work Order Completion** page, enter a **Reference #** (number).
    
5.  To enter the completions with backflush, check the **Backflush** box.
    
    Backflush enables component consumption to be recorded at the same time. Component consumption is based on the proportion designated on the original work order and the build quantity.
    
6.  Select the issue transaction **Date**.
    
7.  Select the **Posting Period**.
    
8.  Optionally, enter a **Memo**.
    
9.  After you enter a quantity to build, click **Inventory Detail** to specify a bin, serial or lot number for the items being processed.
    
    If you use Multiple Units of Measure, the Units field on the Inventory Detail record defaults to base units and cannot be changed.
    
10.  Select a **Department** or **Class** if you track them.
     
11.  Select a **Location**.
     
12.  If you are entering a completion with backflush, verify or enter the **Completed Quantity** of each component consumed.
     
13.  Click **Save**.
     

### Related Topics

-   [Enabling the WIP Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335702.html)
-   [Setting Default WIP Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607056275.html)
-   [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html)
-   [Using WIP on Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html)
-   [Associating Components with Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4165324435.html)
-   [WIP and Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340709.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

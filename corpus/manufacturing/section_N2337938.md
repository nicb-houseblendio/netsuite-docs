---
id: "section_N2337938"
type: "section"
title: "Using WIP on Work Orders"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Work In Process (WIP) > Using WIP on Work Orders"
parent: "chapter_N2335392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2337938.html"
anchors: ["procedure_N2337957"]
sha256: "1b2a50ba6201b3c805e0c7ed4746f8e7b15e6d879ac9f077cd4d3f352e1dd19d"
---

The following procedure provides instructions for using WIP on work orders.

#### To use WIP on a work order: {#procedure_N2337957}

1.  Go to _Transactions > Manufacturing > Enter Work Orders_.
    
2.  Complete the fields, as required.
    
3.  To use WIP **rather than a standard assembly build** on this work order, check the **WIP** box.
    
    Note:
    
    You cannot clear the WIP box after a posting assembly transaction has been attributed to this work order.
    
4.  Select a **Location**.
    
    This field is required for WIP work orders.
    
5.  Complete the necessary form fields. For more information, see [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html).
    
6.  Click **Save**.
    

After you designate a work order as WIP, complete the build process using the following:

-   **Work Order Issue** - Issue components to track material consumption or log service against a work order.
    
    For more information, see [Entering Work Order Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2338862.html).
    
-   **Work Order Completion** - Identify the quantity completed and stocked.
    
    For more information, see [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html).
    
-   **Work Order Close** - Generate reconciliation entries to post variances that may occur during the manufacturing process.
    
    For more information, see [Entering Work Order Closes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html).
    

The following table shows an example of the general ledger impact for WIP transactions:

| **Consumption** |  |  |
| --- | --- | --- |
|  | Component Asset | Location | CR- (credit) |
|  | Component Asset | WIP | DR+ (debit) |
| **Completion** |  |  |
|  | Assembly Asset | Location | DR+ |
|  | Assembly Asset | WIP | CR- |
| **Close** |  |  |  |
|  | Assembly Asset | WIP | DR+ |
|  | Component Asset | WIP | CR+ |
|  | Variances | WIP | DR+ |

### Related Topics

-   [Enabling the WIP Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335702.html)
-   [Setting Default WIP Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161607056275.html)
-   [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html)
-   [Associating Components with Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4165324435.html)
-   [Entering a Completion for an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339540.html)
-   [WIP and Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340709.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

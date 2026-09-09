---
id: "section_N2351557"
type: "section"
title: "Manufacturing Routing Costing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Routing Costing"
parent: "chapter_N2341076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html"
anchors: ["bridgehead_N2351603", "procedure_N2352335", "procedure_N2352728", "bridgehead_4400952267"]
sha256: "8a1300f5bb725174c922da58c92d894534f62aabb9c073b2c09cb6fec1adffd7"
---

Values for assets and expenses associated with a routing work order post to the designated Work In Process (WIP) account during the assembly process.

Values are added to the WIP account based on time logged against operation tasks or quantity produced in a run. After the assembly process completes, the values are removed from the WIP account and added to the Asset for Assembly account.

## Time Updates and Costing {#bridgehead_N2351603}

When time is logged against an operation task for an assembly, NetSuite uses this time to calculate costs associated with the assembly. For example, when completion time is logged against an operation task, NetSuite generates the following accounting entries:

|  | **Account** | **Formula** |
| --- | --- | --- |
| **CR** | Labor | Rate x Resources x Hours |
| **DR** | WIP account for assembly | Rate x Resources x Hours |

-   **Hours** - time logged on a completion record
    
-   **Resources** - sourced from the completion record
    
-   **Rate** - sourced from the operation task record
    

The result of these calculations posts to the WIP account for the assembly. Costs can be one of two types: setup costs or run costs.

## Setup Costs {#procedure_N2352335}

Costs need to be logged for expenses related to setting up for an assembly run. These costs are defined on the operation task record and are based on time logged against the task.

Note:

Setup costs are only time dependent, not based on quantity produced.

For example, the operation task **Staging** defines costs on the Cost Detail subtab. One cost category defined is Labor Setup. Using this category on a task defines the following:

-   The Labor Setup cost category record indicates the item **Other Charge for Purchase - Labor Setup**.
    
-   The task record defines the fixed rate for using the item **Other Charge for Purchase - Labor Setup** at $30 _._
    
-   The item record for **Other Charge for Purchase - Labor Setup** indicates the **Assembly Staging Expense** expense account.
    
    Therefore, when you log time against the **Staging** task, the appropriate amount posts to the **Assembly Staging Expense** account. This amount is calculated as Expense amount = Setup time logged x Labor setup fixed rate.
    
    If 2 hours of time are logged against the **Staging** task, $60 is logged to the **Assembly Staging Expense** account.
    

| **Labor Setup** | **Account** |  |
| --- | --- | --- |
| **CR** | Labor Setup | Rate x Resources x Hours |
| **DR** | WIP account for assembly | Rate x Resources x Hours |

Similar calculations are made for other categories that may be defined on a task record. For example, overheads (Overhead expense amount = Setup time logged x overhead rate).

| **Labor Setup Overhead** | **Account** |  |
| --- | --- | --- |
| **CR** | Labor Overhead Setup Account | Rate x Resources x Hours |
| **DR** | WIP account for assembly | Rate x Resources x Hours |

## Run Costs {#procedure_N2352728}

Costs need to be logged for expenses related to processing an assembly run. These costs are defined on the operation task record and are based on quantity completed during the assembly run.

For example, the operation task **Staging** defines costs on the Cost Detail subtab. One cost category defined is Labor Run. Using this category on a task defines the following:

-   The Labor Setup cost category record indicates the item **Other Charge for Purchase - Labor Run**.
    
-   The task record defines the run rate for using the item **Other Charge for Purchase - Labor Run** at $65 _._
    
-   The item record for **Other Charge for Purchase - Labor Setup** indicates the **Assembly Staging Expense** account.
    
    Therefore, when you log time against the **Staging** task, the appropriate amount posts to the **Assembly Staging Expense** account. This amount is calculated as Expense amount = Setup time logged x Labor setup fixed rate.
    
    If 10 units are completed for the **Staging** task, $650 is logged to the **Assembly Staging Expense** expense account.
    

| **Labor Run** | **Account** |  |
| --- | --- | --- |
| **CR** | Labor Run | Rate x Resources x Hours |
| **DR** | WIP account for assembly | Rate x Resources x Hours |

Similar calculations are made for other categories that may be defined on a task record. For example, overheads (Overhead expense amount = Run quantity logged x overhead rate).

| **Labor Run Overhead** | **Account** |  |
| --- | --- | --- |
| **CR** | Labor Overhead Run Account | Rate x Resources x Hours |
| **DR** | WIP account for assembly | Rate x Resources x Hours |

## Costing Lot Size {#bridgehead_4400952267}

If you use Standard Costing and Manufacturing Routing and Work Center, the Costing Lot Size field appears on the assembly item record's Locations subtab. The default value for this field is 1, and the minimum value for this field is 0.01.

If you also use Multiple Units of measure, the value is in base units of measure.

During the cost rollup process, NetSuite calculates the routing cost of assemblies as follows:

| **Setup Cost** | **Run Cost** |
| --- | --- |
| \# of Resources x Setup Time x Manufacturing Charge Item Unit Cost / Standard Cost Lot Size (assembly item - item location map) Resources are work centers. The Setup Time is from the routing record. Manufacturing Charge Item Unit Cost is from the item record. | \# of Resources (work center) x Run Rate (routing record) x Manufacturing Charge Item Unit Cost (item record) |

### Related Topics

-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Work Center Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3911875603.html)
-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html)
-   [Manufacturing Routing and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html)
-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Supply Planning and Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html)
-   [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html)
-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Work Instructions and Traveler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_9135201182.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

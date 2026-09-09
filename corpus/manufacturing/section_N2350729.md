---
id: "section_N2350729"
type: "section"
title: "Routing Completion Labor and Machine Time Entry"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Routing Completions and Time Entry > Routing Completion Labor and Machine Time Entry"
parent: "section_N2350143"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350729.html"
anchors: ["subsect_161902847126"]
sha256: "9e5ccdfe73eebe30f2951d742f9ddae1b90e3d68414b86936f68cf28d378ea08"
---

Enter a routing work order completion enables you to record labor and machine time completed against an operation task. For more information, see [Routing Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350305.html).

Entering data on the completion form enables you to define the following information:

-   **Starting and Ending Operation** - The completed operation tasks.
    
-   **Quantity Completed** - The amount of time to be logged against each operation.
    

The Operations subtab shows which operations are being completed and the amount of labor and machine time to record against each operation.

#### Identify Completed Operations

1.  Enter the **Starting Operation**.
    
    The first operation task you want to identify as being completed.
    
2.  Enter the **Ending Operation**.
    
    The last operation task you want to identify as being completed.
    
    Operation tasks logged as completed include the indicated starting operation, the ending operation, and all operation tasks in between the starting and ending tasks.
    
3.  Enter the **Completed Quantity**.
    
    NetSuite uses this quantity to calculate the amount of labor and machine time for completed sequences .
    
    Note:
    
    Enter the completed quantity in the Operation Completion section of the form. The Completed Quantity field on the Operations subtab is read-only.
    

For example, enter a completed quantity of 1, with the starting operation of 10, and ending operation of 30.

Operations 10, 20, and 30, the completed quantity is multiplied against the labor and machine time requirements set on the operation task record. The labor and machine time fields on the Operations subtab are populated.

## Labor Time and Machine Time for Completed Operations {#subsect_161902847126}

After the operations marked as complete are identified, you can enter details about labor and machine time for each operation.

The Operations subtab can be used as follows for each operation completed:

-   Completed Quantity displays the amount entered in the Completed Quantity field.
    
-   To record Setup Time:
    
    -   If you haven't recorded an operation setup time against an operation, the setup columns display the full operation setup time. Time is based on the setup time defined on the operation task record.
        
    -   Check the **Record Setup Time** box.
        
        For each operation, you have the following options:
        
        -   Modify the default setup time quantity.
            
        -   Clear the Record Setup Time box.
            
-   NetSuite automatically enters machine and labor run times for each operation based on the quantity completed using the following formula:
    

Default run time = Qty completed x Run rate on the operation record

After the system enters labor and machine times for all completed operation tasks, NetSuite calculates the progress and costs of the assembly.

-   For more information, see [Time and Status Updates on Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351146.html).
    
-   For more information, see [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html).
    

### Related Topics

-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Routing Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350305.html)
-   [Time and Status Updates on Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351146.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

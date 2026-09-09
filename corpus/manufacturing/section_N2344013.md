---
id: "section_N2344013"
type: "section"
title: "Creating Manufacturing Cost Templates"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Setting Up Manufacturing Routing > Creating Manufacturing Cost Templates"
parent: "section_N2341463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html"
anchors: ["procedure_N2344045", "bridgehead_N2344256"]
sha256: "2c4d8e35977a0cbd9d2bba49362b203987081a32f9764f43a5e4ea596f956862"
---

A manufacturing cost template is a list of rates that can be associated with completing a specific operation. The template defines the activities that occur and related costs to be recorded each time this step is completed.

For example, an employee works 10 hours on an assembly activity. A manufacturing operator needs to record the hours worked as a completion for this step. The cost template defines costs associated with the step completed: the rate for each activity, and what accounts these amounts should post to.

A manufacturing cost template streamlines tracking assembly process costs. It provides which rates and accounts are commonly used for each step in an assembly process.

Important:

Including too many cost types on a manufacturing cost template may degrade NetSuite performance. Performance is compounded when multiple cost items aren't related to production.

#### To create a manufacturing cost template: {#procedure_N2344045}

1.  Go to _Lists > Supply Chain > Manufacturing Cost Template > New_.
    
2.  Enter a name for the template.
    
3.  Optionally enter a memo. You can search for text you enter here to find this template later.
    
4.  Check the **Inactive** box if you do not want this template to show in lists on forms and records. Clear this box if you do want this template to show in lists.
    
5.  Select a cost category.
    
    For information about creating a cost category, see [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html).
    
6.  Select an item.
    
    Only items that have been marked as **Manufacturing Charge Items** show on this list.
    
    For more information, see [Defining a Manufacturing Charge Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2343650.html).
    
7.  Enter rates up to 7 decimal places for this line item.
    
    -   If this is a Setup category, enter a fixed rate. This is a one-time charge for a setup activity.
        
    -   If this is a Run category, enter a run rate. This is an amount charged for each run completed.
        
    
    Note:
    
    Template creation performance is negatively affected when the number of lines on the cost templates isn't kept to a minimum.
    
8.  Click **Add**.
    
9.  Repeat steps 5 through 8 for each category. Enter one category for each activity associated with this operational step.
    
    You can add only one of each of the following cost category types: Labor Run, Machine Setup, or Machine Run. However, you can add multiple categories for Overhead cost category types.
    
10.  When all necessary categories have been added, click **Save**.
     

## Cost Template Examples {#bridgehead_N2344256}

A manufacturing cost template shows rates for many possible activities that are associated with an assembly step, such as the examples below:

| **Activity Type** | **Example** | **Rate Type** | **Rate Amount** | **Cost Category** |
| --- | --- | --- | --- | --- |
| **Manufacturing Labor Setup Service** | Warm up molding machine | Fixed | $10 per run | Labor Setup |
| **Manufacturing Labor Setup Overhead** | Facility rental | Fixed | $16 per run | Labor Setup Overhead 1 |
| **Manufacturing Labor Run Service** | Costs to complete one run | Run | $14 per hour | Labor Run |
| **Manufacturing Labor Run Overhead Service** | Electric utility cost per run | Run | $13 per hour | Labor Run Overhead 1 |

### Related Topics

-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Enabling the Manufacturing Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341773.html)
-   [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html)
-   [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html)
-   [Defining a Manufacturing Charge Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2343650.html)
-   [Creating Manufacturing Work Centers or Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344727.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

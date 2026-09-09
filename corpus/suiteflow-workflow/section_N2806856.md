---
id: "section_N2806856"
type: "section"
title: "Welcome Email Sent to Customers Three Days After First Order Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Welcome Email Sent to Customers Three Days After First Order Workflow"
parent: "chapter_N2796642"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html"
anchors: []
sha256: "af0b3dd8df5e1a9f22e4d0ea3d7357f5fab8c8cf621edacbd3e8147eb144ae0a"
---

The following example shows how to create a scheduled workflow to send a "Welcome" email to a customer three days after the customer places an order.

The example uses a custom field, Email Scheduled, on the customer record form to identify if the email has already been scheduled. A saved search identifies customers who have at least one sales order and who have not received the welcome email. The workflow runs the saved search on a daily schedule and sends the email to the customers that meet the saved search criteria.

Note:

If any current customers have existing sales orders, this workflow also sends the welcome email to those customers.

To set up the workflow, complete the following steps:

1.  Create the custom field for the Customer record. For information, see [Step 1 Create the Custom Field for the Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471788460.html).
    
2.  Create the saved search. For information, see [Step 2 Create the Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471788894.html).
    
3.  Create the workflow and set the schedule. For information, see [Step 3 Create the Workflow and Set the Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471789290.html).
    

You can also use these steps to build this process into a larger workflow.

### Related Topics

-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Lead that Did Not Convert to Customer Within Three Days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801202.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

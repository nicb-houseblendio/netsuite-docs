---
id: "section_N2801202"
type: "section"
title: "Lead that Did Not Convert to Customer Within Three Days"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead that Did Not Convert to Customer Within Three Days"
parent: "chapter_N2796642"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801202.html"
anchors: []
sha256: "d02d4b38f181d7f924678d13802e407fb7f5b1ac88541f99c97ce3101782b1f8"
---

The following sample shows how to create a workflow that notifies a sales rep if a Lead record did not convert to a Customer record within three days of Lead record creation.

The example uses a workflow field, **Lost Lead Email Sent**, on the lead record form to track if the sales rep was notified. A saved search identifies leads created three days before the current date. The workflow runs the saved search on a schedule and sends the email to the sales rep of the leads that have not been converted to customers in three days that meet the saved search criteria.

To set up the workflow, complete the following steps:

-   Create the custom field for the Lead record. See [Step 1 Create the Custom Entity Field for the Lead Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4157625832.html).
    
-   Create the saved search. See [Step 2 Create the Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4157634261.html).
    
-   Create and schedule the workflow. See [Step 3 Create the Workflow and Set the Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4157643624.html).
    

### Related Topics

-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Welcome Email Sent to Customers Three Days After First Order Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html)
-   [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html)
-   [Lead Nurturing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003092.html)
-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

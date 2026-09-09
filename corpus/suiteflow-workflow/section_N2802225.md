---
id: "section_N2802225"
type: "section"
title: "Building the Estimate Approval Routing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Building the Estimate Approval Routing Workflow"
parent: "section_N2801522"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html"
anchors: []
sha256: "fe286563c90559169bf82630f62d3ae5f51fe435aa3f24668ed47d99d8530748"
---

Create the workflow definition and define the basic workflow properties and the workflow initiation properties. The workflow initiates after a user saves a new Estimate record and before NetSuite saves the record data to the database.

#### To create the workflow definition and define when the workflow initiates:

1.  Go to _Customization > Workflows > Workflow > New_.
    
2.  On the **New Workflow** page, enter the following properties:
    
    | Section | Property Name | Value |
    | --- | --- | --- |
    | Basic Information | Name | Estimate Approval Routing |
    | Record Type | Transaction |
    | Sub Types | Quote |
    | Release Status | Testing |
    | Keep Instance and History | Always |
    | Initiation | Event Based | selected |
    | Event Definition | On Create | checked |
    | On View or Update | not checked |
    | Trigger Type | Before Record Submit |
    
3.  Click **Save** to save the workflow definition.
    

**Next Step:** To continue with the estimate approval workflow example, go to [Creating States for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802386.html).

### Related Topics

-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Designing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801832.html)
-   [Before You Build the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801644.html)
-   [Testing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2805158.html)
-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

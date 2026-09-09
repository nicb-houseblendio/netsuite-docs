---
id: "section_N2801644"
type: "section"
title: "Before You Build the Estimate Approval Routing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Before You Build the Estimate Approval Routing Workflow"
parent: "section_N2801522"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801644.html"
anchors: ["procedure_N2801656"]
sha256: "087e2dfd2ff9bc24bf702fd06f86adb4cdd29e62a13cf03ce9c876595754c554"
---

Before you begin building the workflow, you must first create the **Approval Status** custom field, required by the Set Field Value actions.

#### To create the Approval Status custom field: {#procedure_N2801656}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Body Fields > New_.
    
2.  On the Transaction Body Field page, enter the following properties:
    
    | Property | Value |
    | --- | --- |
    | Label | Approval Status |
    | Type | List/Record |
    | Applies To | Sale |
    
3.  Click the **New** button next to the **List/Record** field.
    
4.  In the **Name** field of the **Custom Lists** page, enter **Approval Statuses**.
    
5.  On the **Values** tab, enter each of the following values in the **Value** column and click **Add**:
    
    -   Pending Approval
        
    -   Approved
        
    -   Rejected
        
6.  Click **Save** to save the list.
    
7.  Click **Save** to save the custom field.
    
    The **Approval Status** custom field appears as a dropdown list on the **Custom** subtab of Estimate records.
    

**Next Step:** To continue with the estimate approval workflow example, go to [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html).

### Related Topics

-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Designing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801832.html)
-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)
-   [Testing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2805158.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

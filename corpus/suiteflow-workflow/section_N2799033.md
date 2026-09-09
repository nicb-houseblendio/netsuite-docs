---
id: "section_N2799033"
type: "section"
title: "Building the Lead Nurturing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow"
parent: "section_N2797000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html"
anchors: ["bridgehead_4157447602", "procedure_N2799081", "bridgehead_4157458472", "procedure_N2799274"]
sha256: "647255974755d9c691bcec4029cd8d6664cbc444413c411dfcdd0de860b07625"
---

To build the lead nurturing workflow, complete the following tasks:

-   [Create the Workflow Definition](#bridgehead_4157447602)
    
-   [Create the Workflow Fields](#bridgehead_4157458472)
    

Important:

If you have not already done so, complete the prerequisite tasks before you begin this step for the lead nurturing workflow. See [Before You Build the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html).

## Create the Workflow Definition {#bridgehead_4157447602}

Create the workflow definition and define the basic workflow properties, the workflow initiation, and the workflow initiation condition. The workflow should only initiate after a user saves a new Lead record with an **Industry Type** of **Software**.

#### To create the workflow definition and define when the workflow initiates: {#procedure_N2799081}

1.  Go to _Customization > Workflow > Workflows > New_.
    
2.  On the **New Workflow** page, enter the following properties:
    
    | Section | Property Name | Value |
    | --- | --- | --- |
    | Basic Information | Name | Lead Nurturing |
    | Record Type | Customer |
    | Sub Types | Lead |
    | Release Status | Testing |
    | Initiation | Event Based | checked |
    | Event Definition | On Create | checked |
    | On View or Update | unchecked |
    | Trigger Type | After Record Submit |
    
3.  In the **Event Definition** section, select **Visual Builder** and click the **Open** icon to open the Condition Builder.
    
4.  In the **Workflow Condition** window, enter the condition properties in the following columns:
    
    | Column Name | Value |
    | --- | --- |
    | Field | Industry |
    | Compare Type | any of |
    | Selection | Software |
    
5.  Click **Add**.
    
6.  Click **Save** to save the condition.
    
7.  Click **Save** to save the workflow definition.
    

## Create the Workflow Fields {#bridgehead_4157458472}

The workflow runs actions in its states based on how each recipient reacts to the lead nurturing campaign events. The workflow relies on workflow fields tied to campaign event responses to figure out which actions and transitions to run. You need to create two workflow fields: `Webinar.Response` and `CaseStudy.Response`.

For more information, see [Workflow Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071955161.html).

#### To create the campaign response workflow fields: {#procedure_N2799274}

1.  Make sure the Lead Nurturing workflow is open, created in [Create the Workflow Definition](#bridgehead_4157447602).
    
2.  In the context panel, click the **Workflow** tab, click the **Fields** view, and then click **New Workflow Field**
    
3.  On the **Workflow Field** window, enter the following properties:
    
    | Property | Description |
    | --- | --- |
    | Label | Webinar.Response |
    | Type | List/Record |
    | List/Record | Campaign Response |
    | Store Value | Checked |
    
4.  Click **Save**.
    
5.  Repeat the above steps to create another field with the label **CaseStudy.Response**.
    

**Next Step:** To continue with the lead nurturing workflow example, go to [Creating States for the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799369.html).

### Related Topics

-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Configuring Your Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003300.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)
-   [Before You Build the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html)
-   [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

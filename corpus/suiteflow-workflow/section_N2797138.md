---
id: "section_N2797138"
type: "section"
title: "Before You Build the Lead Nurturing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Before You Build the Lead Nurturing Workflow"
parent: "section_N2797000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html"
anchors: ["bridgehead_4157407397", "procedure_N2797199", "bridgehead_4157416080", "procedure_N2797450", "bridgehead_4157430379", "procedure_N2798429"]
sha256: "e2e34f04bbe535bcdebdcf8172be3daeea4595e85aba1c2cdc324ae50d3e909c"
---

Before you begin building the lead nurturing workflow, complete the following tasks:

-   [Create the Marketing Templates](#bridgehead_4157407397)
    
-   [Create the Lead Nurturing Campaign Record and Campaign Events](#bridgehead_4157416080)
    
-   [Create the Industry Custom Field](#bridgehead_4157430379)
    

## Create the Marketing Templates {#bridgehead_4157407397}

The lead nurturing workflow uses the Send Campaign Email action to send marketing materials to the customer for the Lead record. Create the templates required by the Send Campaign Email actions.

#### To create the marketing templates: {#procedure_N2797199}

1.  Go to _Lists > Marketing > Marketing Templates > New_.
    
2.  Click **Campaign** and then select a template layout.
    
3.  Enter the following properties:
    
    | Property | Value |
    | --- | --- |
    | Name | Webinar Invitation |
    | Subject | Trends in Internet Security |
    
4.  Upload a template file or enter the template text directly in the Text Editor.
    
5.  On the **Marketing** subtab, select from and reply email addresses, and choose an optional campaign domain.
    
6.  Click **Save**.
    
7.  Repeat the above steps to create the following templates:
    
    | Template Name | Subject |
    | --- | --- |
    | Email Case Study | Secure your network with Wolfe Electronics |
    | Customer Testimonial | What our customers are saying |
    | Industry Comparison | Best Internet Security Services 2014 |
    | Free Trial Offer | Try us free for 30 days |
    

## Create the Lead Nurturing Campaign Record and Campaign Events {#bridgehead_4157416080}

Campaign records are used to manage all the information that is important to your marketing efforts. On campaign records, you can create events to represent different parts of the same campaign. When you create the Send Campaign Email actions, you also select the campaign event associated to the email. See [Managing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N985526.html).

#### To create the lead nurturing campaign record and campaign events: {#procedure_N2797450}

1.  Go to _Lists > Marketing > Marketing Campaigns > New_.
    
2.  In the **Title** field, enter **New Lead Nurturing**.
    
3.  Click the **Lead Nurturing** subtab.
    
4.  In the **Template** column, choose **Webinar Invitation**.
    
5.  If you use the Subscription Categories feature, select a **Subscription** category.
    
6.  Click **Add**.
    
7.  Repeat steps 4 to 6 to add the following templates:
    
    -   Email Case Study
        
    -   Customer Testimonial
        
    -   Industry Comparison
        
    -   Free Trial Offer
        
8.  Click **Save**.
    

## Create the Industry Custom Field {#bridgehead_4157430379}

The lead nurturing workflow is designed to send campaign emails to Lead records in the software industry. Create a custom entity field and add it to the Customer record. When a user enters a lead in NetSuite, the user specifies the Industry field and the workflow initiates if the field value is **Software**. For more information about entity fields, see [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html).

#### To create the Industry custom field: {#procedure_N2798429}

1.  Go to _Customization > Lists, Records, & Fields > Entity Fields > New_.
    
2.  In the **Label** field, enter **Industry**.
    
3.  In the **Type** field, select **List/Record**.
    
4.  Next to the **List/Record** field, click **New**.
    
    ![A portion of the Custom Entity Field showing the New icon as selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/LeadNurturingExampleEntityField.png)
5.  On the **Custom List** page, enter the following properties:
    
    | Property | Value |
    | --- | --- |
    | Name | Industry Types |
    | Value | Software |
    
6.  Click **Add** and then click **Save**.
    
7.  On the **Custom Entity Field** page, click the **Applies To** subtab, and check the **Customer** box.
    
8.  Click **Save**.
    

**Next Step:** To continue with the lead nurturing workflow example, go to [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html).

### Related Topics

-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Configuring Your Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003300.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)
-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

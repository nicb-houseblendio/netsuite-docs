---
id: "section_N1033645"
type: "section"
title: "Creating a Custom Record Type for a Customer Survey"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Customer Surveys > Creating a Custom Record Type for a Customer Survey"
parent: "chapter_N1033486"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1033645.html"
anchors: ["procedure_N1033693", "procedure_N1033771", "procedure_N1033869"]
sha256: "9d03ec37a5ae23aebdeba0708ae5f30f7c5edac75f8cfda713934d64888b8658"
---

The first step is to create a custom record type and link it to the customer record.

Note:

This task requires permission to create custom record types. By default, marketing roles do not have this permission. Therefore, this step requires an administrator or a customized role to complete.

#### To create a custom record type for a customer survey: {#procedure_N1033693}

1.  Go to _Customization > Lists, Records, & Fields > Record Types > New_.
    
2.  Enter a name for the record type, such as Customer Survey.
    
3.  Clear the **Include Name Field** box.
    
4.  Click **Save**.
    

Next, create a field to link the customer survey record to the customer record. Customer records are the parent records for customer surveys.

#### To create a custom field to link a survey to the customer record: {#procedure_N1033771}

1.  On the **Fields** subtab, click the **New Field** button. A new field page opens.
    
2.  In the **Label** field, type **Customer**.
    
3.  In the **Type** field, select **List/Record.**
    
4.  In the **List/Record** field, select **Customer**.
    
5.  Check the **Record is Parent** box.
    
6.  Click **Save**.
    
    The custom record page appears with the Customer field listed on the **Fields** subtab.
    

Next, create other fields for the questions you want to include in your survey.

#### To create fields for the questions in the survey: {#procedure_N1033869}

1.  Click the **New Field** button.
    
2.  In the **Label** field, enter a name for the custom record field.
    
3.  In the **Type** field, select the type of field this will be. For example, select Free-form text to create a basic text field.
    
4.  Click **Save**.
    
    The custom record page appears with your new field added to the **Fields** subtab.
    
5.  Repeat these steps for each question you want to add to the record.
    

Now you can create a new record of this type. Go to _Customization > Lists, Records, & Fields > Record Types > New_. Click the New Record link next to your Customer Survey record.

NetSuite provides a list of completed surveys (those completed by you and those completed by customers). To view the list, click the List link on the Record Types page.

### Related Topics

-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Building an Online Form for a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034071.html)
-   [Creating the Link to a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034442.html)
-   [Sending Out a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035006.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1034071"
type: "section"
title: "Building an Online Form for a Customer Survey"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Customer Surveys > Building an Online Form for a Customer Survey"
parent: "chapter_N1033486"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034071.html"
anchors: []
sha256: "f182e1a2589d8eba7303f589231cbb1130e47d60de076d7dbfeb95fb51626a4f"
---

You can create an online form for customers to fill out and create a survey record.

Note:

You'll need permissions to create custom record types, which marketing roles don't have by default. An administrator or a custom role has to do this.

#### To create an online form for a customer survey:

1.  Go to _Customization > Lists, Records, & Fields > Record Types_.
    
2.  Click the **Customer Survey** link in the **Edit** column.
    
3.  On the Customer Survey record page, click the **Online Forms** subtab.
    
4.  On the **Online Forms** subtab, do one of the following:
    
    -   Click **New Online Form** to create the form customers will use to complete the survey. Select the record fields that will appear on the form and define the order of those fields. Set other parts of the form's appearance such as the way fields display, color theme, and a form logo.
        
    -   Click **New Online HTML Form** to use a custom HTML template and fully control your form's layout and appearance. For more information, see [Online Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981889.html).
        
5.  On the **Select Fields** subtab, select the **Customer** field in the **Field** column. NetSuite uses this field to link the survey to the customer record.
    
6.  Clear the box in the **Select** column.
    
    You can hide this field on the form. If you pass the customer name through the URL, it can help avoid confusion for the respondent. For more information, see [Creating the Link to a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034442.html).
    
7.  Click **Add**.
    
8.  Repeat these steps for each question you want on the survey.
    
9.  Set up the online form as you want it to appear for customers. For more information, see [Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882522.html).
    
10.  Click **Save**.
     

For a custom HTML form, you must supply tags in the body of your document to show how fields are arranged.

Each field tag should look like <NLTAG>. You make a tag by adding NL to a field ID. You'll find the ID for custom fields on the Fields subtab in the ID column. Each tag should be formatted like this: <NLCUSTRECORD1>.

### Related Topics

-   [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html)
-   [Creating a Custom Record Type for a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1033645.html)
-   [Creating the Link to a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034442.html)
-   [Sending Out a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035006.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

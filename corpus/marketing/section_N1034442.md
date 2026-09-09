---
id: "section_N1034442"
type: "section"
title: "Creating the Link to a Customer Survey"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Customer Surveys > Creating the Link to a Customer Survey"
parent: "chapter_N1033486"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034442.html"
anchors: ["procedure_N1034491", "procedure_N1034587", "procedure_N1034751"]
sha256: "51dffa666ac0383936dbf60943d2215037aaea942a4216f5e8b763765dcbf2dd"
---

The next step is to build the URL you'll use to link customers to your survey.

To build the URL, first find the online form's publishable URL, then add a parameter to the end.

Note:

You'll need permissions to create custom record types, which marketing roles don't have by default. An administrator or a custom role has to do this.

#### To find the form's URL: {#procedure_N1034491}

1.  Go to _Customization > Lists, Records, & Fields > Record Types > New_.
    
2.  Click the link for your Customer Survey record type under the **Edit** column.
    
3.  On the **Online Forms** subtab, click the name of your online form.
    
    The online form record opens in a new window.
    
4.  Click the **External** subtab, and find the **Publishable Form URL**.
    
    The URL is in the following format: https://system.netsuite.com/app/site/crm/ externalcustrecordpage.nl?compid=1a2b3c4d&formid=xx&h=1a2b3c4d
    

The next steps add a parameter to the URL that passes the customer's name into the form. This way, customers can't enter their own name, so you don't have to worry about mismatches that would keep the survey from linking to the correct record.

#### To add a parameter to the form's URL: {#procedure_N1034587}

1.  On the Customer Survey record, click the **Fields** subtab.
    
2.  Copy the ID for the **Customer** field.
    
3.  Create a parameter to add to the end of the publishable form URL. The parameter sets the **Customer** field on the Survey form to the ID of the customer you send the survey email to. There are two parts to this parameter:
    
    -   The field's ID - for example, custrecord1.
        
    -   The FreeMarker Syntax - ${record.field}
        
        This FreeMarker Syntax dynamically pulls the name from the customer's record when you send the email.
        
        (The field ID must be changed to lowercase when you build the parameter.)
        
    
    The parameter in this example would look like &custrecord1=${record.field} and should follow the capitalization in this example.
    
4.  Add this parameter to the end of the publishable form URL located in the previous set of steps.
    
    Your final URL should look like:
    
    https://system.netsuite.com/app/site/crm/externalcustrecordpage.nl?compid=1a2b3c4d&formid=xx&h=1a2b3c4d&custrecord1=${record.field}
    

To verify that you correctly created the form URL, you should test the link before you send it to customers.

#### To test the link to your survey: {#procedure_N1034751}

1.  Go to _Lists > Relationships > Clients > New_ and create a test customer.
    
2.  Enter an email address you have access to in the **Email** field.
    
3.  Click **Save**.
    
4.  After you save the customer record, click the **Communication** subtab, and then click **Email**.
    
5.  On the **Message** subtab of the email message, enter a subject.
    
6.  Enter text for your link, select the text, and click the **Link** button.
    
7.  Enter the URL for the custom record form.
    
    In the URL, replace the **&custrecord1** parameter with the ID of the customer field you created above.
    
    The URL should be in this format: https://system.netsuite.com/app/site/crm/ externalcustrecordpage.nl?compid=1a2b3c4d&formid=xx&h=1a2b3c4d&custrecord1=${record.field}
    
8.  Click **Merge and Send**.
    
    NetSuite replaces the tags with the customer's name in the email it sends.
    
9.  Check your email and click the link to the survey form.
    
10.  Confirm that the name of the test customer is showing in the URL.
     

### Related Topics

-   [Tips for Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html)
-   [Creating a Custom Record Type for a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1033645.html)
-   [Building an Online Form for a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1034071.html)
-   [Sending Out a Customer Survey](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035006.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

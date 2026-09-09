---
id: "section_N529539"
type: "section"
title: "Using Fax Templates"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge > Using Fax Templates"
parent: "section_N523426"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html"
anchors: ["bridgehead_N529703", "bridgehead_N529835", "procedure_N529858"]
sha256: "cb1811025f1ce13ef055449b3d6b86c4f6c701e1202f1961d1dbc23b1b69e69f"
---

Note:

This topic is unrelated to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

Fax templates are text documents you create for use in mail merge operations. Fax templates generate personalized fax documents that you can send to those with whom you do business.

Before you can send faxes from NetSuite, you must register with [eFax®](http://www2.efax.com/efax/twa/page/efaxPlus?). For more information about this service, see [Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163594359424.html).

## Creating a Fax Template {#bridgehead_N529703}

You can create fax templates as scriptable templates. Scriptable templates let you customize the output to include information specific to the recipient. For more information, see [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html).

Below is a sample fax template that incorporates FreeMarker code. This example is a fax sent to new leads by the sales rep they are assigned to.

          `<#if Customer.companyName = "">${Customer.firstName} ${Customer.lastName}<#else>${Customer.companyName}</#if><br /> ${customer.billAddr1}<br /> ${customer.billAddr2}<br /> ${customer.billCity}<br /> ${customer.billState} ${customer.billZip}<br /> ${customer.billCountry}   <p>Dear <#if Customer.companyName = "">${Customer.firstName}<#else>Customer</#if>,</p>   <p>My name is ${Customer.salesRep.firstName}, a sales representative for Wolfe Electronics in the ${Customer.billCity} area.</p>   <p>Thank you for your interest in Wolfe Electronics. If you need any assistance in placing an order, or if you need information about any of our products, please call me on ${Customer.salesrep.phone}.</p>   <p>Sincerely,</p> <br /> ${preferences.MESSAGE_SIGNATURE}` 
        

When NetSuite merges the fax, information from the lead record replaces the tags.

Tom Wetteland

TRS Van Lines, Ltd.

Suite 12

3810 Castleberry Rd.

San Diego, CA 92110

Dear Tom,

My name is Krista Barton, a sales representative for Wolfe Electronics in the San Diego area.

Thank you for your interest in Wolfe Electronics. If you need any assistance in placing an order or if you need information about any of our products, please call me on 408-555-3652.

Sincerely,

Krista Barton

Wolfe Electronics

After you create your fax template, you can create a fax template record.

## Creating a Fax Template Record {#bridgehead_N529835}

If you create a fax template file outside of NetSuite, upload the file to the Fax Templates folder of your NetSuite file cabinet. You can also create a template directly on the template record.

#### To create a fax template record: {#procedure_N529858}

1.  Go to Documents > Templates > Fax Templates > New.
    
2.  Enter a name for this template.
    
3.  In the **Description** field, enter information about this template.
    
4.  On the **Template** subtab, in the **Subject** field, enter the subject of the fax.
    
5.  Do one of the following:
    
    -   Select **File** if you uploaded the template file to your file cabinet, and then select the file. Select **New** if you have not uploaded your template file to your file cabinet.
        
        ![Screenshot of a portion of the Fax Template (Scriptable) page and its Template subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/NewFaxTemplate_Chiles2.PNG)
    -   Select **Text Editor** if you have not created your fax template. Compose your template in the rich text field.
        
        If your template file contains HTML and you want to paste the template text, click the **HTML Source Code** button. This option ensures that your code is properly included.
        
        Select a field in the **Insert Field** list to have NetSuite place the corresponding fields in your template.
        
6.  **On the Restrict Access** subtab, check the **Private** box if you do not want others in your company to use this template.
    
7.  If you want this template to be used by members of a specific group, select that group in the **Restrict to Group** field.
    
8.  Click **Save**.
    

### Related Topics

-   [Merging Faxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N527062.html)
-   [Working with Mail Merge](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N523426.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

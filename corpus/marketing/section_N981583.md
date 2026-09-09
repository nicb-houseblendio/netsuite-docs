---
id: "section_N981583"
type: "section"
title: "Tips for Passing Parameters Through URLs"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Passing Parameters Through URLs > Tips for Passing Parameters Through URLs"
parent: "section_N979468"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html"
anchors: []
sha256: "b254f57b19ec7e228916c3958c6f549a0652af5a00c9bfacec1e28129bbe89cc"
---

Consider the following tips for using parameters correctly in links:

-   The **leadsource** parameter is used to pass the campaign ID into an online customer form. The campaign ID in the URL fills the Lead Source field on the online form.
    
-   To pass a partner code in a URL, use the **partner** parameter. Partner codes help you keep the partner-customer relationship private by not showing the partner's name in the URL.
    
-   For box fields, enter **T** as the value if you want the box checked. Enter **F** if you want the box clear. For example, a link that passes a parameter to a box field would look like this:
    
                  `https://system.netsuite.com/app/site/crm/externalleadpage.nl?compid=ACCT000000&formid=1&h=1bdc80a058&unsubscribe=T` 
                
    
-   You must spell and capitalize campaign IDs, partner names, and partner codes passed in the parameter exactly as they appear on their record.
    
-   You can add as many parameters as you want to pass through to your online customer form. A link with multiple parameters should follow this format:
    
                  `https://system.netsuite.com/app/site/crm/externalleadpage.nl ?compid=ACCT000000&formid=1&h=1bdc80a058?partner=Wilson%20 Computers&leadsource=March%202010%20Flyer` 
                
    
    Each parameter beyond the first begins with an ampersand (&). The first parameter, **compid**, which is an internal parameter identifying your company, begins with a question mark (?). The partner and lead source parameters each begin with an ampersand.
    
-   Replace any spaces in your URLs with hyphens (-).
    
-   You may want to pass information into hidden fields on your online customer forms. Information in a hidden field saves to the customer record when the online form is submitted. However, the person filling out the form can't see the field.
    
    To hide a field on a form, check the box in the Hide column when selecting fields to include on your form.
    

### Related Topics

-   [Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979468.html)
-   [Embedding an Online Form in your Website Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html#bridgehead_N2592052)
-   [Case and Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html)
-   [File Download with Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592134.html)
-   [Online Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981889.html)
-   [Subsidiaries on Online Customer Forms in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

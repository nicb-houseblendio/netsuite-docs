---
id: "section_N979468"
type: "section"
title: "Passing Parameters Through URLs"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Passing Parameters Through URLs"
parent: "chapter_N973827"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979468.html"
anchors: []
sha256: "45df5e5ccbd8247562a68b62322b397fea8de32e3bb5b6f94814178724dbbbc4"
---

You can use parameters to pass information through the links to your online customer forms. For example, if you link from partner websites, you can include the partner's name or code in the URL. When you do this, you know the source of the new lead or customer. You can also use parameters in links for paid search campaigns.

When a customer clicks a link to an online form and submits it, NetSuite creates a new lead, prospect, or customer record. If you include parameters in the link, NetSuite adds that info to the new record, so you can link it to a campaign or partner.

For example, Wolfe Electronics advertises through banner ads online. Each ad links to an online customer form on their website. The marketing manager wants to track which ad campaign sends each lead to the form.

The campaign ID for each ad is passed through the link to the online form. When the lead submits Wolfe Electronics' lead capture form, the campaign is automatically selected on the lead record that NetSuite creates.

You can find a form's URL in the Publishable Form URL field on the External subtab of the online customer form record.

To pass information through a link, you add the information to the end of the publishable form URL. In the example above, the URL might look like this:

          `https://system.netsuite.com/app/site/crm/externalleadpage.nl?compid=ACCT000000&formid=1&h=1bdc80a058&leadsource=JoinNowAd` 
        

In this sample URL, the first parameter in a URL begins with a question mark (?). Each parameter after the first begins with an ampersand (&). Most URLs include parameters by default. In this example, there are parameters referring to the NetSuite company ID and the online form's ID.

Note:

Spaces in parameters should be replaced with `%20`.

The table below lists the parameters you can use to automatically insert information into an online customer form.

| **Field** | **Parameter** |
| --- | --- |
| Campaign Event\*\*\* | &campaignevent=187 |
| Company Name | &companyname=Global%20Distributing,%20Inc. |
| City | &city=New%20York |
| Country | &country=USA |
| Custom Form | &customform=New%20Lead%20Form |
| E-mail | &email=john@example.com |
| Lead Source | &leadsource=Spring%20Ad%20Campaign |
| Login Password | &password=password |
| Partner\*\* | &partner=Universal%20Consulting |
| Partner Code\*\* | &partner=1111 |
| Phone Number | &phone=555-555-5554 |
| Promotion | &promocode=Feb%20Flyer |
| State | &state=New%20York |
| Zip/Postal Code | &zip=54321 |

\* The **&customform** parameter determines which lead, prospect, or customer entry form is used when editing or viewing the record you create.

\*\*The **&partner** parameter is used to pass both partner names and partner codes.

\*\*\*The **&campaignevent** parameter determines which event is associated to the customer entry form. The value of this parameter is the internal ID of the campaign event.

If a partner's site links to your online customer form, you might want the Partner field to show their name. To do this, you can create a link in this format:

            `https://sample.online.customer.form.com?partner=Partner%20Name` 
          

When a lead clicks the link to your online customer form on the partner's web page, they are taken to your online customer form. The Partner field is filled in automatically.

If you link to online customer forms in NetSuite, you can pass information into custom fields about the person filling out the form. For example, you could pass this information when linking to a custom record form from your Customer Center.

The internal form URL from the External subtab of the online form record lets you add any of the parameters in the table below.

| Info | Parameter |
| --- | --- |
| name | {name} |
| login email address | {email} |
| first name | {firstname} |
| last name | {lastname} |
| internal ID | {user} |
| internal ID of user's role | {role} |

Each parameter must be enclosed in brackets, { and }. If you want to pass the user's name and email address to a form, the link could look like this:

          `/app/crm/common/onlineforms/ internalonlineform.nl?formid=100&custrecord123={name}&custrecord124 ={email}` 
        

-   custrecord123 is the ID of a custom field on the custom record that tracks the name of the person filling out the form.
    
-   custrecord124 is the ID of the custom field that tracks the email address of the person filling out the form.
    

For more information about online customer forms, see [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html).

For information about how to set the Subsidiary field on online customer forms, see [Subsidiaries on Online Customer Forms in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html).

You can also embed the online form in your website so that the customer never leaves your website when they use that form. For more information, see [Embedding an Online Form in your Website Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html#bridgehead_N2592052).

### Related Topics

-   [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html)
-   [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html)
-   [Custom Field Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981425.html)
-   [Passing Parameters from Third Party Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981510.html)
-   [Tips for Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "bridgehead_N981425"
type: "bridgehead"
title: "Custom Field Parameters"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Passing Parameters Through URLs > Custom Field Parameters"
parent: "section_N979468"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981425.html"
anchors: []
sha256: "8533c1069a452093fe469b5307c6eb2ecbafc8e56f53a427cf48af5bbf44088a"
---

You can create custom entity fields to track information specific to your business. You can include these fields in online customer forms.

A marketing manager creates a custom box field called Product Trial Candidate to find leads willing to test new products. When a lead clicks the link to "Try New Products - Free!", they're taken to an online lead capture form. The Product Trial Candidate box is checked on the form and on the lead record NetSuite creates when the form is submitted.

If you want to pass custom field information into your online lead capture forms, first determine the custom field ID. It's in the ID field on the custom field record. A URL with custom field parameters should follow this format:

          `https://system.netsuite.com/app/site/crm/externalleadpage.nl?compid=ACCT000000&formid=1&h=1bdc80a058&custentity1=industryperiodical` 
        

Custom box fields follow the following format:

          `https://system.netsuite.com/app/site/crm/externalleadpage.nl?compid=ACCT000000&formid=1&h=1bdc80a058 &custentity2=T` 
        

If you want the box marked, set the parameter to **T** in the URL. To clear the box, use **F** through the URL.

For more information about creating custom fields, see the **Customization** user guide.

### Related Topics

-   [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html)
-   [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html)
-   [Passing Parameters from Third Party Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981510.html)
-   [Tips for Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

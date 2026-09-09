---
id: "section_N282433"
type: "section"
title: "Subsidiaries on Online Customer Forms in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > OneWorld CRM > Subsidiaries on Online Customer Forms in OneWorld"
parent: "section_N281005"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html"
anchors: []
sha256: "5d22ab82ae9d4c6230b71c6cca581cfa3f9808e6eb82584a7cc294fc2b38b3bd"
---

With NetSuite OneWorld, online forms include the Subsidiary field.

NetSuite always considers the Subsidiary field when determining if the records created by a form is a duplicate. You can't clear the box in the Search column for this field. This field is also hidden by default.

If a customer fills out an online form and the information matches a customer record for another subsidiary, NetSuite creates a new record. A customer is considered a duplicate if there is a customer record with the same subsidiary as the one selected on the online form.

To create an online customer form in OneWorld, go to _Setup > Marketing > Setup Tasks > Online Customer Forms > New_. On the Select Type page, click **Default Form Template**. For more information, see [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html).

You can set the subsidiary on an online form in the following ways. If you use more than one method, subsidiary selection follows the order of precedence below:

-   Add the Subsidiary field to the form, and then allow those that fill out the form to select a subsidiary.
    
-   Pass the subsidiary through the URL with the **&subsidiary** parameter. This parameter lets you hide the field on the form.
    
    For more information, see [Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979468.html).
    
-   Select the subsidiary included in the visitor ID of the person submitting the form. NetSuite tracks the visitor ID in the cookie issued when someone visits your website.
    
-   Set the default subsidiary in the Default Subsidiary field on the Set Up Workflow subtab of the online form record.
    

If you use online customer forms to create contact records, NetSuite assigns the contact the subsidiary associated with the customer record.

### Related Topics

-   [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html)
-   [OneWorld CRM](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281005.html)
-   [OneWorld and SuiteCommerce](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282701.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N991575"
type: "section"
title: "Marketing to Contacts"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Managing Campaigns > Creating Target Groups for Campaigns > Marketing to Contacts"
parent: "section_N991148"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N991575.html"
anchors: ["procedure_N991629"]
sha256: "92fa1b18c9b99c8b22e8d3420aeb67cf71e653be55bd9c948526d4f20fcb7319"
---

Depending on your customer base, you may prefer to send your marketing campaigns to contacts, rather than the customer for whom they work. You can create a target group of contacts based on the characteristics of the customer who employ them.

The Wolfe Electronics marketing manager plans to send email messages to let customers know about a summer sales promotion. Rather than send the email to the customer's company email address, the marketing manager sends it to their primary customer contacts. This email includes a coupon code that they can use when they place an order. The marketing manager creates a new customer search that filters out customers that have not purchased within the last year. Then, they create a group made up of the primary contacts for these customers.

You can track lead sources for contacts in the same way you do for leads, prospects, and customers. There is no transaction or revenue impact of a contact's lead source. Contact lead sources can help you understand which marketing campaigns are most effective at bringing contacts to your company.

You can use online customer forms to capture contact information. See [Using Online Customer Forms for Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979259.html).

Before creating a dynamic contact group based on customer criteria, you must first create the contact saved search the group is based on.

#### To create a contact group based on customer criteria: {#procedure_N991629}

1.  Go to _Campaigns > Contacts > Search_.
    
2.  Check the **Use Advanced Search** box.
    
3.  Click **Create Saved Search**.
    
4.  On the **Criteria** subtab, set criteria based on customer fields.
    
5.  After you set the customer criteria, click **Save**.
    
6.  Go to _Campaigns > Marketing > Groups > New_.
    
7.  On the Create Group page, choose **Dynamic**, and then select **Contact** in the list.
    
8.  Enter a name for this group.
    
9.  Next to the **Saved Search** field, choose the saved search you created.
    
10.  Click **Save**.
     

After you have sent a campaign message to contacts, you can track revenue as if the event targeted the customers the contacts work for.

After contacts review the marketing email, they place orders on behalf of their employers. As orders are placed, Wolfe sales reps enter the campaign's coupon code on the order. Later, the Wolfe marketing manager can view the Campaign ROI Analysis and Sales by Promotion reports to determine the success of the campaign.

When contacts submit online customer forms, NetSuite tracks the submissions on the Online Forms subtab on the contact record. NetSuite displays the online form's name, contact's company, and lead source that generated the form submission, for each submission. NetSuite also displays the submission on the Online Forms subtab of the customer record associated with the contact.

### Related Topics

-   [Creating Target Groups for Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N991148.html)
-   [Creating a Campaign Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986170.html)
-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)
-   [Marketing Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1010316.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

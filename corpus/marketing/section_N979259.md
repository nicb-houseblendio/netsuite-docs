---
id: "section_N979259"
type: "section"
title: "Using Online Customer Forms for Contacts"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Online Customer Forms > Using Online Customer Forms for Contacts"
parent: "section_N976289"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979259.html"
anchors: ["procedure_N979300"]
sha256: "f3de0e1a77e58a9b2aba605271a310b4093ae3a061731b9d5344c23b9716977f"
---

If you set up your online customer forms to create company records, NetSuite creates two records when the form is submitted: a contact record, and a lead, prospect, or customer record.

![Screenshot of a portion of the Set Up Workflow subtab with the Create Customers as Companies box checked and outlined](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/Marketing_Using_Online_Cust_Forms.png)

#### To create an online customer form that creates customer records: {#procedure_N979300}

1.  Add the **Company Name**, **First Name**, and **Last Name** fields to the form.
    
2.  Mark these fields as mandatory.
    
3.  On the **Set Up Workflow** subtab, check the **Create Customers as Companies** box.
    
4.  If you want to set the lead source on the contact record, select it in the **Set Lead Source** field. Lead source is the campaign associated with the customer form. The value you select lets you know which campaign generated the new lead, customer, or updated information.
    
5.  You can track an event in the Online Customer Form. After you select a lead source, select a value in the **Set Campaign Event** field. This value lets you map which event led to the form completion by the customer or lead.
    
6.  You can let the lead source on this form to overwrite the lead source on any contact record updated by this form. Check the **Allow Update on Contact Record** box.
    
7.  Click **Save**.
    

When a contact submits the form, NetSuite creates a customer record and a contact record. If there are existing records that match what was entered, NetSuite updates those records instead. For more information, see [Using Online Customer Forms for Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979259.html).

### Related Topics

-   [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html)
-   [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html)
-   [Lead Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N975884.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

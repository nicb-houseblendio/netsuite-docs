---
id: "bridgehead_N1086741"
type: "bridgehead"
title: "Lead Conversion Using the Lead Conversion Feature"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Lead Management > Lead Conversion > Lead Conversion Using the Lead Conversion Feature"
parent: "section_N1086628"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086741.html"
anchors: ["subsect_162708057952", "subsect_162708061572", "subsect_162708066051"]
sha256: "5e18a50e7ce0eb314c2ca91725954203a76a77197883bd1baa0c4bf374e718c3"
---

If your company uses a business-to-business workflow, you should enable the Lead Conversion feature. Administrators can enable the Lead Conversion feature on the CRM subtab of the Enable Features page at _Setup > Company > Setup Tasks > Enable Features_.

Before you start using the feature, set the Default Lead Type preference to **Individual**. This preference is located at _Setup > Company > Preferences > General Preferences_.

With the Lead Conversion feature, some lead records have a Save & Convert button. You'll see this button when an individual lead has a company name. When you click the Save & Convert button, the Convert Lead page opens, giving you several options for the resulting records in your NetSuite account.

On the Convert Lead page, you first transform the lead to a prospect, resolving any potential duplicate records. Then on the same page, you create a contact to associate with the prospect, again resolving potential duplication. Finally, you have the option to create tasks and opportunities. For instructions, see [Converting a Lead on the Convert Lead Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162733129047.html).

You must have the Lead Conversion permission to use the Save & Convert button. In NetSuite accounts created after 2009.2, all standard sales roles have this permission when you use the Lead Conversion feature. However, an administrator must add it to any custom roles. See [Setting Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288727.html).

For a list of fields on the lead record that map to fields on the prospect and opportunity records, see [Lead Conversion Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1090008.html).

For information about the records that result from lead conversion with this feature, see the following:

-   [Prospect Record](#subsect_162708057952)
    
-   [Contact Record](#subsect_162708061572)
    
-   [More Options](#subsect_162708066051)
    

Other topics related to the Lead Conversion feature are as follows:

-   [Converting a Lead on the Convert Lead Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162733129047.html)
    
-   [Lead Conversion Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1090008.html)
    
-   [Setting Up Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093237.html) - includes information not dependent on the feature
    

## Prospect Record {#subsect_162708057952}

The prospect record lets you track all the information you need to convert a prospect into a customer. This record is the next stage in the sales cycle after lead. Prospects can have associated opportunities and estimates. The prospect record includes any transactions and user notes from the lead record.

If existing lead, prospect, or customer records match the company name on the lead record, NetSuite lists the potential matches on the Convert Lead page. You can select one of these potential matches or create a new prospect record. If you select an existing record, NetSuite combines the information and permissions included in the current lead record with information in the existing record.

NetSuite determines possible duplicates based on your Duplicate Detection settings and the setting of the **Consider "Starts With" Matches in Lead Conversion** preference on the Sales Preferences page. When the box for this sales preference is checked, NetSuite compares the first word of the lead's company name to existing prospect and customer records. The comparison is not case sensitive. For example, if the current lead works for Green Corp., NetSuite lists an existing prospect named Green Fields, Inc., as a possible duplicate. For information about Duplicate Detection settings, see [Duplicate Record Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490932.html). For information about other sales preferences, see [Sales Force Automation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035924.html).

## Contact Record {#subsect_162708061572}

Contact records store information about individuals with whom you have a business relationship. For information about these records, see [Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1075037.html).

With the conversion, NetSuite attaches the lead's activities and campaign responses to the contact record. This keeps a history of how your company interacted with your leads even after those leads are converted.

When you convert the lead to an existing contact, NetSuite sets campaign subscriptions according to the following rules. These rules apply only if both the lead and contact have the same email address. If the email addresses are different, the process skips these rules.

-   If either record (the lead or the existing contact) is globally unsubscribed, both records are globally unsubscribed.
    
-   If one record is **Confirmed Opt-In** and the other is **Soft Opt-In** or **Soft Opt-Out**, the contact record is **Confirmed Opt-In**.
    
-   If one record is **Confirmed Opt-Out** and the other is **Confirmed Opt-In**, the contact is **Confirmed Opt-In** because this is the most currently confirmed status.
    
-   If both records are **Soft Opt-In**, the contact record is **Soft Opt-In**. The subscription categories from both the lead and contact record are **Soft Opt-In** before conversion and **Soft Opt-In** after conversion.
    
-   If one record is **Soft Opt-In** and the other is **Soft Opt-Out**, the contact is **Soft Opt-In**. The subscription categories from both the lead and contact record are **Soft Opt-In** before conversion and **Soft Opt-In** after conversion.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

These changes affect only those leads who are converted through the Convert Lead page. The activities and campaign responses are carried over to the prospect or customer record for leads who are converted by entering transactions. This is also true for leads converted by manually changing customer status.

## More Options {#subsect_162708066051}

During conversion you can also:

-   Create an opportunity record for the ensuing negotiations. For information about these records, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).
    
-   Create a task record to track the next step in the process. For information about these records, see [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html).
    

### Related Topics

-   [Lead Conversion](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086628.html)
-   [Conversion by Status Changes and Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086702.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

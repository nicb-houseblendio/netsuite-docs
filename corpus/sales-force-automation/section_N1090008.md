---
id: "section_N1090008"
type: "section"
title: "Lead Conversion Field Mapping"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Lead Management > Lead Conversion > Lead Conversion Using the Lead Conversion Feature > Lead Conversion Field Mapping"
parent: "bridgehead_N1086741"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1090008.html"
anchors: []
sha256: "737f63524f010a0a8ddcdc57525dd85542ae73ac1df2cfd8e9eae7deedba4478"
---

When you use the Lead Conversion feature, NetSuite maps information from the lead record to the resulting prospect, contact, and opportunity records.

In the following table, the first column lists the fields on the Standard Lead Form. The other columns show the corresponding fields on the prospect, contact, and opportunity records. NetSuite doesn't transfer fields on the lead record to the task record. For example, Company Name on a lead record becomes Company Name on the prospect and Company on an opportunity.

| Before Conversion | After Conversion |
| --- | --- |
| Lead | Prospect | Contact | Opportunity |
| --- | --- | --- | --- |
| ID | **Does not transfer** | \- | \- |
| Mr./Ms. | \- | Mr./Ms. | \- |
| Name | \- | Name | \- |
| Status | **Does not transfer** | \- | \- |
| Address 1 | \- | Address 1 | \- |
| Address 2 | \- | Address 2 | \- |
| City | \- | City | \- |
| State | \- | State | \- |
| Country | \- | Country | \- |
| Zip | \- | Zip | \- |
| Company Name | Company Name | \- | Company |
| Phone | Phone\* | Phone | \- |
| Email | Email | Email | \- |
| Fax | Fax\* | Fax | \- |
| Alt. Phone | Alt. Phone\* | Alt. Phone | \- |
| Home Phone | \- | Home Phone | \- |
| Mobile Phone | \- | Mobile Phone | \- |
| Alt. Email | Alt. Email | Alt. Email | \- |
| Job Title | \- | Job Title | \- |
| Web Address | Web Address\* | \- | \- |
| Sales Rep | Sales Rep\*\* | \- | Sales Rep |
| Territory | Territory\* | \- | \- |
| Lead Source | Lead Source\* | Lead Source | Lead Source |
| Lead Role | Lead Role | \- | \- |
| Partner | Partner\* | \- | \- |
| Campaign Category | Campaign Category\* | Campaign Category | Campaign Category |
| Subscription Status | \- | Subscription Status | \- |
| Comments | Comments\* | Comments | \- |
| Estimated Budget | Estimated Budget\*\*\* | \- | Estimated Budget\*\*\* |
| Budget Approved | Budget Approved\*\*\* | \- | Budget Approved\*\*\* |
| Sales Readiness | Sales Readiness\*\*\* | \- | Sales Readiness\*\*\* |
| Buying Time Frame | Buying Time Frame\*\*\* | \- | Buying Time Frame\*\*\* |
| Buying Reason | Buying Reason\*\*\* | \- | Buying Reason\*\*\* |

**\*** NetSuite transfers data from these fields only when you create a new prospect on the Lead Conversion page, not when you use an existing prospect.

**\*\*** The sales representative transfers to the prospect record only if you select the value on the Lead Conversion page.

**\*\*\*** NetSuite transfers data from these fields according to the following rules:

-   You create an opportunity as part of lead conversion. These fields are transferred to the opportunity record.
    
-   You don't create an opportunity, but you create a new prospect as part of conversion. These fields are transferred to the prospect record.
    
-   You don't create an opportunity, but you attach the lead to an existing prospect. These fields are transferred to the prospect record only if the field on the prospect record has no data.
    

If you use the Multiple Currencies feature and attach a lead to an existing customer record, the list of transaction currencies are combined. The primary currency of the existing customer is maintained. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

### Related Topics

-   [Lead Conversion Using the Lead Conversion Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086741.html)
-   [Converting a Lead on the Convert Lead Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162733129047.html)
-   [Mapping Custom Lead Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095304.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "bridgehead_N2886648"
type: "bridgehead"
title: "Available Standard Fields and Field Types for Custom Record Types and Source Lists"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Sourcing with Custom Records > Available Standard Fields and Field Types for Custom Record Types and Source Lists"
parent: "section_N2886428"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2886648.html"
anchors: ["bridgehead_N2886665", "bridgehead_N2888499"]
sha256: "19cdb1b00fa3e2ba5f7746c9c4e71c615668ac2807112b65887820f13e9e90a8"
---

Custom record types and source lists can use sourcing with the standard fields and records listed in the following table. In addition to standard records, you can use custom fields and record types for sourcing. When using custom fields and record types for sourcing, the field type selected depends on the field type of the custom field being sourced from.

For example, let's say you've created a custom entity check box field for Quarterly Mailing. If you want to source information from the Quarterly Mailing field to a custom CRM field for cases, you must select Check Box in the Type field when creating your CRM field.

## Customer, Employee, Partner, and Vendor Fields {#bridgehead_N2886665}

| Field | Type | Customer | Employee | Partner | Vendor |
| --- | --- | --- | --- | --- | --- |
| Name/ID | Free-Form Text | × | × | × | × |
| Bill To | Text Area | × | × | \- | × |
| Ship To | Text Area | × | \- | \- | × |
| Phone | Phone Number | × | × | × | × |
| Fax | Phone Number | × | \- | × | × |
| E-mail | E-mail Address | × | × | × | × |
| City | Free-Form Text | × | × | \- | × |
| State | Free-Form Text | × | × | \- | × |
| Zip | Free-Form Text | × | × | \- | × |
| Country | Free-Form Text | × | × | \- | × |
| Sales Rep | List/Record\* | × | \- | \- | \- |
| Expected Close Date | Date | × | \- | \- | \- |
| Renewal Date | Date | × | \- | \- | \- |
| Contact | Free-Form Text | × | \- | \- | × |
| Alt. Contact | Free-Form Text | × | \- | \- | × |
| Alt. Phone | Phone Number | × | \- | \- | × |
| Balance | Currency | × | \- | \- | × |
| Credit Limit | Currency | × | \- | \- | × |
| Account | Free-Form Text | × | \- | \- | × |
| 1099 Eligible | Check Box | \- | \- | \- | × |
| Tax ID | Free-Form Text | \- | \- | \- | × |
| Company Name | Free-Form Text | \- | \- | × | × |
| Supervisor | List/Record\* | \- | × | \- | \- |
| Soc. Sec. # | Free-Form Text | \- | × | \- | \- |

\* In the List/Record field, you must select the Employee list for sourcing to work properly.

## Item {#bridgehead_N2888499}

| **Field** | **Type** |
| --- | --- |
| Name | Free-Form Text |
| Display Name | Free-Form Text |
| Vendor Name | Free-Form Text |
| Online Name | Free-Form Text |
| Available Online | Check Box |
| Base Price | Currency |
| Cost | Currency |
| Preferred Vendor | List/Record\* |
| On Hand | Decimal Number |

\* In the List/Record Field, you must select the Vendor list for sourcing to work properly.

### Related Topics

-   [Sourcing with Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886428.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

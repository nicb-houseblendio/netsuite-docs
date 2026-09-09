---
id: "bridgehead_N2843917"
type: "bridgehead"
title: "Transaction Body Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Available Standard Fields and Field Types > Transaction Body Fields"
parent: "section_N2843906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2843917.html"
anchors: ["bridgehead_N2843925", "bridgehead_N2845962", "bridgehead_N2846519"]
sha256: "bd7ed87e0d2abdb643b8374c4332985eb728161e2bbb43c16e84cc79c19a555b"
---

You can source from Entity, Ship To, or Sales Rep fields.

## Source From Entity {#bridgehead_N2843925}

The type of entity used to source from depends on the type of transactions you apply your field to. **Purchase** transactions source values from **vendor** records. **Sales** transactions source values from **customer** records, and **expense reports** source from **employee** records.

Note:

To source correctly, select the Employee list in the List/Record field.

| **Field** | **Type** | **Sales Transactions** | **Purchase Transactions** | **Expense Reports** |
| --- | --- | --- | --- | --- |
| Name | Free-Form Text | × | × | × |
| Bill To | Text Area | × | × | × |
| Ship To | Text Area | × | × | \- |
| Phone | Phone Number | × | × | × |
| Fax | Phone Number | × | × | \- |
| Email | Email Address | × | × | × |
| City | Free-Form Text | × | × | × |
| State | Free-Form Text | × | × | × |
| Zip | Free-Form Text | × | × | × |
| Country | Free-Form Text | × | × | × |
| Sales Rep | List/Record | × | \- | \- |
| Expected Close Date | Date | × | \- | \- |
| Renewal Date | Date | × | \- | \- |
| Contact | Free-Form Text | × | × | \- |
| Alt. Contact | Free-Form Text | × | × | \- |
| Alt. Phone | Phone Number | × | × | \- |
| Balance | Currency | × | × | \- |
| Credit Limit | Currency | × | × | \- |
| Account | Free-Form Text | × | × | \- |
| 1099 Eligible | Check Box | \- | × | \- |
| Tax ID | Free-Form Text | \- | × | \- |
| Legal Name | Free-Form Text | \- | × | \- |
| Supervisor | List/Record | \- | \- | × |
| Soc. Sec. # | Free-Form Text | \- | \- | × |

## Source From Ship To {#bridgehead_N2845962}

When you select Ship To, information is sourced from the customer record selected in the **Ship To** field of **purchase** transactions.

Note:

To source correctly, select the Employee list in the List/Record field.

| **Field** | **Type** |
| --- | --- |
| Name | Free-Form Text |
| Bill To | Text Area |
| Ship To | Text Area |
| Phone | Phone Number |
| Fax | Phone Number |
| Email | Email Address |
| City | Free-Form Text |
| State | Free-Form Text |
| Zip | Free-Form Text |
| Country | Free-Form Text |
| Sales Rep | List/Record |
| Expected Close Date | Date |
| Renewal Date | Date |
| Contact | Free-Form Text |
| Alt. Contact | Free-Form Text |
| Alt. Phone | Phone Number |
| Balance | Currency |
| Credit Limit | Currency |

## Source From Sales Rep {#bridgehead_N2846519}

When you select Sales Rep, information is sourced from the employee record selected in the **Sales Rep** field of **customer** records.

Note:

To source correctly, select the Employee list in the List/Record field.

| **Field** | **Type** |
| --- | --- |
| Name | Free-Form Text |
| Bill To | Text Area |
| Phone | Phone Number |
| Email | Email Address |
| City | Free-Form Text |
| Country | Free-Form Text |
| Supervisor | List/Record |
| Soc. Sec. # | Free-Form Text |

### Related Topics

-   [Available Standard Fields and Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2843906.html)
-   [Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2846812.html)
-   [Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2849333.html)
-   [CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2849651.html)
-   [Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2850856.html)
-   [Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2851231.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

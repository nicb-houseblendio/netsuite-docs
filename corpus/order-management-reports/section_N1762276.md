---
id: "section_N1762276"
type: "section"
title: "Using Gross Profit Fields on Transaction Forms"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Using Gross Profit Fields > Using Gross Profit Fields on Transaction Forms"
parent: "section_N1762134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html"
anchors: []
sha256: "bb6a55fd952b5ec7c41b870658ab308c06d117df006ec66966d1d4976bc9f150"
---

When the Gross Profit feature is enabled, the following standard transaction forms display gross profit fields: Cash Refund, Cash Sale, Credit Memo, Estimate, Invoice, Opportunity, Return Authorization, and Sales Order.

If you use custom transaction forms, you must add these fields to the forms to see them. For information about adding these fields to customized transaction pages, see [Creating Custom Transaction Form HTML Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873464.html#subsect_163733107381).

The following table describes gross profit fields that may be available on transaction forms. The table includes whether each field is available for the transaction as a whole, at the line level for specific items, or both. Line level fields for Gross Profit are available on the Items subtab. Transaction level fields are located on the Accounting subtab.

| Field Name | Level | Description |
| --- | --- | --- |
| Cost Estimate Type | Line | Cost estimate type for the item, as defined in the item record. Users with the Override Estimated Costs on Transactions permission can edit this value. |
| Est. Extended Cost | Transaction and Line | Estimated cost of the specific number of items; estimated unit x quantity = estimated extended cost. |
| Est. Gross Profit | Transaction and Line | Read-only field that equals the revenue amount minus the Est. Cost. At the header level, it equals the gross profit of all lines, factoring in transaction-level discounts and markups. |
| 
Est. Gross Profit Percent

(Estimated Gross Profit Margin as a percentage)



 | Transaction and Line | Read-only field that equals the Est. Gross Profit divided by revenue, expressed as a percentage. At the header level, it equals the gross profit percent of all lines, factoring transaction-level discounts and markups. |
| Est. Unit Cost | Transaction | A read-only field that displays the estimated unit cost, based on the cost estimate type for the item. The estimated unit cost x quantity = estimated extended cost. |

### Related Topics

-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)
-   [Using Gross Profit Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762134.html)
-   [Including Gross Profit Values in Reports, Searches, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1763752.html)
-   [Using Gross Profit Values in CSV Import, SOAP Web Services, and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1326010"
type: "section"
title: "Contract Renewals Process"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Contract Renewals Process"
parent: "chapter_N1319596"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html"
anchors: []
sha256: "397be8d715274e6ba5685174ebf50346a367a29f983cf294c9cf8b2842152a3a"
---

On the scheduled run of the script that creates renewal transactions, a renewal sales order is generated for contracts that are within 90 days of its end date. The renewal sales order includes any renewal contract items from the expiring contract that extend to the contract end date. For information about editing renewal transactions, see [Editing a Renewal Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4719408484.html).

Note:

You can change when renewal transactions are generated (Days Before Renewal) and the type of renewal transaction created (Transaction Type to Create) on the **Contract Renewals Creation** subtab of the Contract Renewals Preferences page. To set the these preferences, go to Contract Renewals > Setup > Contract Renewals Preferences. For more information, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

You can also override the Days Before Renewal preference for specific contracts by specifying a value in the **Contract Days Before Renewal** field on the contract record. For more information, see [Editing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448152522.html).

If contract items on the expiring contract are the same, they are combined on the renewal contract. This occurs when additional items are added to a contract some time during its contract term. For items to be combined, the rates on each line must match. For more information, see [Contract Upsell](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326206.html).

If you need to remove an item from a renewal transaction, change the quantity for the line item to 0 (zero) rather than removing the line item. This ensures that downsell is tracked properly and that any invoices created don't include 0 quantity line items.

If you're provisioning based on fulfillment transactions, transaction line items with zero quantity can be a signal to de-provision those items. If you're provisioning based on contract items, you can signal items to de-provision with negative-quantity contract items.

If there are return authorizations associated with a contract that aren't approved before the active contract renewal, those return authorizations aren't reflected in the renewal. For more information, see [Contracts and Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326489.html).

You can create reminders or saved searches for your dashboard to alert you when renewal transactions are generated. You can base your reminder on transactions with the Order Type set to **Renewal**. For more information, see [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html).

Software Vertical Contract Renewals SuiteApp also supports renewing contracts on demand by clicking the **Renew Now** button on a contract record. For more information, see [Renewing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460263181.html).

To better understand the contract renewal process, see [Contract Renewal Sample Business Case](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4460211117.html).

### Related Topics

-   [Contract Renewals Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4442063121.html)
-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html)
-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Creating a New Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325805.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)
-   [Editing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448152522.html)
-   [Renewing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460263181.html)
-   [Contract Upsell](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326206.html)
-   [Contracts and Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326489.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

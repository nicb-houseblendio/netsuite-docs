---
id: "section_N3436356"
type: "section"
title: "Shared Internal and External IDs"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services > Shared Internal and External IDs"
parent: "section_N3428663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html"
anchors: []
sha256: "7172308efc0cd60a3f3fed8bcec21531a0860914efd9fdf5fe31b6ae984db9fe"
---

System-generated internal IDs and custom external IDs are shared among records belonging to the same high-level group. Therefore, when referencing a record using RecordRef, providing the system internal ID or custom external ID without specifying the record type is sufficient to uniquely identify the record within a specific group.

Note:

For information about displaying internal IDs, see [Setting the Internal ID Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423996.html).

External IDs must be unique across the whole record group, not only within a record type. For example, an external ID for a customer must not be reused for any other customer or for any other entity record, including contacts, employees, groups, partners, or vendors. To avoid clashes within record groups, use a consistent format for constructing your external IDs.

The following table provides the list of these high-level groups and the records belonging to each group.

| Record Group | Record Types |
| --- | --- |
| Account | Account; Tax Account |
| Allocation Schedule | Allocation Schedule; Intercompany Allocation Schedule |
| Entity | Contact; Customer; Employee; Entity; Entity Group; Job; Lead; Other Name; Partner; Project Template; Prospect; Vendor |
| Entity Status | Customer Status; Job Status |
| Event | Activity; Campaign; Case; Event; Issue; Manufacturing Operation Task; Phone Call; Project Task; Resource Allocation; Sales Campaign; Solution; Task |
| Inbound Shipment | Bulk Ownership Transfer; Inbound Shipment; Receive Inbound Shipment |
| Inventory Item | Assembly/Bill of Materials; Description Item; Discount Item; Download Item; Expense Item; Gift Certificate Item; Inventory Part; Item; Item Group; Kit Item; Lot Numbered Assembly/Bill of Materials; Lot Numbered Inventory Item; Markup Item; Non-Inventory Part; Non-inventory Item for Purchase; Non-inventory Item for Resale; Non-inventory Item for Sale; Other Charge Item; Other Charge Item for Purchase; Other Charge Item for Resale; Other Charge Item for Sale; Payment Item; Serialized Assembly/Bill of Materials; Serialized Inventory Item; Service; Service Item for Purchase; Service Item for Resale; Service Item for Sale; Subscription Plan; Subtotal Item; Tax Group |
| Payroll Batch | Payroll Batch; Payroll Batch - Add Employees |
| Project Revenue Rule | Fixed Amount Project Revenue Rule; Labor Based Project Revenue Rule; Percent Complete Project Revenue Rule |
| Revenue Recognition Schedule | Amortization Schedule; Amortization Template; Revenue Recognition Schedule; Revenue Recognition Template |
| Timeline | Manufacturing Planned Time; Time; Time Entry |
| Transactions | Advanced Intercompany Journal Entry; Assembly Build; Assembly UnBuild; Bin Transfer; Bin Worksheet; Blanket Purchase Order; Cash Refund; Cash Sale; Check; Commission; Credit Card Charge; Credit Card Refund; Credit Memo; Custom Transaction; Customer Deposit; Customer Payment; Customer Payment Authorization; Customer Refund; Deposit; DepositApplication; Estimate; Expense Report; Fulfillment Request; FxReval; GL Impact Adjustment; Intercompany Journal Entry; Intercompany Transfer Order; Inventory Adjustment; Inventory Cost Revaluation; Inventory Count; Inventory Status Change; Inventory Transfer; Inventory Worksheet; Invoice; Item Fulfillment; Item Receipt; Journal Entry; Opportunity; Ownership Transfer; Partner Commission; Paycheck; Paycheck Journal; Purchase Contract; Purchase Order; Request For Quote; Requisition; Return Authorization; Revenue Arrangement; Revenue Commitment; Revenue Commitment Reversal; Revenue Contract; Sales Order; Statement Charge; Statistical Journal Entry; Store Pickup Fulfillment; Transaction; Transfer; Transfer Order; Vendor Bill; Vendor Credit; Vendor Payment; Vendor Request For Quote; Vendor Return Authorization; Work Order; Work Order Close; Work Order Completion; Work Order Issue |

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
-   [Search Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html)
-   [External IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

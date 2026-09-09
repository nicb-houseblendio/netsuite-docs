---
id: "section_N2373552"
type: "section"
title: "Vendor Bill Approvals"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Approvals"
parent: "chapter_N2370131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html"
anchors: ["bridgehead_N2373620", "procedure_N2373860", "bridgehead_N2373915", "bridgehead_N2373978"]
sha256: "82b0a02066493313894d802ccd401b1c14f93f2dcf2dedca0e31e0f7d86ec99d"
---

You can require approval for vendor bill processing. When you require approval before payment is issued, you can verify the billed amounts and quantities. To manage billing variances, you can compare amounts and quantities shown on vendor bills, item receipts, and purchase orders.

For example, your company's finance manager received a bill from the vendor Smith Widgets. The manager wants to verify that the payment amount requested on the vendor bill correctly corresponds to the purchase order amount. They know that the original purchase order showed five widgets at a price of $10 each. They want to check against the bill to ensure it also shows five widgets at a price of $10 each. Sometimes variances may occur, such as the following:

-   The vendor bill for the order may show five widgets at $13 each.
    
-   The vendor bill for the order may show ten widgets at $10 each.
    

In both of the preceding cases, the value of what was received doesn't match the original purchase order. If a bill is received with variances such as these, the finance manager must know this information. The manager must ensure that the payment being sent to the vendor properly matches what was received.

After the vendor bill correctly reflects the value of the goods received, the bill can be approved and a payment sent to the vendor.

Note:

Vendor bill approval requires the Vendor Bill Approval, Bills, and Find Transaction permissions.

After a vendor bill is entered against a purchase order, an additional bill can"t be entered against the same purchase order items. This is true regardless of the status of that vendor bill. The first bill must be processed or canceled.

To approve a vendor bill, open it in Edit mode. You can"t approve a bill in View mode.

## Vendor Bill Approval Status {#bridgehead_N2373620}

The table below shows how the status of a vendor bill impacts the function of transaction lines on the bill.

| Status | Accounting impact (AP, asset) | Inventory impact (for standalone bills) | Counts towards outstanding bill quantity on the purchase order |
| --- | --- | --- | --- |
| Pending Approval | None | None | Yes |
| Rejected | None | None | None |
| Approved | Yes | Yes | Yes |

## Standard or Custom Approvals {#procedure_N2373860}

You can enforce approval processes for vendor bills in the two following ways:

-   [Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374450.html)
    
    Set an approval status on vendor bills.
    
-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
    
    Create a custom SuiteFlow workflow to require approval.
    

## Standard Vendor Bill Approval {#bridgehead_N2373915}

When you use the Payables feature, your vendor bills show an Approval Status field.

The default approval status can be set to either Pending Approval or Approved. Bills will default to show an Approved status, but you can set a new default approval status. For more information, see [Setting the Default Vendor Approval Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374176.html).

Vendor Bills with a status of Pending Approval can be approved or be canceled. A vendor bill that is canceled is not processed for payment.

You can use standard approval for vendor bills, regardless of whether you enable SuiteFlow for other purposes.

## Custom Vendor Bill Approval Routing Using SuiteFlow {#bridgehead_N2373978}

For more complex approval requirements, you can use SuiteFlow workflow management when you enable the Vendor Bill preference for Approval Routing. Then, you have the option of creating a custom SuiteFlow workflow to process vendor bills.

A SuiteFlow workflow enables you to tailor more flexible processes in a customized workflow that meets your specific approval routing needs. Your workflow may require action from specific employees, showing buttons on forms at certain stages, or sending email based on actions taken.

For example, you can set up a workflow for approvals based on variances between the purchase order and the vendor bill. You might set up workflows to process approvals using a non-sequential approval process or conditionalized routing.

For information about using SuiteFlow for vendor bill approvals, see [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html).

### Related Topics

-   [Bulk Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374794.html)
-   [Standard Vendor Bill Approval FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375312.html)
-   [Entering a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161968486146.html)
-   [Bill Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164726334180.html)
-   [Differences Between Bills and Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370776.html)
-   [Receiving Inventory in Advance of a Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370995.html)
-   [Canceling a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375066.html)
-   [Vendor Bill Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161070688350.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2375066"
type: "section"
title: "Canceling a Vendor Bill"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Canceling a Vendor Bill"
parent: "chapter_N2370131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375066.html"
anchors: ["bridgehead_1513701472"]
sha256: "e57d95664d6d61ad4cf56a74ca8c8e085579d8c125bee971818328e2e33e5de0"
---

You can review a vendor bill and decide it shouldn't be approved for payment. In such cases, you can cancel the bill. The Cancel button only appears on the form in View mode when the status of the bill is Pending Approval.

#### To cancel a vendor bill:

1.  Go to _Transactions > Payables > Approve Bills_.
    
2.  Click the **Cancel Bill** button.
    
    A popup warning asks you to verify that you do want to cancel the vendor bill.
    
    Note:
    
    After you verify the cancellation, the Canceled status can"t be changed.
    

When you cancel a vendor bill, the following applies:

-   A canceled bill remains recorded in the system but is not processed for payment.
    
-   Links to purchase orders are retained for audit purposes.
    
-   The quantities and amounts are not cleared from the transaction form. They are preserved to be referenced or copied.
    

Note:

Also note that a canceled vendor bill is not applied as billed against the purchase order. For example, a purchase order is entered for 20 units. When 20 units are received, a vendor bill for 20 units is created and saved. Then, the purchase order status changes to fully billed. Later, when that vendor bill is canceled, the purchase order status changes to the appropriate status as if the vendor bill was never entered. Depending on related transactions, the new status could revert to Pending Billing.

## Editing or Copying a Canceled Vendor Bill {#bridgehead_1513701472}

A vendor bill can be edited or copied when it has a canceled status. For example, you may add a Memo to indicate why the vendor bill was canceled.

Using Edit mode, a vendor bill can be deleted or all fields can be edited, including adding or editing line-item data. Any changes made to a canceled vendor bill are strictly for reference.

When you copy a canceled vendor bill, the new copy has a Canceled status by default. However, the new copy initially appears in Edit mode. You can change the approval status to Pending Approval or Pending Receipt before you save it the first time. After you save the form, the approval status updates.

### Related Topics

-   [Entering a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161968486146.html)
-   [Bill Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164726334180.html)
-   [Differences Between Bills and Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370776.html)
-   [Receiving Inventory in Advance of a Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370995.html)
-   [Vendor Bill Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161070688350.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)
-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)
-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

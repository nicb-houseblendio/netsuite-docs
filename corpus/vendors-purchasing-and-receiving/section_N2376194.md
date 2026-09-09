---
id: "section_N2376194"
type: "section"
title: "Vendor Bill Approval Workflow"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Approval Workflow"
parent: "chapter_N2370131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html"
anchors: ["bridgehead_N2380082", "procedure_N2380587", "procedure_N2380650", "bridgehead_N2380718", "bridgehead_N2380766", "bridgehead_N2380778"]
sha256: "b087d7ea9505c5043891820c679cc20f11b3f3b622688af3a85c0bf795e45156"
---

Install the Vendor Bill Approval Workflow as part of NetSuite Approvals Workflow SuiteApp to use a pre-built custom workflow for managing vendor bill approvals. The workflow helps you identify discrepancies between vendor bills you enter and their originating purchase order before payment is issued for the bill.

The workflow is a part of NetSuite Approvals Workflow SuiteApp with Bundle ID 537941. For information about how to install the NetSuite Approvals Workflow, see [Installing the NetSuite Approvals Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096250993.html#bridgehead_4096259084). This workflow is an extension of the Payables feature.

After you install the NetSuite Approvals Workflow, your account is changed in the following ways:

1.  The Vendor Bill Approval workflow is initiated
    
    For details on this workflow, read Vendor Bill Approval Workflow below.
    
2.  Four new saved searches are available.
    
    For details on this workflow, read Saved Searches below.
    

## Vendor Bill Approval Workflow {#bridgehead_N2380082}

The Vendor Bill Approval initiates a workflow that examines vendor bills you enter in your NetSuite account. The workflow identifies cases where a vendor bill has a quantity or cost discrepancy between the bill and purchase order.

-   A bill that doesn't have discrepancies is set to have an Approved status.
    
-   A bill that has discrepancies is flagged for an exception. It is required to go through a review and approval process before a payment can be issued.
    
-   A bill that is created without a purchase order is automatically set to have a Pending Approval status and added to the approval queue.
    

For example, your finance controller wants to implement controls for vendors bills received from vendors and installs the Vendor Bill Approval Workflow. The following transactions are entered:

|  | Purchase Order | Vendor Bill |
| --- | --- | --- |
| **Quantity** | 10 widgets | 10 widgets |
| **Amount** | $100 | $100 |

The quantity and amount of the vendor bill matches the purchase order, so this bill is set to Approved and can be paid.

Next, the following transaction is entered:

|  | Purchase Order | Vendor Bill |
| --- | --- | --- |
| **Quantity** | 10 widgets | 10 widgets |
| **Amount** | $100 | $300 |

For the above, the amount billed doesn't match the amount on the purchase order. This discrepancy is flagged as an exception and the bill is set to a Pending Approval status. The finance controller must review the bill and PO to find out why they do not match before the bill is paid.

The following transactions are also entered:

|  | Purchase Order | Vendor Bill |
| --- | --- | --- |
| **Quantity** | 10 widgets | 100 widgets |
| **Amount** | $100 | $1000 |

For the above, both the quantity and amount of the bill do not match the purchase order. This bill is set to Pending Approval for review before payment.

If you need a more comprehensive way of validating a vendor bill, you can use the 3 Way Match Vendor Bill Approval Workflow. For more information, see [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html).

## Bundle Exceptions {#procedure_N2380587}

The following shows the exceptions flagged by the Vendor Bill Approval Workflow. When one or more of these conditions method are met, the bill is set to have a Pending Approval status.

-   Partial Receipt Quantity on Purchase Order
    
    If the order being billed includes quantities not fully received, the status is Pending Approval.
    
-   Purchase Order - Bill Quantity Exception
    
    If the item quantity on the bill is greater than the item quantity on the purchase order, the status is Pending Approval.
    
-   Purchase Order - Bill Amount Exception
    
    If the amount billed for an item is greater than the amount for the item on the purchase order, the status is Pending Approval. This comparison is made on a per-line basis.
    

When a vendor bill is flagged for an exception, NetSuite notes this by adding an exception message in the Memo field on the transaction.

A vendor bill that is flagged for any of these exceptions has its approval status set to Pending Approval. A supervisor must then approve the vendor bill to enable it to be processed for payment.

Note:

The workflow is applied to both inventory and non-inventory item types.

## Approval {#procedure_N2380650}

If a vendor bill is not flagged with any exceptions, the bill status is set to Approved and it can be processed for payment.

If a vendor bill is flagged and set to a Pending Approval status, a supervisor with appropriate permission must then approve the vendor bill.

A supervisor is able to approve vendor bills if they have the Edit permission for both of the following:

-   Vendor bill
    
-   Approve vendor bill
    

For information about how to approve a vendor bill, see [Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374450.html).

## Saved Searches {#bridgehead_N2380718}

After the workflow is installed, the following new saved searches are available in your account:

-   Vendor Bill PO Amount Check
    
-   Vendor Bill PO Quantity Check
    
-   Vendor Bill PO Partial Rcpt QTY Check
    
-   Vendor Bill Standalone Check
    

These reports can be viewed at Reports > Saved Searches > All Saved Searches.

## Availability {#bridgehead_N2380766}

The Vendor Bill Approval Workflow is a managed bundle and is automatically updated whenever there are updates. These issue fixes and enhancements are available after the bundle is updated in your account.

## Customization {#bridgehead_N2380778}

After you have installed the Vendor Bill Approval Workflow, you can optionally customize the workflow used to determine exceptions. You can also customize the new saved searches. For more information, see [Customizing for the Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381204.html).

### Related Topics

-   [Installing the Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2380890.html)
-   [Entering a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161968486146.html)
-   [Bill Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164726334180.html)
-   [Differences Between Bills and Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370776.html)
-   [Receiving Inventory in Advance of a Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370995.html)
-   [Canceling a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375066.html)
-   [Vendor Bill Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161070688350.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)
-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

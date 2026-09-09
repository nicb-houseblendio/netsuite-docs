---
id: "section_N2473830"
type: "section"
title: "Web Store Checkout Process with PayPal Express Checkout"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > PayPal Integration and Express Checkout for Commerce Web Stores > Web Store Checkout Process with PayPal Express Checkout"
parent: "section_N2470255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2473830.html"
anchors: []
sha256: "64cdd6e5e5538d5bb4d8c70c936c2f17b17c5ab8909d1e1861eaf9a78b988a34"
---

PayPal Express Checkout lets your web store customers pick their payment method at various points in the checkout process, helping lower cart abandonment.

The PayPal Express Checkout button appears in the shopping cart and address information page. If customers pick PayPal on the payment methods page, they'll see the Pay with PayPal button, with Express Checkout functionality, on the last checkout page of checkout.

Customers click the PayPal Express Checkout button and are temporarily redirected to the PayPal site to confirm their payment and address details.

The following diagram shows the PayPal Express Checkout process for Commerce websites:

![redirection to PayPal site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/Transactions/PaypalWorkFlowchart.png)

After the sales order record is created in NetSuite, the following PayPal fields are displayed on the sales order form:

| Field Name | Field ID | Field Type | Description |
| --- | --- | --- | --- |
| PayPal Status | paypalstatus | Text | Shows the payment status from PayPal. Possible values are:
-   None - No status.
-   Canceled-Reversal - The reversal was canceled, so the funds from the reversed transaction were returned to you. For example, you won a dispute with the customer and the funds for the reversed transaction have been returned to you.
-   Completed - Payment's complete and the funds are in your account. This is the only status for point-of-sale transactions.
-   Denied - You denied the payment.
-   Expired - The authorization period for this payment expired.
-   Failed - The payment has failed. This happens only if the payment was made from your customer's bank account.
-   Pending - The payment's pending.
-   Refunded - You refunded the payment.
-   Reversed - A payment was reversed due to a chargeback or other type of reversal. The funds have been removed from your account balance and returned to the buyer.
-   Processed - The payment's been accepted.
-   Voided - The authorization for this transaction was voided.

 |
| PayPal Order ID | paypalorderid | Text | The ID of the order submitted through PayPal Express Checkout. Populated from the PayPal response. |
| PayPal Tran. ID | paypaltranid | Text | Unique transaction identification number of the payment. Populated from the PayPal response. |
| Authorization ID | paypalauthid | Text | Authorization identification number. Populated from the PayPal response. |
| Process PayPal Payment | paypalprocess | Checkbox | If checked, PayPal processes the payment or refund. If not checked, the info is saved in NetSuite but the data entered in the other PayPal fields will be stored in NetSuite but not sent to PayPal. This is checked by default for PayPal Express Checkout orders. |
| Override PayPal Settings | paypaloverride | Checkbox | If checked, the user can override the **PayPal Tran. ID** and **PayPal Status** fields. If not checked, these field IDs are disabled and populated with the PayPal response. |

### Related Topics

-   [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

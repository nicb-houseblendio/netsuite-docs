---
id: "bridgehead_N1569446"
type: "bridgehead"
title: "Payment Events"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Payment Events"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1569446.html"
anchors: ["bridgehead_4226219524", "bridgehead_4262379818", "bridgehead_1491395929", "bridgehead_1491396826", "bridgehead_4709266644"]
sha256: "cddee6eda9dff067119ee2339aad1efc0d5ebc43651d0f501a5a8979ec479306"
---

On the Billing subtab of a sales order, the Payment subtab displays a list of all payment event activity that has occurred for the order with the most recent event at the top of the list. Each payment event has a link to view the payment event details. Payment event details include the request information, the response for the request, the payment status, and the raw transmission details.

![Payment subtab and an example Payment Event Details page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/paymentevent.png)

Use the Payment subtab to review the summary information about the gateway communication requests and responses, such as the payment event, the result, and reason for the result. Drill down for full payment event details, including the response code, authorization code, address verification (AVS) and card security code (CSC) results, payment status, and the raw request and response transmission details.

## Populating the invoice\_number in the Request Details for MerchantE {#bridgehead_4226219524}

If you select a MerchantE credit card processing profile, the invoice\_number parameter is always populated in the request NetSuite sends to the gateway. Depending on the page where you record the customer payment, this parameter is populated by one of the following fields:

-   On a Sales Order page:
    
    -   PO#
        
    -   Order#
        
    -   Internal ID
        
    
    If the PO# field is empty, the parameter uses Order#. If the Order# field is empty, the parameter uses the internal ID of the record. For more information about the internal ID, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)
    
-   On an Invoice page or on a Customer Payment page:
    
    -   PO#
        
    -   Invoice#
        
    -   Internal ID
        
    
    If the PO# field is empty, the parameter uses the Invoice#. If the Invoice# is empty, the parameter uses the internal ID of the record.
    
-   On a Cash Sale page:
    
    -   Check#
        
    -   Sale#
        
    -   Internal ID
        
    
    If the Check# field is empty, the parameter uses Sale#. If the Sale# field is empty, the parameter uses the internal ID of the record.
    
-   On a Customer Deposit page:
    
    -   Deposit#
        
    -   Internal ID
        
    
    If the Deposit# field is empty, the parameter uses the internal ID of the record.
    
-   On a Customer Refund page, the parameter uses the internal ID of the record.
    

## Populating Level III Item Data with CyberSouce Decision Manager {#bridgehead_4262379818}

If you use a CyberSource processing profile with Decision Manager enabled, line-level data is populated in the request NetSuite sends to the gateway. This includes the product name, product code, item name, and others. You can view these details in the Raw Request section of the payment event.

The following table lists some of the parameters populated in the request and their corresponding item fields.

Note:

The populated data vary depending on the transaction type.

| Payment Event Parameter \* | Item Field | Notes |
| --- | --- | --- |
| item\_#\_productName | Display Name/Code |  |
| item\_#\_productSKU | Item Name/Number |  |
| item\_#\_productCode | UPC Code | If the UPC Code field is empty, item\_#\_productCode takes the value **default**. |
| item\_#\_productRisk | Fraud Risk | If the Fraud Risk field is empty, item\_#\_productRisk isn't populated in the payment event. |
| \* In the payment event, the # mark is replaced by a number that indicates the order of the line item. |

Important:

With CyberSource Decision Manager, line-level data is sent only for the authorization request. To send line-level data with capture and sale requests, you must have the Purchase Card Data feature enabled. For more information, see [Accepting Purchase Cards (Level II and Level III Credit Cards)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html#bridgehead_N1569481).

## Understanding the P/N Ref. Field {#bridgehead_1491395929}

The P/N Ref. field contains an identifier of the a request that NetSuite sends to a payment gateway. This identifier is unique. You can use this identifier to inquiry about a certain request at the gateway's back office.

When NetSuite sends a request that references another request, NetSuite includes the P/N Ref. of the original request. For example, when NetSuite sends a capture request, the P/N Ref. of the original authorization request is included.

You can enter or edit a P/N Ref. manually to record requests that occurred outside of NetSuite. To enter or edit a P/N Ref. manually, you must check the CC Approved box. For more information, see [Recording Payment Events that Occurred Outside of NetSuite](#bridgehead_1491396826).

## Recording Payment Events that Occurred Outside of NetSuite {#bridgehead_1491396826}

To keep a record of authorizations or other payment transactions that occurred outside of NetSuite, you can create cash sales, sales orders, or other payment transactions and manually enter the P/N Ref. and other payment details on the Payment subtab.

To record payment events for these transactions without the [Payment Instruments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html) enabled, you **must** check the CC Approved box. If you don't check the CC Approved box, a payment event isn't created for the transaction, and the payment details are not preserved on the transaction. If you check the CC Approved box, you must provide either a payment card number or a P/N Ref identifier.

If you enable the [Payment Instruments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html), the Handling mode field replaces the functionality of checking the Charge Credit Card and CC Approved boxes. Select **Record External Event** to create a NetSuite record of a payment event that took place outside of NetSuite, for example in an e-commerce solution that authorizes payments outside of NetSuite.

Note that although the Charge Credit Card and CC Approved fields are no longer visible on the transaction after you enable Payment Instruments, the fields remain available for scripting.

For information about other handling modes, see the help topic [Using the Handling Mode Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158453792666.html).

## Viewing Gateway Asynchronous Notifications {#bridgehead_4709266644}

During payment processing, the communication between NetSuite and a payment gateway is sometimes asynchronous. For example, some alternative payment methods that use external checkout require asynchronous processing. The gateway can also send an asynchronous request to NetSuite to update the voiding status of a transaction.

To view a list of asynchronous notifications received from payment gateways, go to _Transactions > Management > View Gateway Asynchronous Notifications_.

### Related Topics:

-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1569326"
type: "section"
title: "Accepting Credit Card Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Accepting Credit Card Payments"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html"
anchors: ["bridgehead_N1569481", "bridgehead_N1569782", "bridgehead_N1569813"]
sha256: "74c215e237610f0755cdba65ced1324b5b49d782a961943bd49d216a2a4c50ea"
---

You can enter credit card payments on:

-   Billing subtab on a sales order
    
-   Payment Method subtab on the new Payment page. From an invoice, click Accept Payment
    
-   Billing subtab on a cash sale
    

When accepting credit card payments, the system immediately notifies you if the card was accepted or rejected. You don't have to check the Card Card Approved box. If the card is rejected, you are notified with the reason for rejection.

For more information, see the Payment section of [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html) and [Entering a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244457.html).

When you save an order with the Get Authorization box checked on the Payment subtab, NetSuite sends an authorization request to your credit card gateway to verify the card is valid and place a hold on the cardholder's funds for the order. The hold on the cardholder's funds is immediate.

When you bill the order, NetSuite sends a capture request to the gateway. By the end of every day, the gateway processes all capture requests, which settles the money from the cardholder's issuing bank account to your merchant bank account.

The credit card gateway attempts to verify that the cardholder's address and security code match the order billing information submitted. The gateway returns a response with the results. If the card information is authorized, NetSuite displays the results on the Payment subtab and saves the order.

![Sample credit card authorization response returned by the payment gateway.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/cardapproved.png)

If the gateway returns a response other than card approved, NetSuite follows the authentication settings and order verification rules, if any, set up on the gateway profile to determine what action to take for the sales order. The possible actions are:

-   Save the order for fulfillment
    
-   Place the order on payment hold for review and further action
    
-   Cancel the order
    

Note:

You can automate the capture of credit card payments for billed and fulfilled sales orders. For more information, see [Auto-charge Credit Card](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1500449969.html).

## Accepting Purchase Cards (Level II and Level III Credit Cards) {#bridgehead_N1569481}

Businesses use purchase cards, also called Level II and Level III cards, to streamline their procurement process. If your customers use business, corporate, or government GSA purchasing cards, then you can reduce your credit card processing expense by accepting these type of payments.

For every credit card authorization, NetSuite automatically sends Level I data, which covers basic info like the transaction amount and merchant name.

To process Level II purchase cards, processors need extra details like the tax code, customer code, and a few merchant codes.

Level III cards need even more data sent with the authorization request to qualify for lower processing rates. This includes detailed item, freight, and destination information, as well as Level II data.

## Using the Purchase Card Data Module {#bridgehead_N1569782}

With the Purchase Card Data module, NetSuite identifies when payment is made with a purchase card and sends the additional Level III order line-item data. This enables you to take advantage of potential lower card processing fees.

When you enter a credit card payment for a customer, NetSuite determines, based on the card's bank identification number (BIN), whether it is a purchase card. It then passes the extended transaction data along with the payment authorization request for processing.

On the Payment subtab of a transaction or the Payment Method subtab of a customer payment, NetSuite automatically checks the Purchase Card BIN box when it identifies that the credit card is a purchase card. The Process as Purchase Card box is also checked. When both boxes are checked, NetSuite processes the credit card payment as a purchase card.

If NetSuite doesn't recognize the card as a purchase card, you can manually check the Process as Purchase Card box to send Level III data (which includes Level II data) with the payment request. You can also clear the Process as Purchase Card box to process the payment without sending Level III data.

The Purchase Card Data module is currently available for use only with the following processing solutions:

-   CyberSource Acquiring (using GPN)
    
-   MerchantE
    

Note:

The Purchase Card Data module helps you meet credit card industry requirements for these transaction types, as defined by Visa, MasterCard, and American Express.

NetSuite doesn't make any claims about your ability to meet specific Visa, MasterCard, or American Express interchange qualification goals.

Visa, MasterCard, and American Express set their own interchange qualification rules, and your merchant services provider handles the related fees and expenses.

Interchange qualifications include requirements that are outside of NetSuite's control. If you have questions about interchange, transaction qualifications, or card processing costs, reach out to your merchant services provider.

## Setting Up Purchase Card Processing {#bridgehead_N1569813}

Complete the following to set up and use the Purchase Card Data module to process level II and level III credit cards through CyberSource and MerchantE:

1.  Provision the feature by contacting your NetSuite account manager for more details and pricing information for this module.
    
2.  Enable the Purchase Card Data feature in NetSuite:
    
    1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
        
    2.  On the **Transactions** subtab, under Payment Processing, check the **Send Purchase Card Data** box. This box is available only after your account has been provisioned for this feature.
        
    3.  Click **Save**.
        
3.  Check the **Process Purchase Card Data** box on the CyberSource and MerchantE credit card processing profiles you will use to process purchase cards. See instructions for setting up [CyberSource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573308.html) and [MerchantE](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1576356.html).
    

After completing the steps to provision and set up the feature in your account, you can process credit card payments from purchase cards.

### Related Topics

-   [Accepting Purchase Cards (Level II and Level III Credit Cards)](#bridgehead_N1569481)
-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)
-   _Credit Card Processing Gateway FAQ_
    
-   [Issuing Credit Card Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1569907.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)
-   [Voiding Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1570067.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "bridgehead_N1566955"
type: "bridgehead"
title: "Payment Gateways"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Payment Gateways"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html"
anchors: ["bridgehead_4122004523", "section_N1577424", "subsect_160692470774", "procedure_N1577574", "procedure_N1577608", "procedure_N1577640", "procedure_N1577682", "procedure_N1577737", "bridgehead_N1577775", "procedure_N1577791", "procedure_N1577832"]
sha256: "c57d640cdf1e32dff19ee866ddfe1f1e47dc7651a3e2e8ca83ecb545500db512"
---

NetSuite supports a variety of payment acceptance or customer payment solutions. These pre-integrated SuitePayments partner solutions can be found at [SuiteApp.com](http://suiteapp.com/business-needs/Payment-Acceptance).

Click on a listed partner solution to see more details. To inquire directly with the partner click the **Contact Me** button on the listing.

The legacy SECPay (PayPoint) gateway partner is maintained for existing accounts in NetSuite.

An add-on module is required to use the PayPal Payflow Pro gateway. For information about this module, please contact your account representative.

To set up a credit card gateway, go to _Setup > Accounting > Payment Processing Profiles > New_. For information see [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html).

## Credit Card Gateway Integration {#bridgehead_4122004523}

NetSuite integrates with several credit card gateways to enable you, using your processor, to accept credit card payments from your customers. The gateway manages the flow of data and funds electronically between you, your customer, and the processors involved.

Credit card transactions consist of an initial exchange of data to authorize the transaction and a subsequent transfer of funds. The process begins in NetSuite with a Web site transaction or a traditional sales order. It involves:

-   **Cardholder** - a consumer with a debit or credit card
    
-   **Merchant** - a person or business that sells goods or services to a customer
    
-   **Merchant Account (acquiring bank)** - an account with a financial institution that is used by a merchant for collecting proceeds from consumer credit card accounts
    
-   **Payment Gateway (credit card gateway)** - technology that interfaces with the NetSuite credit card checkout system and is responsible for transmitting transaction data securely over the Internet for processing within the credit card processing networks
    
-   **Processor** - a financial institution that provides a financial account to collect proceeds from consumer bank account or credit card payment transactions
    
-   **Credit Card Interchange** - a system of networked computers that manages the processing, clearing, and settlement of credit card transactions including assessing, collecting, and distributing fees between the parties involved; the interchange includes processors, acquiring banks, and issuing banks
    
-   **Cardholder's Issuing Bank** - a financial institution that issues credit cards to consumers
    

For information regarding processing credit card payments from your customers, see:

-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
    
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
    
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
    
-   [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html)
    
-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
    
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
    
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
    
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)
    
-   [Transitioning to a New Gateway and Disabling the Old Gateway](#section_N1577424)
    
-   _Credit Card Processing Gateway FAQ_
    

## Transitioning to a New Gateway and Disabling the Old Gateway {#section_N1577424}

You can change the credit card gateway that you use to process credit card payments in NetSuite.

When you set up a credit card credit card gateway in NetSuite to process customer payments, you have the ability to select the types of transactions the gateway processes. The credit card processing profile page lists types of gateway requests enabled for the processor:

-   **Authorizations** - process requests to place a hold on a credit line for a specified amount until fulfillment is complete
    
-   **Captures** - process charges for authorizations after fulfillment
    
-   **Sales** - process authorization and funds capture for immediate fulfillment of products or services
    
-   **Refunds** - process requests for refunds that reference a previous transaction
    
-   **Credits** - process requests to distribute funds a cardholder with no reference to a previous transaction
    

Manage the transition from one gateway to another by disabling the gateway request types for the old gateway in stages. This enables you to fulfill and bill sales authorized by the old gateway and use the new gateway for new sales authorizations and captures.

To transition from using one credit card gateway to another:

-   [To set up a new gateway:](#procedure_N1577574)
    
-   [To update other settings:](#procedure_N1577608)
    
-   [Partially Disable the Old Gateway](#procedure_N1577640)
    
-   [To process open transactions:](#procedure_N1577682)
    
-   [To fully disable the old gateway:](#procedure_N1577737)
    

## Setting up a New Gateway {#subsect_160692470774}

Prerequisite: Establish a new account with a credit card gateway.

#### To set up a new gateway: {#procedure_N1577574}

1.  Establish a new account with a credit card gateway.
    
2.  Add the new credit card credit card gateway in NetSuite. Verify that all the gateway request types are selected.
    
3.  Test the new account setup.
    
4.  When satisfied that the configuration works properly, clear the Test Mode box. The credit card gateway is now available to process transactions.
    

#### To update other settings: {#procedure_N1577608}

1.  Do a search for assigned credit card processing profiles on customer records. Change or remove any that are set to the old gateway.
    
2.  Set or change the Supporting Merchant Accounts on existing payment methods to include the new gateway.
    
3.  If you have a Web site, set or change the credit card processing profile selected on the Web Site Setup page to the new gateway.
    

## Partially Disable the Old Gateway {#procedure_N1577640}

On the setup page for the old gateway, clear the following gateway request types:

-   Authorizations
    
-   Sales
    
-   Credits
    

The old gateway is still able to capture funds for existing authorizations and process refunds that reference transactions it previously processed. It isn't going to process any new requests for authorizations.

#### To process open transactions: {#procedure_N1577682}

1.  Determine the open sales orders and cash sales that were authorized by the old gateway.
    
2.  When a cash sale is created from a sales order, and the old gateway authorized the sales order, NetSuite processes this as a sale instead of a settlement referencing an authorization.
    
3.  When a refund references a cash sale processed by the old gateway, NetSuite creates a credit.
    
4.  Memorized transactions that reference the old gateway fails and returns an error message telling you to change the credit card processing profile on the base memorized transaction template. For more information, see [Automatic Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html#bridgehead_N565640) and [Memorizing a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html).
    

#### To fully disable the old gateway: {#procedure_N1577737}

1.  After you bill all sales orders authorized by the old gateway, clear the **Captures** box for the credit card gateway. This is generally about 3-7 days after the last new sales order was created.
    
2.  Clear the **Refunds** box after you close the account with the provider.
    
3.  Check the **Inactive** box for the credit card gateway.
    
4.  Close the merchant account for the old gateway.
    

## Resolving Processing Errors for Inactive Gateways {#bridgehead_N1577775}

If you receive an error message that a gateway is inactive when trying to capture funds for a cash sale with an existing authorization, it means you have fully disabled and inactivated the gateway before processing all open transactions from that gateway.

To be able to save a cash sale and capture funds previously authorized you can reactivate the old gateway or select a different gateway to process the order.

#### To process the order and capture funds using the inactive gateway: {#procedure_N1577791}

1.  On the setup page for the inactive gateway, change the Gateway Request Types:
    
    -   Clear the **Inactive** box.
        
    -   Check the **Captures** box.
        
2.  Save the cash sale. This initiates the request for the gateway to capture funds previously authorized for the cash sale.
    

#### To process the order and capture funds using a different gateway: {#procedure_N1577832}

1.  Before saving the cash sale:
    
    -   Clear the **Charge Credit Card** box.
        
    -   Clear the data in **P/N Ref** and **Auth. Code** fields.
        
    -   In the **Payment Processing Profile** field, select an active credit card gateway.
        
    -   Check the **Charge Credit Card** box.
        
2.  Save the cash sale to resubmit the order for payment authorization and funds capture.
    

### Related Topics:

-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

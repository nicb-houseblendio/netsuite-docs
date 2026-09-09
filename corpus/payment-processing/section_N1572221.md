---
id: "section_N1572221"
type: "section"
title: "Setting Up Customer Credit Card Processing"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html"
anchors: ["procedure_N1572251", "procedure_N1572297"]
sha256: "82fc60653d8b9ddde0e5f75d88b952b352333d1c3f2d29490943a7cff0f152f8"
---

Setting up credit card processing enables you to securely process credit card charges in real time directly from your NetSuite account. You can use any number of credit card gateways in your NetSuite account.

If you use NetSuite OneWorld, you can associate any number of credit card gateways with each subsidiary.

## Prerequisites {#procedure_N1572251}

Before you can set up a gateway processor in NetSuite, you'll need an internet-enabled merchant account that works with the credit card gateway you choose.

Merchant accounts and credit card gateways work closely together. NetSuite integrates with several gateways, and some of them offer both merchant accounts and gateway processing. Some merchant accounts only work with certain gateways. For a current list of gateways, see [Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html).

Some merchant accounts only use specific gateways.

Depending on your location, business needs, and selling market, you can either:

-   Select a gateway and then a merchant account that is compatible with the gateway.
    
-   Select a merchant account and use its partnered gateway. The gateway must integrate with NetSuite.
    

Whatever method you choose, you must decide which gateway and merchant account you want to use before you can add credit card gateways on the Payment Processing Profiles page.

You must also create a payment method in NetSuite for each type of credit card you accept. The name of the payment method must be a name that the gateway can identify as a card type used for payment. Don't create a generic payment method called Credit Card. For instructions and a list of card names, see [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html). Later when you add your credit card gateways, you'll associate the payment methods with each gateway you set up.

#### To set up credit card processing in NetSuite: {#procedure_N1572297}

1.  Enable the credit card feature by going to _Setup > Company > Enable Features_.
    
2.  On the **Transactions** subtab in the Payment Processing section, check the **Credit Card Payments** box.
    
3.  Establish a merchant account with a payment gateway. See [Establishing a Merchant Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572500.html).
    
4.  Set up an account with a credit card gateway. See [Setting Up a Merchant Account with a Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572566.html).
    
5.  Add the credit card gateway in NetSuite. See [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html).
    
6.  Set NetSuite payment processing preferences relating to credit cards, at _Setup > Accounting > Accounting Preferences_, on the Items/Transactions subtab. See [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html), [Payment Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html#bridgehead_N1387830).
    
7.  If you have a web store, follow the instructions for assigning a credit card processing profile to your web store in [Set Up Credit Card Payments for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469773.html).
    

### Related Topics:

-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)
-   [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

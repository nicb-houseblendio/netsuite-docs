---
id: "section_N1573049"
type: "section"
title: "SecurePay and SecurePay FraudGuard"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Regional Payment Gateways > SecurePay and SecurePay FraudGuard"
parent: "section_N1577002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573049.html"
anchors: ["bridgehead_4651973159"]
sha256: "172eab83222c664cf04218886e55ab42651897cca7871fa266bdf1c9657cc991"
---

Important:

This is a NetSuite **Integration with Third Party Applications.**

Integration with the SecurePay gateway is available in the Payment Gateway SuiteApp. This specific integration is best suited for use with the NetSuite Australia edition and NetSuite OneWorld accounts with an Australian or New Zealand subsidiary. For more information about the SuiteApp, see [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html).

Note:

The Payment Gateway SuiteApp is automatically provisioned to Australia and New Zealand accounts that are provisioned with the following products: NetSuite Australia, NetSuite JCurve Premium Edition (PRO), NetSuite JCurve Financials Edition (GROW), NetSuite JCurve Edition (GO).

| **Country of operation** | Australia, New Zealand |
| --- | --- |
| **Supported NetSuite processing methods** | Authorization, capture, sale, refund |
| **Other supported features** | 
-   Recurring payments with SecurePay
-   CVV validation with SecurePay and SecurePay FraudGuard
-   Recurring Payments are not supported by SecurePay FraudGaurd Note: Support for CVV validation is available in the Payment Gateway SuiteApp version 3.0 onwards.

 |

## Setup Requirements for SecurePay and SecurePay FraudGuard Integration {#bridgehead_4651973159}

You need the following requirements for installation and setup:

-   The SecurePay with FraudGuard integration enables you to use SecurePay fraud screening rules from within the merchant login. Enable this integration in SecurePay.
    
    Note:
    
    You must have FraudGuard activated for your merchant account before you can set up SecurePay with FraudGuard profiles. Please contact SecurePay for activation of FraudGuard.
    
-   To use CVV validation, you must enable the Use Card Security Code for Credit Card Transactions preference. This preference enables you to accept card security codes for preauthorization and sales transactions. When online shoppers pay using a credit card, they can enter the CVV number. You can then send the payment details with the CVV number to the bank for validation. For more information about this preference, see [Set Up Credit Card Payments for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469773.html).
    
-   Credentials provided by SecurePay: Merchant ID and password.
    
    These credentials used for live transaction processing are different from user login credentials. Use the credentials to set up as many credit card processing profiles for SecurePay as needed.
    

After obtaining your credentials, follow the procedures in the [Setting Up Regional Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html) topic.

### Related Topics:

-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
-   [Regional Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_N1572795)
-   [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html)
-   [AsiaPay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573186.html)
-   [AsiaPay External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609621020.html)
-   [eWAY Rapid](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471740031.html)
-   [PayU Latin America External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4536913874.html)
-   [VeriTrans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3843570937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

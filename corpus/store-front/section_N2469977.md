---
id: "section_N2469977"
type: "section"
title: "Credit Card Payer Authentication for Commerce Web Stores"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > Credit Card Payer Authentication for Commerce Web Stores"
parent: "chapter_N2469683"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469977.html"
anchors: ["procedure_N2470039"]
sha256: "79414dce9903d7bc472ea2744830c3c166e0031a9685a14d58ca6782d5132b78"
---

Credit card payer authentication is available for credit cards used in your Commerce website checkout. With payer authentication, customers can set up a password linked to their credit card. This password helps verify the card's owner and protects you from chargebacks.

When you enable payer authentication, you can add the Verified by Visa, MasterCard SecureCode, and Maestro SecureCode logos to your site. After placing an order, customers are taken to a payer authentication site. They can enter or create a password, or choose to skip this step. They're then sent back to your website's confirmation page, and the order is created in your NetSuite account.

In addition, a Payer Authentication Status field is added to sales orders. For credit card orders on your website, this field shows if authentication was successful, failed, or skipped. For other sales orders, it'll be blank.

Payer authentication is currently offered through these credit card gateways:

-   MerchantE
    
-   CyberSource
    
-   eWAY Rapid
    
-   Payflow Pro
    
-   WorldPay
    

Note:

If you use CyberSource or MerchantE, you'll need to contact them to add payer authentication feature to your account before enabling it in NetSuite. If you use Payflow Pro, you'll need to enroll in PayPal's Buyer Authentication Service through your PayPal Manager account.

Payflow Pro, owned by PayPal, is used for credit card processing. PayPal is the checkout method that enables you to enter or accept payment information.

For information about regional payment gateways, see the Order Management help topic, [Setting Up Regional Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html).

For information about payer authentication for eWAY Rapid, see the Order Management help topic, [Payer Authentication for eWay Rapid](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4651871224.html).

For information about integration with third-party checkout providers, like PayPal Express, see [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html).

#### To enable credit card payer authentication: {#procedure_N2470039}

1.  Go to Setup > Accounting > Financial Statements > Payment Processing Profiles.
    
2.  Click **Edit** next to the credit card gateway you'd like to use for payer authentication.
    
3.  In the Primary area, check **Payer Authentication**.
    
    Note:
    
    Don't check this box if you want to use 3D Secure 2 payment flows on your website. See [3D Secure Payment Authentication for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503444797.html) for more information.
    
4.  Click **Save**.
    

Now, customers will be redirected to a payer authentication site after submitting a credit card order.

### Related Topics

-   [Payment Options for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2469683.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

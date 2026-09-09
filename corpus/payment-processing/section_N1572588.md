---
id: "section_N1572588"
type: "section"
title: "Setting Up Payment Processing Profiles in NetSuite"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Payment Processing Profiles in NetSuite"
parent: "section_N1572221"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html"
anchors: ["bridgehead_0813105039", "bridgehead_4595030256", "bridgehead_4595031963", "bridgehead_4335053679", "bridgehead_N1572795"]
sha256: "a7cb94beccb7bc19b50933252e569f8e8d8f52a826127303a6dc1a1bbe499c42"
---

Set up payment processing profile in NetSuite for each payment card gateway you use. You can set up multiple profiles in NetSuite based on your business needs. You must set up a payment card gateway profile for each settlement currency and merchant bank account your company uses.

NetSuite integrates with the following preferred gateway partners:

-   CyberSource
    
-   MerchantE
    
-   PayPal Payflow Pro (This processor requires an add-on module be enabled in your NetSuite account. For more information, contact your NetSuite account representative.)
    

Note:

NetSuite currently maintains SECPay as a legacy gateway partner only for existing payment card gateways.

NetSuite also integrates with additional regional gateway partners that provide payment card processing services in specific countries. See [Regional Payment Gateways](#bridgehead_N1572795).

Before you set up a payment card processing profile in NetSuite, you must:

-   Establish a merchant account. See [Establishing a Merchant Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572500.html).
    
-   Set up the merchant account with the gateway you will be using in NetSuite. See [Setting Up a Merchant Account with a Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572566.html).
    

#### To set up a payment card processing profile:

1.  Go to _Setup > Accounting > Payment Processing Profiles > New_.
    
2.  Click the **Add Profile** next to the gateway integration you want to set up.
    
    The gateway integration must be installed in your account. Otherwise, Install shows instead of Add Profile.
    
    For instructions for setting up a preferred gateway, see [CyberSource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573308.html) and [MerchantE](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1576356.html).
    
    For information about setting up a regional gateway, see [Setting Up Regional Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html).
    

The new payment card processing profile page includes a section where you select the types of payment requests the gateway will process:

-   **Authentications** - process requests for cardholder authentication when required. The Payment Processing Plug-in must support 3D Secure 2 for the Authentication operation to be available.
    
    Support for 3D Secure 1 ended on October 15, 2022. See [End of Support for 3D Secure 1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_070511571310.html) for more information, including information about migrating your website technologies from 3D Secure 1 to 3D Secure 2.
    
-   **Authorizations** - process requests to place a hold on a credit line for a specified amount until fulfillment is complete.
    
    Warning:
    
    When you use a payment processing profile that doesn't support authorization to process card payments on sales orders, make sure you follow the card acceptance guidelines of your payment card issuer.
    
    If your business involves shipping goods to your customers, you must process the sales order with a payment processing profile that supports authorization. Funds must be deposited only when goods have been fulfilled.
    
    Use a payment processing profile that doesn't support the authorization request on a sales order only when you provide an immediate delivery of goods or services.
    
-   **Captures** - process charges against authorizations after fulfillment.
    
-   **Sales** - process authorization and funds capture for immediate fulfillment of products or services.
    
-   **Credits** - process requests to distribute funds a cardholder without reference to a previous transaction.
    
-   **Refunds** - process requests for refunds that reference a previous transaction.
    
-   **Voids** - process requests for voiding authorizations. Only CyberSource and MerchantE support voiding authorizations.
    

In most cases, select all request types for a gateway to fully use the gateway processing functionality and provide smooth payment card processing for your website. All the gateway request types are enabled by default when you set up a new payment card gateway. For information about how to set these options when changing payment card gateways, see [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424).

Note:

If you select the Sales request and leave the Authorizations request blank, the processing profile will perform a direct sale request. When you select this profile on a sales order, the funds are captured before fulfilling the order. The captured funds are associated with the order as a customer deposit.

## Signing Keys {#bridgehead_0813105039}

Use signing keys to enhance security when using the external checkout payment method.

When your payment provider offers enhanced security for external checkout, they will ask you to enter the signing keys on the payment processing profile.

Enter the key in the Signing Key field. You can use multiple signing keys, revoke signing keys, and define an expiration day.

## Payer Authentication {#bridgehead_4595030256}

Enable the Payer Authentication on a payment processing profile to redirect the shopper to a payer authentication site. On this site, shoppers enter or create passwords for their payment cards. Payer authentication protects you from chargebacks for unauthorized transactions by verifying that the cardholder makes the purchase. This also provides enhanced security for cardholders.

## Allow Request ID to Meet Payment Card Field Requirements {#bridgehead_4595031963}

On a Payment Processing Profile page, check the **Allow Request ID to Meet Payment Card Field Requirements** box to allow payment cards to be charged by referencing the original Request ID when the order is authorized outside of NetSuite.

These are orders passed to NetSuite using SOAP web services. This preference enables the payment card entered on the external order to be charged by referencing the request ID from the originating authorization rather than requiring card information to be present on the sales order in NetSuite.

## Restricting Payment Processing Profiles by Customer Data {#bridgehead_4335053679}

To prevent processing payments with incompatible payment processing profiles, you can show in the Payment Processing Profile field only those payment processing profiles that support all of the following requirements:

-   The selected payment method
    
-   Customer's currency
    
-   Customer's subsidiary (One World accounts only)
    

If you use One World intercompany accounts, this restriction prevents one subsidiary from using another subsidiary's payment processing profiles.

#### To restrict payment processing profiles by customer data:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Items/Transactions** subtab.
    
3.  Under Payment Processing, check the **Use Strict Rules for the Selection of Payment Processing Profiles**.
    
    Important:
    
    When this preference is enabled, it takes precedence over the Restrict Payment Methods by Customer Currency preference on the Shopping subtab of your Website record at _Commerce > Websites > Website List_. This means that even if the Restrict Payment Methods by Customer Currency is disabled, only those payment methods that support the shopper's currency are displayed on your web store.
    
    In addition, if no payment method supports the shopper's currency, no payment method shows on the Payment Information page of your web store. (This is the opposite behavior of the Restrict Payment Methods by Customer Currency preference.)
    
4.  Click **Save**.
    

Now, only compatible payment processing profiles show in the Payment Processing Profile field on the Payment subtab of a sales order, cash sale, or any other transaction that has this subtab.

## Regional Payment Gateways {#bridgehead_N1572795}

NetSuite integrates with payment card gateways that provide card processing services for a specific country or region. To use a regional payment card gateway, the Payment Gateway SuiteApp must be installed in your account. The SuiteApp is automatically provisioned in some accounts. For others, you must install it from _Customization > SuiteBundles > Search & Install Bundles_. For more information about installing the Payment Gateway SuiteApp, see [Installing the Payment Gateway SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html#bridgehead_4537023531).

Note:

Regional payment gateways don't support credit requests.

To learn more, see the following topics:

-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
    
-   [Setting Up Regional Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html)
    

### Related Topics:

-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

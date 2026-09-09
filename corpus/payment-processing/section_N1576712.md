---
id: "section_N1576712"
type: "section"
title: "WorldPay (UK) Limited"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Payment Processing Profiles in NetSuite > WorldPay (UK) Limited"
parent: "section_N1572588"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1576712.html"
anchors: ["procedure_N1576736", "bridgehead_4595104784"]
sha256: "fc73c97a0659d7e5c2d2690adfb7ae8e4af2c836a32882793ceba666b91addca"
---

Warning:

The NetSuite integration with the Worldpay Payment Gateway (Worldpay UK) does not support EMV 3DS. Relying on the older 3DS 1.x for your SiteBuilder or SuiteCommerce web store is expected to result in more failed or declined payment card transactions. For more information, refer to the e-mail message sent on May 3, 2022, with the following subject: Required Transition to Updated Customer Authentication for Online Payments.

If you use custom transaction forms for either cash sales or sales orders, don't hide the Credit Card Approved field on the forms. Hiding this field also hides other Address Verification System (AVS) related fields. For more information, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

#### To add a new WorldPay (UK) Limited credit card processing profile: {#procedure_N1576736}

1.  Go to _Setup > Accounting > Payment Processing Profiles > New_ and next to **WorldPay (UK) Limited**, click **Add Profile**.
    
    The WorldPay (UK) Limited integration must be installed in your account. Otherwise, Install shows instead of Add Profile.
    
2.  In the Primary section, enter the profile primary information. See [Entering WorldPay (UK) Limited Profile Primary Information](#bridgehead_4595104784).
    
3.  In the Authentication Credentials section, enter the installation ID provided by WorldPay (UK) Limited.
    
    Enter and confirm your XML Password.
    
    A merchant code supports e-commerce or MOTO (WorldAccess) transactions. If you plan to process both e-commerce and MOTO transactions, then you need two merchant codes from WorldPay (UK) Limited and must set up two profiles in NetSuite.
    
4.  Under Payment Information, select the credit cards you accept with WorldPay (UK) Limited. For a list of accepted credit cards, see _WorldPay Credit Card Processing Gateway FAQ_.
    
5.  Under Gateway Request Types, select requests you want this profile to support.
    
    Warning:
    
    When you use a payment processing profile that doesn't support authorization to process credit card payments on sales orders, make sure you follow the card acceptance guidelines of the credit card issuer. For information about the Visa card acceptance guidelines, see [Card Acceptance Guideline for Visa Merchants](https://usa.visa.com/content/dam/VCOM/global/support-legal/documents/card-acceptance-guidelines-visa-merchants.pdf).
    
    If your business involves shipping goods to your customers, you must process the sales order with a payment processing profile that supports authorization. Funds must be deposited only when goods have been fulfilled.
    
    Use a payment processing profile that doesn't support the authorization request on a sales order only when you provide an immediate delivery of goods or services.
    
6.  Click **Save**.
    

## Entering WorldPay (UK) Limited Profile Primary Information {#bridgehead_4595104784}

On the WorldPay (UK) Limited Credit Card Processing Profile page at _Setup > Accounting > Payment Processing Profiles > New_, you can enter the profile's primary information

#### To enter WorldPay (UK) Limited profile primary information:

1.  If you use the Multiple Web Sites feature, select the site on which this credit card processing profile is used.
    
2.  Enter a name for the credit card gateway, for example, WorldPay (UK) Limited e-Commerce or WorldPay (UK) Limited MOTO.
    
3.  If you use NetSuite OneWorld, select the subsidiary for this account.
    
4.  Select the settlement currency for this processor.
    
5.  In the **Charge Currencies** field, select the currencies you receive payment in with this processor.
    
6.  Select the bank account to use when receiving settlement for transactions processed with this credit card gateway.
    
7.  Check the **Payer Authentication** box to offer payer authentication for credit card payments on your Web site.
    
    For more information, see [Payer Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_4595030256).
    
8.  Check the **Test Mode** box to enter test transactions to test this processing profile.
    
    Test transactions don't affect your merchant account.
    
9.  Check the **Allow Request ID to Meet Payment Card Field Requirements** box to permit orders authorized through a third party order entry system to be created and processed in NetSuite.
    
    For more information, see [Allow Request ID to Meet Payment Card Field Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_4595031963).
    
10.  Select the **Inactive** box to make the account inactive, without deleting it.
     

### Related Topics

-   _Credit Card Processing Gateway FAQ_
    
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html)
-   [Payment Gateways](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

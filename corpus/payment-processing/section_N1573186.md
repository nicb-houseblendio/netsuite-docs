---
id: "section_N1573186"
type: "section"
title: "AsiaPay"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Regional Payment Gateways > AsiaPay"
parent: "section_N1577002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573186.html"
anchors: ["bridgehead_4651990084", "subsect_43090718521", "procedure_0715085555"]
sha256: "74c78b2dedbe86c627db971394a4cddc8500c20b9f25c86c95764f81700824d4"
---

Integration with the AsiaPay gateway is available in the Payment Gateway SuiteApp. For more information about the SuiteApp, see [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html).

| **Country of operation** | Australia, China, Hong Kong, India, Indonesia, Macao, Malaysia, New Zealand, Philippines, Singapore, Taiwan (Province of China), Thailand, Viet Nam |
| --- | --- |
| **Supported NetSuite processing methods** | Authorization, capture, sale, and refund Note: For AsiaPay Direct integrations, your merchant or acquiring bank require payer authentication, which currently isn't supported. |
| **Other supported features** | AsiaPay External Checkout Note: The AsiaPay External Checkout integration includes support for payer authentication. For more information, see [AsiaPay External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609621020.html). |

## Setup Requirements for AsiaPay Integration {#bridgehead_4651990084}

You need the following requirements for installation and setup:

-   Prerequisites for AsiaPay Direct:
    
    -   Enable the Multiple Currencies feature in your account. For information about using multiple currencies, see [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html).
        
    -   Enable Secure Hash Encryption (SHA256) feature for AsiaPay Direct. Contact AsiaPay's service team for assistance in enabling this feature in your merchant account.
        
    -   Get the merchant account credentials from AsiaPay: Merchant ID, merchant API login, password, and Secure Hash Secret key.
        
        Important:
        
        NetSuite ended the support for SHA1 algorithm. To enable the SHA256 feature in your merchant account and NetSuite account you must contact the AsiaPay's service team. See [Upgrading the Secure Hash Algorithm from SHA1 to SHA256](#subsect_43090718521).
        
        These API credentials are different from your AsiaPay user login credentials. Use the credentials to set up as many credit card processing profiles for AsiaPay as needed.
        
-   Prerequisites for AsiaPay External Checkout, see [Enabling prerequisites for AsiaPay External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609624270.html#bridgehead_4609625069).
    

After enabling the prerequisites and obtaining your requirements, see the procedures in the following topics:

-   To set up AsiaPay Direct integration, see [AsiaPay Direct](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1557795720.html).
    
-   To set up AsiaPay External Checkout, see [Setting Up AsiaPay External Checkout Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609624270.html).
    

## Upgrading the Secure Hash Algorithm from SHA1 to SHA256 {#subsect_43090718521}

After enabling SHA256 in your merchant account, manually upgrade the secure hash algorithm in NetSuite.

Note:

You must log in to NetSuite as an administrator to perform the upgrade from SHA1 to SHA256.

#### To manually upgrade the secure hash algorithm from SHA1 to SHA256: {#procedure_0715085555}

1.  Go to Setup > Accounting > Payment Processing Profiles.
    
2.  Click **Edit** next to the payment processing profile you want to update.
    
3.  From the **Secure Hash Algorithm** list, select **SHA256**.
    
4.  Update the SHA256 secret key in the **Secure Hash Secret** field.
    
5.  Click **Save**.
    

### Related Topics:

-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
-   [eWAY Rapid](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471740031.html)
-   [PayU Latin America External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4536913874.html)
-   [SecurePay and SecurePay FraudGuard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573049.html)
-   [VeriTrans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3843570937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

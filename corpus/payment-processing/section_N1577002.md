---
id: "section_N1577002"
type: "section"
title: "Setting Up Regional Payment Gateways"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Regional Payment Gateways"
parent: "section_N1572221"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1577002.html"
anchors: ["bridgehead_4537022247", "bridgehead_4537023531", "subsect_160692452231", "procedure_N1577132", "subsect_160692394906", "procedure_N1577167"]
sha256: "47a9590a5353ad061e3b77f77ff81438f083592f6fa54dbc087ba5641bc88178"
---

Warning:

If you use custom transaction forms for either cash sales or sales orders, don't hide the Credit Card Approved field on the forms. Hiding this field also hides other Address Verification System (AVS) related fields. For more information, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

Using the Payment Gateway SuiteApp, you can integrate your NetSuite account with the regional payment gateways. For more information about the SuiteApp, see [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html).

## Prerequisites for Payment Gateway Integration {#bridgehead_4537022247}

Before installing the Payment Gateway SuiteApp, be sure to enable the required features. You can review specific gateway features and requirements in the following topics:

-   [Setup Requirements for AsiaPay Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573186.html#bridgehead_4651990084)
    
-   [Setting Up AsiaPay External Checkout Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609624270.html)
    
-   [Setup Requirements for eWay Rapid Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4651858847.html)
    
    Important:
    
    As of Version 2017 Release 1, retirement of eWAY (XML) integration support will be completed and you will no longer be able to process credit card payments using eWAY (XML) payment processing profiles. To help you in your transition to eWAY Rapid, see [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424).
    
-   [Setting Up PayU Latam External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4536934906.html)
    
    Note:
    
    Due to an ongoing PayU security upgrade, all sales orders using the PayU profile will be placed on hold and reviewed for approval. For more information, see [Change in Sales Order Processing using PayU Latam External Checkout Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4536966934.html#bridgehead_155978832368).
    
-   [Setup Requirements for SecurePay and SecurePay FraudGuard Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573049.html#bridgehead_4651973159)
    
-   [Setup Requirements for VeriTrans Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3843570937.html#bridgehead_4651962972)
    
    Important:
    
    VeriTrans gateway integration is temporarily unavailable in NetSuite 2019.1 due to an ongoing VeriTrans security upgrade.
    
    To continue processing credit card payments, use other payment processing profiles. For more information, see [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424).
    

After enabling the required features, you can install the SuiteApp and set up the integration. Follow the procedures in these topics:

-   [Installing the Payment Gateway SuiteApp](#bridgehead_4537023531)
    
-   [To activate the payment processing plug-in:](#procedure_N1577132)
    
-   [To add a new credit card processing profile:](#procedure_N1577167)
    

## Installing the Payment Gateway SuiteApp {#bridgehead_4537023531}

To install the Payment Gateway SuiteApp, go to _Customization > SuiteBundler > Search & Install Bundles_. On the Search & Install Bundles page, search for the SuiteApp with the following details:

-   Bundle name: **Payment Gateway**
    
-   Bundle ID: **47196**
    

To verify that the SuiteApp is installed in your account, go to _Customization > SuiteBundler > Search & Install Bundles > List_. For more information about SuiteApp installation, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).

Payment Gateway is a managed SuiteApp and is automatically updated whenever there are updates. Issue fixes and enhancements are available after the bundle has been updated in your account.

## Activating the Payment Processing Plug-in {#subsect_160692452231}

After you have installed the Payment Gateway SuiteApp, you must activate the payment processing plug-in specific to the regional payment gateway.

#### To activate the payment processing plug-in: {#procedure_N1577132}

1.  Go to _Customization > Plug-ins > Manage Plug-ins_.
    
2.  On the Manage Plug-In Implementations page, check the box next to the payment gateway to be activated.
    
3.  Click **Save**.
    

## Adding a New Credit Card Processing Profile {#subsect_160692394906}

Create credit card processing profiles for the regional payment gateways and associate them with payment methods that you have set up for each credit card or payment solution. For information about setting up payment methods, see [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html).

#### To add a new credit card processing profile: {#procedure_N1577167}

1.  Go to _Setup > Accounting > Payment Processing Profiles > New_.
    
2.  Click **Add Profile** next to the integration that you want to add.
    
    If the gateway integration isn't installed in your account, you must click Install before you can add a new profile.
    
3.  On the Payment Processing Profile page, do the following in the specific sections:
    
    1.  In the Primary section, enter or select the details in the fields based on the regional payment gateway you want to set up.
        
        | Field | Description |
        | --- | --- |
        | Web Site | Select the websites this processor is used to capture payment for. |
        | Name | Enter a name for the payment gateway profile. |
        | Subsidiary | If you use NetSuite OneWorld, select the subsidiary for profile. |
        | Settlement Currency | If you use Multiple Currencies, select the settlement currency for this processor. |
        | Charge Currencies | Select the currencies you receive payment in with this processor. |
        | Settlement Bank Account | Select the bank account to use when receiving settlement for transactions processed by the payment gateway. |
        
        You can select the following options or features based on your requirements:
        
        Note:
        
        The **Allow Request ID to Meet Payment Card Field Requirements** option isn't available for regional credit card gateways.
        
        -   **Payer Authentication** - Don't check this box to enable payer authentication for regional payment gateways. Payer authentication is currently available through the eWay Rapid and AsiaPay External Checkout integrations. For more information, see the following topics:
            
            -   [Payer Authentication for eWay Rapid](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4651871224.html)
                
            -   [AsiaPay External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609621020.html)
                
            
            Note:
            
            For other payment gateway integrations, if payer authentication is required in your country, please work with your merchant bank to implement it.
            
        -   **Test Mode** - Check this box to enter test transactions for a payment processor. Transactions entered in test mode are reflected in a test account and don't affect your merchant account in any way.
            
            Note:
            
            AsiaPay doesn't process refunds in test mode.
            
        -   **Inactive** - Check this box to make the profile inactive, without deleting it.
            
    2.  In the Authentication Credentials section, enter the merchant account credentials from the gateway provider.
        
        Note:
        
        Merchant account credentials used for live transaction processing are different from user login credentials.
        
        -   AsiaPay credentials:
            
            AsiaPay Direct - Enter the login ID, merchant ID, and password.
            
        -   eWay credentials:
            
            eWay Rapid - Enter the API Key and password, which you need to configure in the eWay merchant portal.
            
        -   PayU Latam credentials - Enter the API key, API login, password, and account ID.
            
            Important:
            
            PayU gateway integration is temporarily unavailable in NetSuite 2019.1 due to an ongoing PayU security upgrade.
            
            All sales orders using the PayU profile will be placed on hold and reviewed for approval. To manage PayU payment holds, check the payment status on the PayU gateway portal then manually override the payment hold on NetSuite. For more information, see [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html).
            
        -   SecurePay credentials:
            
            -   SecurePay (Direct) - Enter the merchant ID and password.
                
            -   SecurePay FraudGuard - Enter the merchant ID and password.
                
        -   VeriTrans credentials - Enter the merchant ID and merchant verification key.
            
            Important:
            
            VeriTrans gateway integration is temporarily unavailable in NetSuite 2019.1 due to an ongoing VeriTrans security upgrade.
            
            To continue processing credit card payments, use other payment processing profiles. For more information, see [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424).
            
    3.  In the Payment Information section, choose the credit cards or payment methods you accept with this processor in the **Supported Payment Methods** field.
        
        To create additional payment methods, see [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html).
        
    4.  In the Gateway Request Types section, check the boxes for the request types supported by the regional payment gateway integration: **Authorizations**, **Captures**, **Sales**, and **Credits**.
        
        Note:
        
        Gateway request types that are not supported by the regional payment gateway are disabled. All regional gateways don't support credit requests.
        
        For more information about the gateway request types, see [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html). If you want to use alternate payment methods, see [Alternative Non-Credit Card Payment Methods for Web Store Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4213266422.html).
        
4.  Click **Save**.
    
    When transitioning from one gateway to another, you need to update the payment processing profile to change the gateway request types. For more information, see [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424).
    

### Related Topics:

-   [Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3803057063.html)
-   [AsiaPay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573186.html)
-   [AsiaPay External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609621020.html)
-   [eWAY Rapid](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471740031.html)
-   [PayU Latin America External Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4536913874.html)
-   [SecurePay and SecurePay FraudGuard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573049.html)
-   [VeriTrans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3843570937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

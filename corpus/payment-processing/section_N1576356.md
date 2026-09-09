---
id: "section_N1576356"
type: "section"
title: "MerchantE"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Processing > Setting Up Payment Processing Profiles in NetSuite > MerchantE"
parent: "section_N1572588"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1576356.html"
anchors: ["procedure_N1576380", "procedure_N1576419", "bridgehead_4595115513", "bridgehead_N1576612"]
sha256: "3398f54940bc62b7046af704fe2a508f3e8e7242151dfc9a4449f1409ecb0596"
---

Warning:

If you use custom transaction forms for either cash sales or sales orders, don't hide the Credit Card Approved field on the forms. Hiding this field also hides other Address Verification System (AVS) related fields. For more information, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

#### To add a new MerchantE credit card processing profile: {#procedure_N1576380}

1.  [To enter profile information:](#procedure_N1576419).
    
2.  [Set Up Order Verification](#bridgehead_N1576612).
    

#### To enter profile information: {#procedure_N1576419}

1.  Go to _Setup > Accounting > Payment Processing Profiles > New_ and next to **MerchantE**, click **Add Profile**.
    
2.  In the Primary section, enter the primary information for this profile. See [Entering MerchantE Profile Primary Information](#bridgehead_4595115513).
    
3.  Under Authentication Credentials:
    
    1.  Enter the **Profile ID**. This is a unique 20-digit number provided by MerchantE.
        
    2.  Enter the **Profile Key** provided by MerchantE. This is a unique, 32-character alphanumeric, case-sensitive transaction passkey.
        
4.  Under Payment Information, select the credit cards you accept with this processor.
    
5.  Under Gateway Request Types, select requests you want this profile to support.
    
    Warning:
    
    When you use a payment processing profile that doesn't support authorization to process credit card payments on sales orders, make sure you follow the card acceptance guidelines of the credit card issuer. For information about the Visa card acceptance guidelines, see [Card Acceptance Guideline for Visa Merchants](https://usa.visa.com/content/dam/VCOM/global/support-legal/documents/card-acceptance-guidelines-visa-merchants.pdf).
    
    If your business involves shipping goods to your customers, you must process the sales order with a payment processing profile that supports authorization. Funds must be deposited only when goods have been fulfilled.
    
    Use a payment processing profile that doesn't support the authorization request on a sales order only when you provide an immediate delivery of goods or services.
    
6.  Click **Save**.
    

## Entering MerchantE Profile Primary Information {#bridgehead_4595115513}

On the MerchantE Credit Card Processing Profile page at Setup > Accounting > Payment Processing Profiles, you can enter the profile's primary information.

#### To enter MerchantE profile primary information:

1.  If you use the Multiple Web Sites feature, select the site on which this credit card processing profile is used.
    
2.  Enter a name for the credit card gateway.
    
3.  If you use NetSuite OneWorld, select the subsidiary for this account.
    
4.  Select the settlement currency for this processor.
    
5.  In the **Charge Currencies** field, select the currencies you receive payment in with this processor.
    
6.  Select the bank account to use when receiving settlement for transactions processed with this credit card gateway.
    
7.  Check the **Payer Authentication** box to offer payer authentication for credit card payments on your Web site.
    
    For more information, see [Payer Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_4595030256).
    
8.  Check the **Allow Request ID to Meet Payment Card Field Requirements** box to permit orders authorized through a third-party order entry system to be created and processed in NetSuite.
    
    For more information, see [Allow Request ID to Meet Payment Card Field Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_4595031963).
    
9.  Check the **Process Purchase Card Data** box to enable purchase card processing (also known as level II and level III cards).
    
    This box is available only when your account is provisioned for the Purchase Card Data module. See [Accepting Purchase Cards (Level II and Level III Credit Cards)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html#bridgehead_N1569481).
    
10.  Select the **Inactive** box to make the account inactive, without deleting it.
     

## Set Up Order Verification {#bridgehead_N1576612}

For instructions on how to set up order verification rules for this gateway, see [Setting Up Order Verification Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567770.html#bridgehead_N1567973).

### Related Topics

-   [Payment Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1569446.html)
-   [Setting Up a Merchant Account with a Payment Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572566.html)
-   [Establishing a Merchant Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572500.html)
-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)
-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Voiding Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1570067.html)
-   [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html)
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

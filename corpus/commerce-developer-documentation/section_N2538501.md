---
id: "section_N2538501"
type: "section"
title: "SSP Application Governance"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > SSP Application Governance"
parent: "section_N2496227"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538501.html"
anchors: []
sha256: "b05d312c4ec642a668510f18f1ae8a6ca8759d3ee48c735b6d08bbd746b69336"
---

SSP applications have a governance model in accordance with SuiteScript governance model, with the same goal of optimizing performance. SSP application governance is based on usage units. Each shopping method consumes a system-defined number of processing units, and each SSP application script can execute a system-defined number of units. If the number of allowable units is exceeded by an SSP application script, the script is terminated.

The limit for SSP applications is 1000 units per script.

The units consumed per method are as follows:

-   Shopping Session Methods
    
    -   nlobjShoppingSessionImpl.logIn(20)
        
    -   nlobjShoppingSessionImpl.registerCustomer(20)
        
    -   nlobjShoppingSessionImpl.registerGuest(20)
        
    -   nlobjShoppingSessionImpl.setShopperCurrency(10)
        
    -   nlobjShoppingSessionImpl.setShopperLanguageLocale(10)
        
    -   nlobjShoppingSessionImpl.setShopperSubsidiary(10)
        
    -   nlobjShoppingSessionImpl.getPaymentMethods(10)
        
    -   nlobjShoppingSessionImpl.getCountries(10)
        
    -   nlobjShoppingSessionImpl.getShipToCountries(10)
        
    -   nlobjShoppingSessionImpl.getStates(10)
        
    -   nlobjShoppingSessionImpl.getItemFieldValues(10)
        
    -   nlobjShoppingSessionImpl.getSiteCategoryFieldValues(10)
        
    -   nlobjShoppingSessionImpl.getInformationItemFieldValues(10)
        
    -   nlobjShoppingSessionImpl.getMediaItemFieldValues(10)
        
-   Customer Methods
    
    -   nlobjWebStoreCustomerImpl.addAddress(10)
        
    -   nlobjWebStoreCustomerImpl.updateAddress(10)
        
    -   nlobjWebStoreCustomerImpl.removeAddress(10)
        
    -   nlobjWebStoreCustomerImpl.addCreditCard(10)
        
    -   nlobjWebStoreCustomerImpl.updateCreditCard(10)
        
    -   nlobjWebStoreCustomerImpl.removeCreditCard(10)
        
    -   nlobjWebStoreCustomerImpl.getAddressBook(10)
        
    -   nlobjWebStoreCustomerImpl.getAddress(10)
        
    -   nlobjWebStoreCustomerImpl.getCreditCards(10)
        
    -   nlobjWebStoreCustomerImpl.getCreditCard(10)
        
-   Order Methods
    
    -   nlobjWebStoreOrderImpl.addItems(20)
        
    -   nlobjWebStoreOrderImpl.addItem(10)
        
    -   nlobjWebStoreOrderImpl.removeItem(10)
        
    -   nlobjWebStoreOrderImpl.updateItemQuantity(10)
        
    -   nlobjWebStoreOrderImpl.updateItemQuantities(20)
        
    -   nlobjWebStoreOrderImpl.removeAllItems(10)
        
    -   nlobjWebStoreOrderImpl.estimateShippingCost(20)
        
    -   nlobjWebStoreOrderImpl.applyPromotionCode(5)
        
    -   nlobjWebStoreOrderImpl.removePromotionCode(5)
        
    -   nlobjWebStoreOrderImpl.applyGiftCertificate(5)
        
    -   nlobjWebStoreOrderImpl.removeAllGiftCertificates(5)
        
    -   nlobjWebStoreOrderImpl.setShippingAddress(10)
        
    -   nlobjWebStoreOrderImpl.setShippingMethod(5)
        
    -   nlobjWebStoreOrderImpl.getAvailableShippingMethods(20)
        
    -   nlobjWebStoreOrderImpl.getAvailableShippingMethod(10)
        
    -   nlobjWebStoreOrderImpl.submit(20)
        

Note:

There is no concurrency limit for SSP applications but you should not use them for high volume catalog pages or to deliver content that should be delivered from a cache.

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

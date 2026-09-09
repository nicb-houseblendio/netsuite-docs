---
id: "section_N2503226"
type: "section"
title: "Customer Methods"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > Shopping Objects > Customer Methods"
parent: "section_N2496577"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html"
anchors: ["bridgehead_4482704717", "bridgehead_3995006665", "bridgehead_444990780", "bridgehead_444990781", "bridgehead_444990782", "bridgehead_4482704999", "bridgehead_3995009656", "bridgehead_444990783", "bridgehead_444990784", "bridgehead_444990785", "bridgehead_4482705235", "bridgehead_3995013225", "bridgehead_3995013226", "bridgehead_444990786", "bridgehead_4479555835", "bridgehead_3995014099", "bridgehead_3995014098", "bridgehead_4479555967", "bridgehead_3995014109", "bridgehead_4479556076", "bridgehead_4482705456", "bridgehead_3995015558", "bridgehead_4479556176", "bridgehead_4479556290", "bridgehead_4479556410", "bridgehead_3995016234", "bridgehead_3995016233", "bridgehead_4479556520", "bridgehead_4479556655", "bridgehead_4479556762", "bridgehead_3995016850", "bridgehead_3995016859", "bridgehead_4479556870", "bridgehead_4479556981", "bridgehead_4479557124", "bridgehead_4482705660", "bridgehead_3995017872", "bridgehead_4479557247", "bridgehead_4479557344", "bridgehead_4479557489", "bridgehead_4482705957", "bridgehead_3995020810", "bridgehead_4479557592", "bridgehead_4479557703", "bridgehead_4479557813", "bridgehead_160831867508", "bridgehead_160831867505", "bridgehead_160831867506", "bridgehead_161860662624", "bridgehead_160831867507", "bridgehead_4479557923", "bridgehead_3995022756", "bridgehead_4479558041", "bridgehead_4479558163", "bridgehead_4479558284", "bridgehead_4479558415", "bridgehead_3995023385", "bridgehead_4479558523", "bridgehead_4479558637", "bridgehead_4479558745", "bridgehead_4479558894", "bridgehead_3995024400", "bridgehead_4479559014", "bridgehead_4479559134", "bridgehead_4479559252", "bridgehead_3995025095", "bridgehead_3995025094", "bridgehead_4479559396", "bridgehead_4479559501", "bridgehead_4479559635", "bridgehead_4482706357", "bridgehead_3995025514", "bridgehead_4479559776", "bridgehead_4479559887", "bridgehead_4479559998", "bridgehead_4482706566", "bridgehead_3995026141", "bridgehead_4479560103", "bridgehead_4479560239", "bridgehead_4479560351", "bridgehead_4482706776", "bridgehead_3995026799", "bridgehead_3995026800", "bridgehead_4479560464", "bridgehead_4479560613", "bridgehead_4482706982", "bridgehead_3995028144", "bridgehead_4479560758", "bridgehead_4479560865", "bridgehead_4479561033", "bridgehead_4482707195", "bridgehead_3995030007", "bridgehead_4479561151", "bridgehead_4479561263", "bridgehead_4479561407", "bridgehead_4482707447", "bridgehead_3995031397", "bridgehead_3995031398", "bridgehead_4479561536", "bridgehead_4479561641", "bridgehead_3995034825", "bridgehead_3995034824", "bridgehead_4479561773", "bridgehead_4479561880", "bridgehead_4479561999"]
sha256: "9ccfbf8a428c33d61d203ca7ea6d014464005e8b817e02b1d256f94d26e20a3f"
---

A customer object holds data for the logged in customer. This object is different from a NetSuite customer record, because it holds information for the given shopping session only.

The following Customer methods are available:

-   [addAddress(address)](#bridgehead_4482704717)
    
-   [addCreditCard(creditcard)](#bridgehead_4482704999)
    
-   [emailCustomer(subject, body)](#bridgehead_4482705235)
    
-   [getAddress(addressid, fields)](#bridgehead_3995014099)
    
-   [getAddressBook(fields)](#bridgehead_4482705456)
    
-   [getCampaignSubscriptions(fields)](#bridgehead_3995016234)
    
-   [getCampaignSubscriptions(subscriptionId,fields)](#bridgehead_3995016850)
    
-   [getCreditCard(creditcardid, fields)](#bridgehead_4482705660)
    
-   [getCreditCards(fields)](#bridgehead_4482705957)
    
-   [getCustomerSegments()](#bridgehead_160831867508)
    
-   [getCustomFields()](#bridgehead_4479557923)
    
-   [getCustomFieldValues()](#bridgehead_4479558415)
    
-   [getFieldValues(fields)](#bridgehead_4479558894)
    
-   [isGuest()](#bridgehead_3995025095)
    
-   [removeAddress(addressid)](#bridgehead_4482706357)
    
-   [removeCreditCard(creditcardid)](#bridgehead_4482706566)
    
-   [setLoginCredentials(customer)](#bridgehead_4482706776)
    
-   [updateAddress(address)](#bridgehead_4482706982)
    
-   [updateCampaignSubscriptions(subscriptions)](#bridgehead_4482707195)
    
-   [updateCreditCard(creditcard)](#bridgehead_4482707447)
    
-   [updateProfile(customer)](#bridgehead_3995034825)
    

## addAddress(address) {#bridgehead_4482704717}

Adds an address for current customer.

## Parameters {#bridgehead_3995006665}

-   `address` \[required\] {Object with values for fields}
    
    -   `addressee` \[required\]
        
    -   `addr1` \[required\]
        
    -   `addr2` \[optional\]
        
    -   `addr3` \[optional\]
        
    -   `city` \[required\]
        
    -   `state` \[required\]
        
    -   `country` \[required\]
        
    -   `zip` \[required\]
        
    -   `phone` \[optional\]
        
    -   `isresidential` \[optional\]
        
    -   `defaultshipping` \[optional\]
        
    -   `defaultbilling` \[optional\]
        

## Returns {#bridgehead_444990780}

String - key of added address.

## Supported Domains {#bridgehead_444990781}

Checkout

## Login Required? {#bridgehead_444990782}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## addCreditCard(creditcard) {#bridgehead_4482704999}

Adds a credit card for current customer.

Note:

This method is not compatible with SuiteCommerce 2019.1 if the Payments Instruments feature is enabled. SuiteScript methods should be used instead.

## Parameters {#bridgehead_3995009656}

-   `creditcard` \[required\] {Object with values for fields}
    
    -   `ccnumber` \[required\]
        
    -   `ccname` \[required\]
        
    -   `authcode` \[optional\]
        
    -   `customercode` \[optional\]
        
    -   `paymentmethod` \[required\] (numerical ID for credit card type in NetSuite)
        
    -   `expmonth` \[required\]
        
    -   `expyear` \[required\]
        
    -   `validfrommon` \[required for UK\]
        
    -   `validfromyear` \[required for UK\]
        
    -   `debtcardissueno` \[required for UK\]
        
    -   `ccdefault` \[optional\]
        

## Returns {#bridgehead_444990783}

String - key of added credit card.

## Supported Domains {#bridgehead_444990784}

Checkout

## Login Required? {#bridgehead_444990785}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## emailCustomer(subject, body) {#bridgehead_4482705235}

Sends email to current customer with given subject and body.

## Parameters {#bridgehead_3995013225}

-   `subject` \[required\] {String}
    
-   `body` \[required\] {String}
    

## Returns {#bridgehead_3995013226}

No value returned.

## Supported Domains {#bridgehead_444990786}

Checkout

## Login Required? {#bridgehead_4479555835}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getAddress(addressid, fields) {#bridgehead_3995014099}

Gets address with given ID for current customer.

## Parameters {#bridgehead_3995014098}

-   `addressid` \[required\] {string}
    
-   `fields` \[optional\] Array of field names to be included in returned JSON object; if omitted, all supported fields are returned}
    

## Returns {#bridgehead_4479555967}

Object of type [address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html).

## Supported Domains {#bridgehead_3995014109}

Checkout

## Login Required? {#bridgehead_4479556076}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getAddressBook(fields) {#bridgehead_4482705456}

Gets all addresses for current customer

## Parameters {#bridgehead_3995015558}

-   `fields` \[optional\] Array of field names to be included in returned JSON object; if omitted, all supported fields are returned}
    

## Returns {#bridgehead_4479556176}

Array of objects of type [address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html).

## Supported Domains {#bridgehead_4479556290}

Checkout

## Login Required? {#bridgehead_4479556410}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCampaignSubscriptions(fields) {#bridgehead_3995016234}

Gets subscription information for the current customer

## Parameters {#bridgehead_3995016233}

-   `fields` \[optional\] Array of field names to be included in returned JSON object; if omitted, all supported fields are returned}
    

## Returns {#bridgehead_4479556520}

Array of objects of type [subscriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2535600.html).

## Supported Domains {#bridgehead_4479556655}

Checkout, Shopping

## Login Required? {#bridgehead_4479556762}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCampaignSubscriptions(subscriptionId,fields) {#bridgehead_3995016850}

Gets data for a single campaign subscription with passed id.

## Parameters {#bridgehead_3995016859}

-   `subscriptionId` \[required\] {String}
    
-   `fields` \[optional\] Array of field names to be included in returned JSON object; if omitted, all supported fields are returned
    

## Returns {#bridgehead_4479556870}

Array of objects of type [subscriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2535600.html)

## Supported Domains {#bridgehead_4479556981}

Checkout, Shopping

## Login Required? {#bridgehead_4479557124}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCreditCard(creditcardid, fields) {#bridgehead_4482705660}

Gets credit card with given ID for current customer.

Note:

This method is not compatible with SuiteCommerce 2019.1 if the Payments Instruments feature is enabled. SuiteScript methods should be used instead.

## Parameters {#bridgehead_3995017872}

-   `creditcard` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `ccnumber` \[required\]
        
    -   `ccname` \[required\]
        
    -   `authcode` \[optional\]
        
    -   `customercode` \[optional\]
        
    -   `paymentmethod` \[required\]
        
    -   `expmonth` \[required\]
        
    -   `expyear` \[required\]
        
    -   `validfrommon` \[required for UK\]
        
    -   `validfromyear` \[required for UK\]
        
    -   `debtcardissueno` \[required for UK\]
        
    -   `ccdefault` \[optional\]
        

## Returns {#bridgehead_4479557247}

Object of type [creditcard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2518010.html).

## Supported Domains {#bridgehead_4479557344}

Checkout

## Login Required? {#bridgehead_4479557489}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCreditCards(fields) {#bridgehead_4482705957}

Gets all credit cards for current customer.

Note:

This method is not compatible with SuiteCommerce 2019.1 if the Payments Instruments feature is enabled. SuiteScript methods should be used instead.

## Parameters {#bridgehead_3995020810}

-   `customer` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `email` \[optional\]
        
    -   `emailsubscribe` \[optional\]
        
    -   `firstname` \[optional\]
        
    -   `lastname` \[optional\]
        
    -   `middlename` \[optional\]
        
    -   `phoneinfo` \[optional\]
        
    -   `customfields` \[optional\] {Object with {customfield id : customfield value} }
        

## Returns {#bridgehead_4479557592}

Array of objects of type [creditcard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2518010.html).

## Supported Domains {#bridgehead_4479557703}

Checkout

## Login Required? {#bridgehead_4479557813}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCustomerSegments() {#bridgehead_160831867508}

Gets all customer segments to which the current customer belongs.

## Parameters {#bridgehead_160831867505}

No parameters to set.

## Returns {#bridgehead_160831867506}

Array of objects with the field:

-   `id` {number}
    

## Supported Domains {#bridgehead_161860662624}

Shopping, Checkout

## Login Required? {#bridgehead_160831867507}

No

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCustomFields() {#bridgehead_4479557923}

Gets custom fields on customer record for current customer.

## Parameters {#bridgehead_3995022756}

No parameters to set.

## Returns {#bridgehead_4479558041}

Object with custom field names.

## Supported Domains {#bridgehead_4479558163}

Checkout, Shopping

## Login Required? {#bridgehead_4479558284}

No

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getCustomFieldValues() {#bridgehead_4479558415}

Gets custom field values on customer record for current customer.

## Parameters {#bridgehead_3995023385}

No parameters to set.

## Returns {#bridgehead_4479558523}

Object with custom field values. Multiple field values are separated by the Unicode character 'ENQUIRY' ("\\u0005").

## Supported Domains {#bridgehead_4479558637}

Checkout, Shopping

## Login Required? {#bridgehead_4479558745}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## getFieldValues(fields) {#bridgehead_4479558894}

Gets standard field values on customer record for current customer.

## Parameters {#bridgehead_3995024400}

-   `fields` \[optional\] Array of field names to be included in returned JSON object; if omitted, all supported fields are returned}
    

## Returns {#bridgehead_4479559014}

Object of type [customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2519129.html).

## Supported Domains {#bridgehead_4479559134}

Checkout

## Login Required? {#bridgehead_4479559252}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## isGuest() {#bridgehead_3995025095}

Checks whether the shopper is logged in as a guest. Returns False when the shopper is not logged in or is logged in as a customer.

## Parameters {#bridgehead_3995025094}

No parameters to set.

## Returns {#bridgehead_4479559396}

Boolean

## Supported Domains {#bridgehead_4479559501}

Checkout, Shopping

## Login Required? {#bridgehead_4479559635}

No

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## removeAddress(addressid) {#bridgehead_4482706357}

Removes address with given ID from current customer's list of addresses.

## Parameters {#bridgehead_3995025514}

-   `addressid` \[required\] {string}
    

## Returns {#bridgehead_4479559776}

No value returned.

## Supported Domains {#bridgehead_4479559887}

Checkout

## Login Required? {#bridgehead_4479559998}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## removeCreditCard(creditcardid) {#bridgehead_4482706566}

Removes given credit card from current customer.

Note:

This method is not compatible with SuiteCommerce 2019.1 if the Payments Instruments feature is enabled. SuiteScript methods should be used instead.

## Parameters {#bridgehead_3995026141}

-   `creditcardid` \[required\] {string}
    

Note:

Websites on SuiteCommerce versions earlier than 2019.1 must have a patch applied to be compatible with the Payments Instruments feature. See <link to patch documentation>. If the correct patch has been applied, the Payment Instruments feature is enabled, and the credit card has been tokenized, the `creditcardid` parameter should contain the numerical ID of the payment token.

## Returns {#bridgehead_4479560103}

No value returned.

## Supported Domains {#bridgehead_4479560239}

Checkout

## Login Required? {#bridgehead_4479560351}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## setLoginCredentials(customer) {#bridgehead_4482706776}

Sets login credentials for current guest customer.

## Parameters {#bridgehead_3995026799}

-   `customer` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `email` \[required\]
        
    -   `password` \[required\]
        
    -   `customfields` \[Optional\] {Object with {customfield id : customfield value} }
        

## Returns {#bridgehead_3995026800}

No value returned.

## Supported Domains {#bridgehead_4479560464}

Checkout

## Login Required? {#bridgehead_4479560613}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## updateAddress(address) {#bridgehead_4482706982}

Updates a specified address.

## Parameters {#bridgehead_3995028144}

-   `address` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `addressee` \[required\]
        
    -   `addr1` \[required\]
        
    -   `addr2` \[optional\]
        
    -   `addr3` \[optional\]
        
    -   `city` \[required\]
        
    -   `state` \[required\]
        
    -   `country` \[required\]
        
    -   `zip` \[required\]
        
    -   `phone` \[optional\]
        
    -   `isresidential` \[optional\]
        
    -   `defaultshipping` \[optional\]
        
    -   `defaultbilling` \[optional\]
        

## Returns {#bridgehead_4479560758}

No value returned.

## Supported Domains {#bridgehead_4479560865}

Checkout

## Login Required? {#bridgehead_4479561033}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## updateCampaignSubscriptions(subscriptions) {#bridgehead_4482707195}

Updates a specified campaign subscription.

## Parameters {#bridgehead_3995030007}

-   `subscriptions` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `subscribed` \[required\]
        
        Customer can only opt-in or opt-out of an email campaign category by setting subscribed to 'T' or 'F'.
        

## Returns {#bridgehead_4479561151}

No value returned.

## Supported Domains {#bridgehead_4479561263}

Checkout, Shopping

## Login Required? {#bridgehead_4479561407}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## updateCreditCard(creditcard) {#bridgehead_4482707447}

Updates given credit card for current customer.

Note:

This method is not compatible with SuiteCommerce 2019.1 if the Payments Instruments feature is enabled.

## Parameters {#bridgehead_3995031397}

-   `creditcard` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `ccnumber` \[required\]
        
    -   `ccname` \[required\]
        
    -   `authcode` \[optional\]
        
    -   `customercode` \[optional\]
        
    -   `paymentmethod` \[required\]
        
    -   `expmonth` \[required\]
        
    -   `expyear` \[required\]
        
    -   `validfrommon` \[required for UK\]
        
    -   `validfromyear` \[required for UK\]
        
    -   `debtcardissueno` \[required for UK\]
        
    -   `ccdefault` \[optional\]
        

Note:

If given `ccnumber` does not match an existing record, `internalid` is ignored and a new credit card record is added for customer.

## Returns {#bridgehead_3995031398}

String - key of added or updated credit card.

## Supported Domains {#bridgehead_4479561536}

Checkout

## Login Required? {#bridgehead_4479561641}

Yes

**Back to** [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## updateProfile(customer) {#bridgehead_3995034825}

Updates profile of current customer.

## Parameters {#bridgehead_3995034824}

-   `customer` \[required\] {Object with values for fields}
    
    -   `internalid` \[required\]
        
    -   `email` \[optional\]
        
    -   `emailsubscribe` \[optional\]
        
    -   `firstname` \[optional\]
        
    -   `lastname` \[optional\]
        
    -   `middlename` \[optional\]
        
    -   `phoneinfo` \[optional\]
        
    -   `customfields` \[optional\]{Object with {customfield id : customfield value} }
        
    -   `cookieoptions` \[optional\]{Object with {cookie approval type : boolean value} }
        

## Returns {#bridgehead_4479561773}

No value returned.

## Supported Domains {#bridgehead_4479561880}

Checkout

## Login Required? {#bridgehead_4479561999}

Yes

### Related Topics:

-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Input Parameters/Return Values for Shopping Object Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497278.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

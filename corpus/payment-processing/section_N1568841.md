---
id: "section_N1568841"
type: "section"
title: "Setting Up Customer Credit Card Soft Descriptors"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Setting Up Customer Credit Card Soft Descriptors"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html"
anchors: ["bridgehead_N1568877", "procedure_N1568990", "procedure_N1569021", "procedure_N1569099", "bridgehead_N1569138", "procedure_N1569150", "bridgehead_N1569213"]
sha256: "f7656775205804b38a90e978a3085591a1d15bd628b1b02ca1d0e5c737070f05"
---

With the Credit Card Soft Descriptors feature, you can dynamically specify the company name and phone number that appear on the cardholder's credit card statement for purchases from your business. You assign the descriptors to the items you sell. Then that information is provided to the card issuing bank with the transaction to help customers recognize their purchases. The descriptors appear only on cardholder statements. To help customers track their purchases, create descriptors that include a business or product name the customer recognizes, and a phone number. You can create as many soft descriptors as you need.

For example, your company, Hampton, Inc., operates several clothing stores: Fog Outfitters, Southern Nature, and Snow Cap. If a customer purchases an item from Snow Cap, but sees a charge from Hampton, Inc. on his credit card statement, he not recognize the charge. You can set 'Snow Cap' as a soft descriptor and associate it with each item you sell at Snow Cap stores. Customers will then see 'Snow Cap' with charges on their credit card statements instead of your company name.

## Setting Up Soft Descriptors {#bridgehead_N1568877}

To use soft descriptors, you must have an account with one of the following payment gateways:

-   MerchantE
    
-   PayPal Payflow Pro with one of the following processors:
    
    -   Paymentech
        
    -   FDMS North
        
    
    This processor requires an add-on module be enabled in your NetSuite account. For more information, please contact your NetSuite account representative.
    

For more information about setting up customer credit card processing, see [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html).

The process to set up soft descriptors includes:

-   [To enable the credit card soft descriptors feature:](#procedure_N1568990)
    
-   [To create a list of soft descriptors to use:](#procedure_N1569021)
    
-   [Specifying a soft descriptor for each inventory item](#procedure_N1569099)
    

#### To enable the credit card soft descriptors feature: {#procedure_N1568990}

1.  Go to Setup > Company > Setup Tasks > Enable Features.
    
2.  On the **Transactions** subtab, check the **Credit Card Soft Descriptors** box.
    
3.  Click **Save**.
    

#### To create a list of soft descriptors to use: {#procedure_N1569021}

1.  As an Administrator, go to Setup > Accounting > Financial Statements > Credit Card Soft Descriptors.
    
2.  To use a single descriptor that is consistent with most of the items on a charge, check the **Use Plurality Soft Descriptor for Credit Card Transactions** box. This displays the descriptor for the majority of items.
    
3.  In the **Descriptor** column, enter the business or product name as it should appear on a customer's statement.
    
    Important:
    
    Credit card issuers have different limitations on the symbols and the number of characters permitted in a soft descriptor. A descriptor that exceeds the limitations appears truncated on your customers' credit card statements. To ensure a consistent experience for your customers, we recommend creating descriptors of twenty characters or less that contain no special characters.
    
4.  In the **Phone** column, enter the telephone number that should appear after the descriptor text.
    
    For example, if you enter '**APhoneBCXYZ Pumps Service**' as the descriptor text and provide a phone number (**957-987-6543**) for a customer service facility, that descriptor and number combination appear on customer statements as: **ABCXYZPUMPSSERVICE 9579876543**.
    
5.  In the **Default** column, check the box if this descriptor should be selected by default on all new item records.
    
6.  Click **Add**.
    
7.  Repeat steps 3 through 6 for each soft descriptor you want to create.
    
8.  Click **Save**.
    

#### Specifying a soft descriptor for each inventory item {#procedure_N1569099}

1.  Go to _Lists > Accounting > Items > List_.
    
2.  Click **Edit** next to the item's name.
    
3.  On the **Sales/Pricing** subtab, in the **Soft Descriptor** field, select the name of the descriptor to use when this item is purchased by a customer using a credit card.
    
4.  Click **Save**.
    

## Using Default and Plurality Descriptors {#bridgehead_N1569138}

You can designate a default descriptor to be assigned to all new item records you create. The default descriptor also displays in some cases if a customer orders items with different descriptors. When you set a default soft descriptor, the Soft Descriptor field on existing item records remains blank. You can edit the descriptor on the Basic subtab of the item's Inventory Item page. Or you can set soft descriptors on several item records at the same time.

#### To set a soft descriptor for a group of items: {#procedure_N1569150}

1.  Go to Lists > Mass Update > Mass Updates > General Updates > Inventory Item.
    
2.  Define criteria and filters to limit the update to a group of inventory items.
    
3.  Click the **Mass Update Fields** subtab.
    
4.  Check the **Soft Descriptors** box.
    
5.  Select a descriptor from the dropdown list.
    
6.  Click **Save**.
    
    For more information about mass updates, see [Defining a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N667342.html).
    

## Plurality Soft Descriptors {#bridgehead_N1569213}

If you create more than one soft descriptor, enable the Use Plurality Soft Descriptors for Credit Card Transactions option if you want to display the descriptor associated with the majority of items purchased on the credit card statement.

The default and plurality descriptor settings work together to select the descriptor displayed on the cardholder's statement. Review the following to determine the best settings to use for your business.

With Use Plurality Soft Descriptors for Credit Card Transactions enabled:

-   If no descriptor has plurality and a default soft descriptor exists, the default descriptor is used, even if it isn't associated with any items on the invoice.
    
-   If no descriptor has plurality and no default descriptor is designated, the descriptor associated with the first item on the invoice is used.
    
-   If there are descriptors associated with an equal number of items on an invoice, there is a tie for plurality. If one of the tied descriptors is the default descriptor, that descriptor is used. If none of the tied descriptors is the default, the tied descriptor appearing first on the invoice is used.
    

If you don't enable the plurality descriptor option:

-   If a default soft descriptor is designated, the default descriptor is used, even if it isn't associated with any items on the invoice.
    
-   If a default soft descriptor isn't designated, the descriptor associated with the first item on the invoice is used.
    

### Related Topics:

-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424)
-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

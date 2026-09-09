---
id: "section_N1257579"
type: "section"
title: "Setting Up Shipping"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Setting Up Shipping"
parent: "chapter_N1257369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html"
anchors: ["bridgehead_N1257598", "procedure_N1257656", "bridgehead_N1257848", "bridgehead_1545058316", "procedure_N1257985", "procedure_1545060140", "procedure_1545060148", "procedure_1545060154", "procedure_1545060160", "procedure_1545060168", "bridgehead_N1258591", "procedure_N1258634"]
sha256: "f5bd1e0445f9d5454a434b47977384b4b2e6dcf6f1bdc8359862cb250ac9a675"
---

To set up shipping, complete the following tasks:

-   [Setting Shipping Preferences](#bridgehead_N1257598)
    
-   [Carrier Registration Subtab](#bridgehead_N1257848)
    
-   [Preferences Subtab](#bridgehead_1545058316)
    
-   [Packages Subtab](#bridgehead_N1258591)
    

## Setting Shipping Preferences {#bridgehead_N1257598}

After you've set your shipping preferences and registered any integrated UPS, FedEx, or U.S. Postal Service (USPS) accounts, you can create the shipping methods you want to offer. For more information, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).

#### To set up shipping: {#procedure_N1257656}

1.  To define how to charge for shipping, go to _Setup > Accounting > Shipping_.
    
2.  To automatically charge for shipping orders, check the **Charge for Shipping** box.
    
    If you don't check this box, but still want to charge for shipping on sales transactions, create a separate line item on the transaction.
    
    For more information, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
    
3.  To charge handling separately from shipping, check the **Charge Handling Separate from Shipping** and **Charge for Shipping** boxes.
    
    This enables you to assign shipping and handling charges to different accounts.
    
    If you check these boxes when creating a shipping item, you'll see a Handling Rate subtab. Shipping and handling will show up as separate charges in your website's Checkout Summary page.
    
4.  Select the **Default Shipping Carrier** that will appear on sales and website orders.
    
    Note:
    
    Before selecting your default carrier, set up your FedEx, UPS, or USPS accounts on the [Carrier Registration Subtab](#bridgehead_N1257848).
    
    For more information, see [Selecting a Default Shipping Carrier](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html#bridgehead_N1265950).
    
5.  Select the **Default Shipping Method** you want to use for sending sales orders and invoices.
    
6.  If you use Pick, Pack, and Ship, select the default sales order process **Default Item Fulfillment Stage** status.
    
7.  If you use Shipping Label Integration to print labels and track packages, select the earliest Pick, Pack, and Ship **Shipping Label Creation Stage** you can receive tracking numbers and print shipping labels.
    
    This might be different from your Default Item Fulfillment Stage selection.
    
    For example, if you want to mark fulfilled sales orders as Shipped, change part of your inventory fulfillment status to Picked, get tracking numbers, and then print shipping labels. Set the Shipping Label Creation stage to Picked.
    
8.  If you haven't recorded an item's weight, enter a default shipping weight in the **Default Item Weight in Lbs** field.
    
    If you don't enter a weight, NetSuite defaults to 1 lb.
    
    If you charge shipping by weight or use real-time rates, the item's weight helps determine shipping costs.
    
9.  Enter the average **Number of Days to Shipment** between when a sales order is entered and when it's shipped.
    
    This value helps create an estimated ship date on sales orders, and the ship date updates after the order is fulfilled.
    
    By default, the ship date doesn't include weekends or holidays. You can set holiday dates on the **Preferences** subtab.
    
10.  Enter the time of day when you stop shipping orders in the **Cutoff Time for Shipments** field.
     
     Note:
     
     The time format will update based on your current settings. For example, it could be 23:00 or 12-00 PM.
     
     Orders entered after this time count toward the next working day.
     
11.  To include Saturday or Sunday in your days-to-shipment calculation, check the **Ship on Saturday** or the **Ship on Sunday** box.
     
     For example, if you ship on Saturday and have a three-day shipment policy, orders placed before Friday's cutoff will ship on Tuesday.
     

## Carrier Registration Subtab {#bridgehead_N1257848}

To use real-time rates or to use the Shipping Label Integration feature, register a UPS, FedEx, or U.S. Postal Service (USPS) account on the Carrier Registration subtab.

Note:

NetSuite and NetSuite OneWorld support integration with USPS. NetSuite, NetSuite OneWorld, and NetSuite Canada edition support integration with FedEx.

-   To set up UPS accounts, see [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274) or [Registering a UPS Account (UK)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274638.html).
    
-   To set up FedEx accounts, see [Registering a FedEx Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html#bridgehead_N1267326).
    
-   To set up USPS accounts, see [Register a USPS Account with NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283332.html).
    

Important:

When you use the Shipping Label Integration in NetSuite Sandbox or Release Preview accounts, you must use the same production carrier account used in your production NetSuite account.

Any labels generated in Sandbox or Release Preview are live, shippable labels and may incur carrier charges. Contact your carrier directly to understand billing and how to avoid unintended charges.

For more information, see [Important Update: Shipping Label Integration in Sandbox and Release Preview](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046102/kw/1046102) (SuiteAnswers article 1046102).

### Related Items:

-   [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html)
-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [USPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html)
-   [Shipping Integration with FedEx, UPS, and USPS/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html)

## Preferences Subtab {#bridgehead_1545058316}

Entering information in the Preferences subtab can help to generate forms, such as a Shipper's Export Declaration (SED) and NAFTA Certificate of Origin.

#### To complete Carrier Basics: {#procedure_N1257985}

1.  To enable the International subtab for Shipping Label Integration and shipping items internationally using UPS or FedEx, check the **International Shipping** box.
    
2.  To enable restricted material shipping when using FedEx shipping integration, check the **HazMat/Dangerous Goods Shipping** box.
    
    To learn more, see [Shipping Dangerous Goods and Hazardous Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1269990.html).
    
3.  To insure packages by default, check the **Insure Packages** box.
    
    You can override this option on item fulfillments.
    
4.  To not expose your account number on shipping labels, check the **Mask Account Number on Labels** box.
    

#### To complete rates: {#procedure_1545060140}

1.  Select the **FedEx Rates Type** to display and charge customers:
    
    -   **Negotiated Rates** represent the rate FedEx charges shipments.
        
    -   **List Rates** are generic list rates. FedEx still charges the negotiated rates.
        
2.  To mark customer addresses as residential by default, check the **Residential Address for Shipping** box.
    
    If you do not check this box, FedEx and UPS will treat customer addresses as business addresses.
    
    You can also designate residential addresses on individual customer records and sales orders. This information helps return accurate shipping rates from UPS and FedEx. Residential addresses may incur higher shipping rates.
    
    USPS charges the same shipping rates for both residential and business addresses.
    
3.  Select the **UPS Rates Types** to display and charge customers.
    

#### To complete Third Party Billing: {#procedure_1545060148}

1.  If you use Shipping Label Integration and want to bill integrated shipping charges to other FedEx or UPS accounts, check the **Third Party Billing** box.
    
    For example, if your company has a production account, each location can bill the production account as a third party. You can also choose to bill a customer or distributor's UPS or FedEx account.
    
    Checking this box enables third party account fields on the company information page, customer records, and item fulfillments.
    
2.  To remove shipping charges on orders where third party shipping is used, check the **Do Not Charge Shipping on Third Party Billing Orders** box.
    
    This prevents the customer from being charged twice for shipping.
    
3.  To remove handling charges on orders where third party shipping is used, check the **Do Not Charge Handling on Third Party Billing Orders** box.
    
4.  For international shipments, select a **Fedex Duty Payment Type**:
    
    -   **None Selected** - FedEx bills your account
        
    -   **Recipient** - FedEx bills the recipient
        
        When fulfilling the order, enter the recipient's FedEx account number on the **Shipping** subtab
        
    -   **Third Party** - FedEx bills a third party
        
        When fulfilling the order, enter the account number to bill on the **Shipping** subtab.
        
    
    If you have enabled the integrated shipping labels feature, specify the type of packaging you most frequently use with FedEx, UPS and USPS services in the **Default Package Type** section.
    

#### To complete Default Package Type: {#procedure_1545060154}

1.  Select a **Fedex Packaging** type.
    
    If you select **Your Packaging**, select the packaging type in the **FedEx Admissibility Package Type** field.
    
2.  Select the type of **Fedex One Rate Packaging** you use most often.
    
3.  Select an item fulfillment default **UPS Packaging** type.
    
4.  Select an item fulfillment default **USPS Packaging** type.
    

#### To complete References Fields: {#procedure_1545060160}

1.  Select additional information to include on packages to help with package tracking from **Reference #1**.
    
    This information is copied to the order fulfillments reference fields packages subtab. This information is included on all multiple package orders.
    
2.  UPS and USPS support more information in the **Reference #2**.
    
    If you select Item Name, the name of the first item on the order is used.
    

#### To complete Address Validation: {#procedure_1545060168}

1.  To validate the delivery address when fulfilling orders, check the **FedEx Address Validation** and **UPS Address Validation** boxes.
    
    Only shipping addresses are validated. Return shipping addresses are not validated.
    
    UPS validates in the United States and Puerto Rico only. FedEx also validates addresses in Canada.
    
2.  If you completed the Number of Days to Shipment field, enter the holiday dates you don't ship in the **Holiday Date** column.
    
3.  Enter a holiday **Description**.
    
    These holidays are skipped when calculating the ship date for orders. New holiday dates should be entered each year.
    
4.  Click **Add**.
    

## Packages Subtab {#bridgehead_N1258591}

If you use Shipping Label Integration, you can create package types to capture the shipping information for the packaging you use most often. A package type defines the dimensions (measurements), the weight, and the maximum number of items that can be shipped in a package. You can create a package type on the **Packages** subtab and then assign it on item records to automatically enter the package details when shipping the item.

#### To enable shipping label integration:

1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
    
4.  Click **Save**.
    

#### To set up a package type: {#procedure_N1258634}

1.  Go to _Setup > Accounting > Shipping_.
    
    If you use Pick, Pack, and Ship, you can set your Default Item Fulfillment Integration Stage to Packed or Shipped.
    
    If your integration stage is Picked, packages are not automatically created based on your items and package types.
    
2.  In the **Packages** subtab, enter a package **Name**.
    
    For example, eBay Package or Largest Box.
    
3.  Enter the package **Length** measurement in inches.
    
4.  Enter the package **Width** measurement in inches.
    
5.  Enter the package **Height** measurement in inches.
    
6.  If the package **Weight** is the same every time, enter the weight in pounds.
    
7.  Enter the highest number of items that would ship in this type of package in the **Maximum Items** column.
    
    When an item is selected for this package type and the order quantity is greater than one, or other items will be included in this package type, the maximum number of items is included in one package.
    
    For example, speaker sets and keyboards use a medium box. The maximum number of items set is three (3). When an order is created for two speaker sets and one keyboard, they are placed into one medium box.
    
    If an item always ships in its own package with no other items, do not enter a separate package for that item. Enter the default package type, and then check the **Ships Individually** box on the item record.
    
    Note:
    
    If you do not enter a maximum number of items, the package type maximum number of items is assumed to be unlimited until the total weight is equal to or greater than 150 lbs.
    
8.  To designate the default package type for all items that do not have a package type defined, check the **Default** box.
    
9.  Click **Add**.
    
    Repeat these steps for each type of package you ship.
    
10.  Click **Submit**.
     

After you set up your most-used packages, set packages for an item on the Basics subtab of each item record.

When an item is selected on an order, the item package type is automatically selected in the Your Packaging field on the packages subtab of the fulfillment. The number of packages is calculated based on the number of items on the order and the number of items allowed in each package type.

### Related Items

-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Charging for Shipping and Handling per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1260542.html)
-   [Shipping Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262219.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

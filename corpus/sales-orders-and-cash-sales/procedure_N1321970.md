---
id: "procedure_N1321970"
type: "procedure"
title: "Contract Renewals Creation"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Setting Up Contract Renewals Preferences > Contract Renewals Creation"
parent: "section_N1321619"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N1321970.html"
anchors: []
sha256: "a79d25afd2f442d07767cadacc0882ce028ca3cb8665a7d906ab27b89479487a"
---

These preferences affect how renewal transactions are created:

| Field | Description |
| --- | --- |
| Enable Script R05 | Check this box to enable the script that creates renewal transactions. |
| Restrict to Customer | Check this box to create renewal transactions only for a specific customer. Important: This setting is used for testing purposes. Be sure to clear this box when you're finished testing. |
| Default Renewal Form ID | Select the custom transaction form you want to use when creating renewal transactions. For more information about contract renewals transaction forms, see [Setting Preferred Forms for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321283.html). |
| Renewal Form Based From | If you're using multiple renewal transaction forms, select whether you want the form chosen based on subsidiary or channel tier. If this field is blank, the form selected in the **Default Renewal Form ID** field is used. |
| Zero Dollar Item | Zero price item is used by Contract Renewals to retrieve dynamic values when generating renewal transactions. For more information, see [Creating a Zero Price Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321133.html). |
| Renewals License Pricing Model | Select the pricing model that you want to use for contract value calculation and pricing of renewed items. For information about how contract values are calculated for each pricing model, see [Contract Value Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4473187166.html).
-   **Current License List Rate - Price Level on Customer Record** - Calculates the contract value based on the price level set on the customer record and its corresponding price specified on the item record. If there is no price level specified on the customer record, the base price on the item record is used to calculate the contract value.
-   **Historical License List Rate - From Tran Line** - Calculates the contract value based on the price level and list rate specified on the contract's source transaction.
-   **Current License List Rate - Price Level on Contract** - Calculates the contract value based on the price level set on the contract's source transaction and its corresponding price specified on the item record. If a custom price level is specified on the source transaction (that is, contract price level is blank), the base price on the item record is used to calculate the contract value.
-   **Current License List Rate - Price Level on Contract with Custom Price Handling** - Calculates the contract value based on the price level set on the contract's source transaction and its corresponding price specified on the item record, with the option to set a custom price on the source transaction. If a custom price level is specified on the source transaction (that is, contract price level is blank), the original list rate specified on the source transaction is used to calculate the contract value. When a custom price is set on the contract and the Renew With item is the same as the original item, the renewal contract uses the custom price for the item on the source transaction. If the Renew With item is different, the renewal contract uses the base price of the renewal item.

 |
| Days Before Renewal | Enter the number of days prior to a contract's end date when a renewal transaction is generated. Default value is 90. You can override this preference for specific contracts by specifying a value in the **Contract Days Before Renewal** field on the contract record. For more information, see [Editing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448152522.html). |
| Default Renewal Period | Enter the default renewal term in months. |
| Transaction Type to Create | Select the type of transaction that is created by the renewal process. Note: When creating a renewal transaction form mapping, the transaction type on the mapping must match the value set in this preference. Otherwise, the contract won't be renewed. To create a renewal transaction form mapping, go to Setup > Custom > Renewal Tran Form Mapping > New. |
| Assign To | Select whether the renewal transaction is assigned to a sales representative of the customer or to a specific employee. If you select **An Employee**, choose an employee in the **Assign to Employee/Default** field. |
| Assign to Employee/Default | Select the employee to be assigned to renewal transactions by default. |
| Transaction Department Based On | Select how the department is set on the renewal transaction:

-   **Sales Rep (Department, Location, and Class)** - The sales representative's department is set on the transaction.
-   **None** - Department isn't set on the transaction.

 |
| Transaction Location Based On | Select how the location is set on the renewal transaction:

-   **Sales Rep (Department, Location, and Class)** - The sales representative's location is set on the transaction.
-   **None** - Location isn't set on the transaction.

 |
| Transaction Class Based On | Select how the class is set on the renewal transaction:

-   **Sales Rep (Department, Location, and Class)** - The sales representative's class is set on the transaction.
-   **Order Type** - Class is set with all order types.
-   **None** - Class isn't set on the transaction.

 |
| Include Tran Line Description | Check this box to copy transaction line descriptions to renewal transaction lines. Transaction line descriptions are always copied to contract item records. |
| Default Customer Discount Renewals | Check this box to apply customer discounts on renewal transactions by default. |
| M/S In-Line Discount | Check this box to apply a line item discount to maintenance and support items. This preference applies only when the **Inline Discounting on Trans** preference is checked. |
| Combine Like Items | Check this box to combine similar line items on renewal transactions. Line items are combined if the item, end date, and list rate all match. Note: When items have different discount rates, no discount rate will be applied to the combined item. Note: When the original transaction contains same items that use custom price levels with different list rates, these items aren't combined if the Renewals License Pricing Model is either **Current License List Rate - Price Level on Contract with Custom Price Handling** or **Historical License List Rate - From Tran Line**. Otherwise, the said same items are combined. |
| Require Same Discount when Combining Like Items | Check this box to combine like items only when the items have the same discount rates. |
| Apply Upsell and Downsell on Renewal Transaction | Check this box if you want to include upsell and downsell items when generating contract items on renewal transactions. Contract items will be classified by order type on the renewal transaction. Added items are classified as upsell and removed items are classified as downsell. Clear this box if you want to include only the final items (after upsell and downsell orders are applied to the original contract) when generating contract items for renewal transactions. |

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

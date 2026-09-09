---
id: "section_N1391837"
type: "section"
title: "Setting Up Accounting Lists"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Features and Preferences > Setting Up Accounting Lists"
parent: "chapter_N1383640"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391837.html"
anchors: []
sha256: "da39e00b19475e140c0e499e0cad714e0cfbf613b164f68f88811fbff874a7cb"
---

NetSuite provides several predefined categories used to group records. These categories are called lists because each category can includes a list of values that can be set on records. Some lists have system-defined values, but you can add values to most lists as required by your business. System-defined values and the values you add to these lists, display as options in lists for related fields. The system displays a maximum of 10,000 records in these lists.

Accounting lists provide values for accounting-related groupings on a variety of records, including transactions, items, budgets, customers, projects, and vendors.

-   To review existing values available for the various accounting lists, go to _Setup >Accounting > Accounting Lists_. Values are grouped alphabetically by list name, and within that, alphabetically by value description.
    
-   To add a value to an accounting list, go to _Setup > Accounting > Accounting Lists > New_, and click on a list. Complete field(s) and click Save. You can click the New button to add another value.
    
    Note:
    
    Changes made to accounting lists are captured in system notes. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).
    

The following lists may be available in your account:

| List | Description |
| --- | --- |
| Billing Class | Billing class values are used on employee records to set billable time rates for service items. For more information, see [Using Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233375.html). |
| Budget Category | This list is available if the Multiple Budgets feature is enabled. Budget category values are used on budget records to categorize types of budgets. In NetSuite OneWorld, budget category values are used indicate whether budgeting is done at the local subsidiary level in local currency or globally using the root subsidiary's currency. Each budget category is associated with a budget category type of Local or Global. See [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html). |
| Charge Type | List for the type of service of the subscription plan items that use a specific charge plan. Note: If this object was installed as part of a bundle, the Bundle ID column displays the bundle that includes the Charge Type object. The Bundle ID column applies to only the Charge Type accounting list. |
| Cost Category | This list is available if the Landed Cost or Standard Costing feature is enabled. Cost categories have two purposes:
-   Material or Service Cost categories track standard costs for items. For more information, see [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html).
-   Landed Cost Category values are used for items on bills and item receipts to categorize the different kinds of expenses incurred when making purchases. For more information, see [Landed Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417902.html).

 |
| Customer Category | Customer categories are used on customer records to categorize them. A common use is to define the source of each customer. |
| Customer Message | Customer message values can be selected on transaction records to include standardized messages to customers. For example, a message of "Thank you for your order!" can be selected on an invoice record to be displayed on the invoice sent to the customer. To create a customer message, go to _Setup >Accounting > Accounting Lists_ and click New. Then, click the Customer Message link, complete the fields and save. |
| Distribution Category | This list is available if the Distribution Resource Planning feature is enabled. Distribution categories are used to set up a distribution network for supply planning. For more information, read [Creating a Distribution Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4049501123.html). |
| Incoterm | This list is available if the Purchase Contracts feature or Blanket Purchase Orders feature is enabled. This is a standardized three-letter trade term used on transactions related to international commercial procurement practices that communicate the tasks, costs, and risks associated with the transportation and delivery of goods. Incoterms define where the customer takes ownership of the product and are typically used for international orders, such as when an item goes through customs or crosses a border. This is an expansion of a concept similar to FOB terms used in the United States. For more details, read [Creating Purchase Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077190978.html) or [Creating a Blanket Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4083950023.html). |
| Order Type | This list is available when the Warehouse Management feature is enabled. On order transactions, use order types to associate attributes to orders. See [Creating Order Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541433528.html). |
| Other Name Category | Other name category values are used on Other Name records to categorize them. The list of other name records is a collection of records for people or companies who are not vendors, customers or employees. You can use Other Name records to track other people or companies to whom you write checks or from whom you receive deposits. For example, your company might donate money to a favorite charity, so you can create an other name record for the charity. You might also list your owners and partners here if they contribute or withdraw equity. |
| Payment Method | Payment method values are used on transactions such as cash sales and customer payments, to specify how payment was received. Possible payment methods include cash, check, credit card, money order, or PayPal™. For more information, see [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html). For more information about setting up PayPal processing, see [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html). |
| Price Level | This list is available when the Multiple Prices features is enabled. Price level values are used on item records to enable you to set up multiple prices for each item. When you create price level values, they automatically appear on item records with space for you to assign a price to each level. If the Quantity Pricing feature is enabled, you can assign quantity-based prices for each level. For more information, see [Creating Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181938.html). |
| Pricing Group | This list is available when the Multiple Prices feature is enabled. Pricing group values are used on customer and item records to enable the creation of customer-specific pricing for items. For more information, see [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html). |
| Project Status | This list is available when the Projects feature is enabled. Project status values are used on project records to indicate the progress of projects. For more information, see [Creating a Basic Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179164.html). |
| Project Type | This list is available when the Projects feature is enabled. Project type values are used on project records to categorize them in whatever manner is needed. You can create a hierarchy of project types by identifying a subtype for each type value. |
| Revenue Allocation Group | This list is available when the Advanced Revenue Management (Revenue Allocation) feature is enabled. The revenue allocation group value is used in the GroupSum function in fair value formulas. For more information, see [Fair Value Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4331943130.html) and [GroupSum Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4352551823.html). |
| Term | Term values are used on invoice and customer records to specify when payment is due. You can select terms on a customer record to default on all invoices for that customer. You also can select terms on an invoice to apply to that transaction only. For more information, see [Creating Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html). |
| Transaction Deletion Reason | This list is available when the Use Deletion Reason feature is enabled. You can create unique reasons why a transaction was deleted and choose the languages in which the reason should display. You can also inactivate specific deletion reasons if they no longer suit your needs. For more information, see [Recording a Reason for Deleting a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4338624600.html). |
| Vendor Category | Vendor categories are used on vendor records to categorize them. |
| 1099-MISC Category | This list's values are used for 1099 forms that you issue to vendors. You can't add values to this list. |

Other lists in addition to Accounting Lists are available for use in categorizing other types of records:

-   Employee related lists provide values to group employee records. See [Setting Up Employee Related Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1394576.html).
    
-   CRM lists provide customer relationship management values to group records such as contacts, sales representatives, partners, and campaigns. [CRM Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1044602.html).
    
-   Users with the Custom Lists permission can create additional, custom lists to categorize records, by going to _Customization > Lists, Records, & Fields > Lists > New_.
    

### Related Topics:

-   [Accounting-Related Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1383904.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html)
-   [Setting Up Employee Related Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1394576.html)
-   [Accounting Features and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1383640.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

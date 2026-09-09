---
id: "section_N2839994"
type: "section"
title: "Sourcing and Filtering Examples"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Sourcing and Filtering Examples"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839994.html"
anchors: []
sha256: "4ffc9c18d3b5c44773d61359ef9522af25614095974c76e36f8a081da2e338f5"
---

This topic provides some examples of how you can use the Source Filter by field to create dynamic custom fields.

Let's say you want to link two transactions, such as a sales order and a subsequent credit memo. First, create a transaction custom field and add it to customer credit memos (using a custom form to limit it to the credit memo form only). For more information, see [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html) and [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html)

On the transaction custom field record, set these field values:

-   List/Record - Transaction
    
-   Source List - Entity
    
-   Source Filter by - Customer
    

When you select a customer on the credit memo, NetSuite fills the new list field with transactions for that customer only.

Here's an example of the setup for a new transaction body field called Associated Transaction that uses the setup criteria described previously. In addition, The Sale box is checked on the Applies To subtab, so that the new field appears only on Sale transaction types, such as credit memo.

![Transaction Body Field record showing sourcing settings.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/LinkedOrderTransBodyField.png)

On the credit memo, the associated transactions for the selected customer are available in the new Associated Transaction field. All associated transactions are listed because no filters were applied.

![Associated Transaction field showing list of transactions for a customer.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CreditMemoAssocTrans.jpg)

Now, suppose you want to create a similar field called Associated Sales Order on the same credit memo that lets you choose only a sales order from the available sales order for that customer.

Create the new field using the same setup that was used to create the previous Associated Transaction field. For this example, also include a filter to limit the list to include only transactions of a particular type (sales orders). When you create a new credit memo, and select a customer, the Associated Sales Order list will show only sales orders from that customer.

The following example shows the setup for a transaction body field called Associated Sales Order that uses the setup criteria described previously. In addition to the sourcing criteria, this example contains filtering criteria that includes only the Sales Order transaction type.

![Fliter settings for Associated Sales Transaction field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/AssocSalesTransField.jpg)

On the credit memo, only sales orders for the selected customer are available in the new field.

![Associated Sales Transaction field on credit memo showing only sales orders for a customer.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/AssocSalesTransCreditMemo.jpg)

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Assigning Custom Fields to Specific Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html)
-   [Behavior of View from Order Only Settings on Transaction Line and Transaction Body Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0528113109.html)
-   [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html)
-   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
-   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
-   [Setting Filtering Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html)
-   [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html)
-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html)
-   [Creating Read-Only Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842596.html)
-   [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html)
-   [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html)
-   [Tracking Changes to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_54095541974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

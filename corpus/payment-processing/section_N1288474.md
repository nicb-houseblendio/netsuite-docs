---
id: "section_N1288474"
type: "section"
title: "Consolidated Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Payments > Consolidated Payments"
parent: "section_N1285644"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html"
anchors: ["bridgehead_N1288603", "bridgehead_N1288692", "bridgehead_N1288753", "bridgehead_N1288768"]
sha256: "367d9c033802cce46c4a60cbb2e005af6e376ba3a1d0e1185fa9c70eda8b784c"
---

If you sell to customers who have subcustomers, the Consolidated Payments feature gives you the flexibility to accept payment for subcustomer invoices from either the top-level customer or from the individual subcustomer.

With this feature enabled, when you select a top-level customer in the Customer field at _Customers > Accounts Receivable > Accept Customer Payments > List_, the Invoices subtab shows both the invoices entered for the top-level customer as well as the open invoices for each of its subcustomers.

Additionally, when a top-level customer is selected on the Payment page, the Deposits and Credits subtabs list all of the deposits and credits entered for the top-level customer and its subcustomers. These credits and deposits can be applied to any of the open invoices entered for the top-level customer or its subcustomers.

If you allow customers to make payments through the Customer Center, top-level customers can make payments on their invoices or the invoices of their subcustomers. They can also apply any credits or deposits to these invoices. For more information, see [Allowing Customers to Pay Online](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293669.html).

To enable the Consolidated Payments feature, go to _Setup > Company > Setup Tasks > Enable Features > Accounting (Administrator)_, click the Accounting subtab, and check the Consolidated Payments box. After enabling the feature, you can go to _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_, and enable the **Apply Payments Through Top-Level Customer Only** preference if you want to only apply payments, credits, and deposits through the top-level customer.

For more information on accepting payments, see [Applying a Payment on the Customer Payment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288824.html).

For information on consolidated payments and the Multiple Currencies feature, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

## Consolidated Balance Fields {#bridgehead_N1288603}

To help you track the consolidated balance for a customer-subcustomer hierarchy, when you enable this feature, the following consolidated balance fields are shown on the Financial subtab of customer records:

-   **Consolidated Balance** - the total of all open invoices for the entire customer-subcustomer hierarchy.
    
-   **Overdue** - shows the total overdue balance for all customers and subcustomers in the hierarchy
    
-   **Days** - the number of days the consolidated overdue balance is past due
    
-   **Consolidated Deposit Balance** - the total amount of unapplied deposits for all subcustomers and customers in this hierarchy
    
-   **Consolidated Unbilled Orders** - the total amount on orders for the customers and subcustomers in this hierarchy that have been entered but not billed
    
-   Consolidated aging fields - show the current consolidated balance broken down into amounts in each aging category (1 - 30 days, 31 - 60 days, etc.).
    

These fields can be added to custom reports by selecting the consolidated fields from the Customer folder. The consolidated fields are also available when performing a customer search. If you use the Multiple Currencies feature, balance fields on the customer record are shown in the customer's currency. To add these fields to searches or reports, you can choose between either the fields in the base currency or the foreign currency.

## Customer Statements {#bridgehead_N1288692}

With the Consolidated Payments feature, you can print either individual customer statements or consolidated statements with balance information for the entire customer-subcustomer hierarchy.

To print a single consolidated statement, go to _Customers > Accounts Receivable > Individual Statement_, and check the Consolidated Statement box. To print consolidated statements for multiple customers, go to _Billing > Sales > Generate Statements_, and check the Consolidated Statements box. For more information, see [Customer Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300430.html).

If you use a custom invoice form to include balance information on printed invoices and use the Consolidated Payments feature, these fields show the consolidated balance. For more information, see [Printing Mini Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1301336.html).

You can add Deposit Balance and Net Amount Due information to customer statements. For more information, see [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html).

## Credit Limits and Holds {#bridgehead_N1288753}

With the Consolidated Payments feature enabled, the credit limit defined for a top-level customer is the applied to the entire hierarchy. With this feature enabled, credit limits set on individual subcustomer records are not enforced.

Likewise, manual credit holds placed on the top-level customer are applied to the entire hierarchy.

## Reports and KPIs {#bridgehead_N1288768}

With Consolidated Payments, the A/R Aging report shows the un-consolidated balance for each subcustomer. Amounts are totaled for each customer-subcustomer hierarchy allowing you to see the consolidated balances.

The following consolidated KPIs are available on customer dashboards with the Consolidate Payments feature:

-   Consolidated Balance
    
-   Consolidated Overdue Balance
    
-   Consolidated Unbilled Orders
    
-   Consolidated Days Overdue
    
-   Consolidated Average Days Overdue
    

### Related Topics:

-   [Accepting Customer Payments Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html#section_N1288273)
-   [Applying a Payment on the Customer Payment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288824.html)
-   [Applying a Payment on an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1289458.html)
-   [Correcting Payments to Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292877.html)
-   [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html)
-   [Removing Credits from Deleted Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292961.html)
-   [Reversing or Deleting Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4744566376.html)
-   [Approving Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4373987935.html)
-   [Managing Undeposited Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1294497.html)
-   [Payment Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293235.html)
-   [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html)
-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)
-   [Allowing Customers to Pay Online](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293669.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

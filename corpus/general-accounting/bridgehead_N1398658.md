---
id: "bridgehead_N1398658"
type: "bridgehead"
title: "Currency on Customer Transactions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Assigning Currencies to Entities > Customers and Multiple Currencies > Currency on Customer Transactions"
parent: "section_N1398493"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1398658.html"
anchors: ["bridgehead_N1398725", "bridgehead_N1400310", "bridgehead_N1398805"]
sha256: "d2714cce80d938503bdab96ab18a5134b02d3295aef1675ea7eff20967065618"
---

When you enter a transaction for a customer, the customer's primary currency is selected by default. In the Currency field, you can select a different transaction currency from the customer's record before you save the transaction. The location of the Currency field varies depending on the transaction.

If you change the currency before you save the transaction, NetSuite converts shipping rates, prices, gross profit, and other currency amounts to the new currency. Billable items, expenses, and time are also recalculated when you change the currency on a sales transaction.

Exceptions to automatic recalculation are as follows:

-   If you enter a custom price for a line item and then change the currency, the rate isn't converted to the new currency.
    
-   The forecast fields on opportunities aren't recalculated when you change the currency.
    

You can't change the currency after the transaction has been saved. If the currency is incorrect, you can make a copy of the transaction and change the currency on the copy.

When using the Invoice Billable Customers page to generate invoices in bulk, you create invoices only in a customers' primary currency.

Customers who place orders through the Customer Center or the My Account section of the web store can select any transaction currency included on their customer record. In web store checkout, customers can place orders only in their primary currency.

You can enter journal entries and intercompany journal entries for a customer in any currency used by that customer. If you have a customer who is also a vendor, the customer's vendor currencies are also available for the journal entry currency. For instructions, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).

When you apply a gift certificate, the list of gift certificates includes only the available gift certificates in the transaction currency. For more information, see [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html).

See the following sections for additional information about the behavior of currency on customer transactions:

-   [Transaction Workflows](#bridgehead_N1398725)
    
-   [Projects and Transactions](#bridgehead_N1400310)
    
-   [Accepting Payments](#bridgehead_N1398805)
    

## Transaction Workflows {#bridgehead_N1398725}

When you convert a sales transaction to another sales transaction in the sales process, **the currency from the original transaction is maintained. You can't change it later in the process**.

This includes the following workflows:

-   Estimate to opportunity or sales order
    
-   Opportunity to sales order
    
-   Sales order to invoice
    
    This includes the Bill Sales Orders page and the Invoice Billable Customers page. Invoices are created in the same currency as the sales order.
    
-   Sales order, invoice, or cash sale to return authorization to refund or credit
    
-   Deposit to refund
    

You can change the currency on a copy of a transaction. All currency amounts (except custom prices) are converted to the new currency.

Finance charges accrue in the currency of the overdue transaction. The Assess Finance Charges page shows a line for each customer in each currency in which a finance charge has been incurred. For more information, see [Finance Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1301640.html).

## Projects and Transactions {#bridgehead_N1400310}

Projects and their associated transactions must share a single currency. When you select a customer on a new project record, you can select any of this customer's transaction currencies. The same currency is used for any sales transaction associated with the project. Any subproject records use the currency of the parent project.

When adding project items to sales transactions, the currency of the project must match the transaction currency.

When creating a project from a sales order line, the project inherits the currency of the sales order.

## Accepting Payments {#bridgehead_N1398805}

When you click Accept Payment on an invoice or customer record, the value in the Currency field is set by default. You can change the value, but the value you select determines the list of invoices to which you can apply the payment. NetSuite expects the payment currency to match the invoice currency. The default values for the Currency field on a payment are as follows:

-   When you accept the payment from the invoice, the payment uses the invoice currency.
    
-   When you accept the payment from the customer record, the payment uses the customer's primary currency.
    

You can only accept credit card payments in currencies for which you've set up credit card processing profiles. For more information, see [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html).

With the Consolidated Payments feature, you can accept payments for any open invoice in any currency used by any customer in the hierarchy. If you accept payment through a top-level customer, the invoice currency must be a currency associated with that top-level parent. For information about this feature, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).

### Related Topics

-   [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html)
-   [Item Sales Prices and Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1398871.html)
-   [Website Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

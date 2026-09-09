---
id: "bridgehead_N1400109"
type: "bridgehead"
title: "Balance Information for Entities with Multiple Currencies"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Assigning Currencies to Entities > Balance Information for Entities with Multiple Currencies"
parent: "section_N1397405"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400109.html"
anchors: ["subsect_161610274695", "subsect_161610501614"]
sha256: "b9e701def2ca837a1a0be8e064d7083d50de7daeffce2d0a53c06cc018bd15ea"
---

The currency used to display balance information depends on the type of entity and the access. Balances displayed on entity records and reports in NetSuite are in the base currency for your company or subsidiary. For exceptions to this general rule, see the following:

-   [Customer Balances in Transaction Currencies](#subsect_161610274695)
    
-   [Vendor Balances in Transaction Currencies](#subsect_161610501614)
    

By default, KPIs and reports are in the base currency for your company or subsidiary. NetSuite converts foreign currency balances to base currency using the exchange rates on the transactions. For more information, see [Currency on Customer Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1398658.html) and [Currency on Vendor Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400935.html).

In NetSuite OneWorld, subsidiary base currency amounts for consolidated reports are converted again as needed for the subsidiary context. For details, see [Consolidated Reporting in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278654.html).

A/R and A/P reports also show transaction and balance amounts in the base currency. You can, however, customize these reports to add the foreign currency information. **Amount (Foreign Currency)** is under Unpaid Receivables Transactions in the A/R reports. In the A/P reports, this field is under Open Payables. **Currency : Name** displays the name of the source transaction currency. For instructions, see [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html).

## Customer Balances in Transaction Currencies {#subsect_161610274695}

If Customer Access is enabled in your account, you can give your customers access to view their information in the Customer Center. Customers see their balance information in their primary currency. NetSuite converts balances in other currencies to the customer's primary currency. For more information, see [Giving Customers Access](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322750.html).

In customer records, the Financial subtab includes balances for all currencies. Balances in each currency appear in the Currencies subtab, as shown in the following screenshot. If you use the Consolidated Payments feature, consolidated balance information is shown in each currency.

![Screenshot showing customer record Financial subtab Currencies subtab with balances in transaction currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/CustomerFinancialCurrencies.png)

Customer statements, printed both individually and in bulk, include separate statement pages for each currency the customer has a balance in. For information, see [Customer Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300430.html).

With the Consolidated Payments feature, each currency that's used by any customer in the customer hierarchy gets a separate page in the consolidated statement. For details, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).

In advanced and saved customer searches, the **Customer Currency Balance** related record field includes the following fields for balances in transaction currencies:

-   **Balance (Foreign Currency)** - This field displays the transaction currency balance amount for the currency in a line on the search results.
    
-   **Currency** - This field displays the name of the currency. When you select this field, the results include a line for each transaction currency associated with the customer.
    
-   **Deposit Balance (Foreign Currency)** - This field displays the total deposit balance for each of a customer's transaction currencies.
    
-   **Last Financial Charge Date (Foreign Currency)** - This field displays the date of the last finance charge in each of a customer's transaction currencies.
    
-   **Unbilled Orders (Foreign Currency)** - This field shows the unbilled sales order total in each of a customer's transaction currencies.
    

## Vendor Balances in Transaction Currencies {#subsect_161610501614}

On vendor records, the Financial subtab includes balances for all currencies. Balances in each currency appear in the Currencies subtab. The Currencies subtab on the vendor record includes columns only for Balance and Unbilled Orders.

Credit limits for each vendor are displayed in the Credit Limit field in the vendor's primary currency. The Credit Limit field is in the Account Information section of the Financial subtab.

In advanced and saved vendor searches, the **Vendor Currency Balance** related record field includes the following fields for balances in transaction currencies:

-   **Balance (Foreign Currency)** - This field displays the transaction currency balance amount for the currency in a line on the search results.
    
-   **Currency** - This field displays the name of the currency. When you select this field, the results include a line for each transaction currency associated with the vendor.
    
-   **Unbilled Orders (Foreign Currency)** - This field displays the unbilled purchase order total in each of a vendor's transaction currencies.
    

### Related Topics

-   [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html)
-   [Duplicate Entity Records with Different Primary Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400329.html)
-   [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html)
-   [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

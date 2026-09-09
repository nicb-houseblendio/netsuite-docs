---
id: "section_N1784998"
type: "section"
title: "Using Foreign Currency Amortization"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Foreign Currency Amortization > Using Foreign Currency Amortization"
parent: "section_N1784814"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784998.html"
anchors: ["bridgehead_N1785150", "bridgehead_N1785196", "bridgehead_N1785286", "bridgehead_N1785364", "procedure_N1785401", "bridgehead_N1785464", "bridgehead_N1785484"]
sha256: "59e97d8302a61ef0870615d343495f4560f9e3f8dc83e5780aa5278ffab14f71"
---

Note:

Foreign currency amortization is available only in NetSuite U.K. editions.

Use the same process to work with foreign currency amortization that you use to amortize expenses in a single currency. The basic amortization process involves these steps:

-   **Create templates.** For information, see [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html) . .
    
-   **Associate amortization templates with item and expense records.** See [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html) and [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html).
    
-   **Generate amortization schedules.** [Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html).
    
-   **Create amortization journal entries.** See [Generating Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1779279.html). .
    
-   **View amortization reports.** See [Amortization Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1789982.html).
    

Although the general process is the same, each part of the process has additional elements specific to foreign currency amortization.

## Amortization Templates {#bridgehead_N1785150}

The Amortization Template displays the Use Transaction Currency check box. This check box controls whether the template calculates the amortization schedule amounts in a foreign currency or in the base currency. You must check this box when creating a foreign currency template to generate amortization schedules in a foreign currency. You can't specify a currency when you create a template. The template always refers the transaction to determine the currency for amortization.

Use a naming convention for amortization templates so you can distinguish foreign currency amortization templates from standard amortization templates. For example, add the currency code to the template name, such as Even Periods - USD and Even Periods - Foreign.

If you associate a foreign currency template on a base currency transaction line, it creates an amortization schedule for the item using the base currency, which is a standard amortization schedule. This has the same result as if you use an amortization template where the Use Transaction Currency box isn't checked. Depending on your business needs, you may be able to use foreign currency templates to amortize amounts for both foreign and base currency transactions.

If you check the Use Transaction Currency box for a template and populate the Initial Amount or Residual fields, the amortization schedule created from the template assumes or uses the currency of the transaction. For example, on a foreign currency amortization template, you enter 100 in the Initial Amount field. You associate the template on a transaction recorded in GBP. On the amortization schedule, the 100 represents 100 GBP.

## Foreign Currency Amortization Schedules {#bridgehead_N1785196}

The foreign currency amortization schedule displays the base currency and the foreign currency amortization amount information in the following fields. You can add these fields to your amortization searches, lists, and reports.

-   **Foreign Currency** - indicates if the schedule is a foreign currency schedule
    
-   **Currency** - indicates the currency used in the schedule to calculate amounts. This is the transaction currency.
    
-   **Base Amount** - the amortization amount converted to the base currency (the foreign currency amount for the period multiplied by the transaction exchange rate)
    
-   **Amount** - the amount to be recognized for a line of the schedule
    
-   **Total Amortized** - shows the cumulative amount already recognized on the schedule to date
    

The currency of the transaction determines the currency for the amortization schedule amounts. The transaction currency becomes the amortization schedule currency. Amounts to be amortized are shown in the Amount column. The base amount shows the foreign currency amount for period multiplied by the transaction exchange rate on the transaction.

Note:

The total amortization amount in the **Base Amount** column may be slightly different from the total base currency amount on the related transaction due to rounding. You may want to journal out these rounding differences periodically.

## Foreign Currency Amortization Journals {#bridgehead_N1785286}

Create foreign currency amortization journals the same way you create standard amortization journals. Foreign currency journals use the exchange rate on the transaction to determine the foreign currency journal amounts.

NetSuite segregates journals by currency type. You will have, at a minimum, one journal per currency per currency exchange rate. For example, you have four amortization schedules:

-   Schedule 1 using USD, your base currency
    
-   Schedule 2 using GBP and transaction exchange rate 2.1
    
-   Schedule 3 using GBP and transaction exchange rate 2.2
    
-   Schedule 4 using EUR and transaction exchange rate 1.1
    

NetSuite creates four amortization journals, one for each amortization schedule.

Note:

If Schedule 2 and Schedule 3 in the example use the same exchange rate, then NetSuite creates only three amortization journals.

## Foreign Currency Amortization Reports {#bridgehead_N1785364}

You must customize the standard amortization reports to display foreign currency amortization information. The amortization reports are:

-   Amortization Forecast Summary
    
-   Amortization Forecast Detail
    
-   Deferred/Capitalized Expense
    

#### To customize amortization reports for foreign currency amortization: {#procedure_N1785401}

1.  Go to the amortization report and click **Customize**.
    
2.  On the Report Builder (or Financial Report Builder), click **Edit Columns**.
    
3.  In the Add Fields pane, select **Amount (Foreign Currency)** and **Schedule Currency**.
    
4.  In the Report Preview pane, leave the default heading or enter a new heading for each column. Reorder columns as needed.
    
5.  Click **Save**.
    

## Foreign Currency Amortization Forecast Reports {#bridgehead_N1785464}

The Amortization Forecast reports display the forecasted value of the amounts to be amortized or the amounts that have already been amortized based on the related amortization schedules. When it's customized for foreign currency, the Amortization Forecast reports display the foreign currency amortization amounts and currency in addition to the amortization amount in the base currency.

Note:

An Amortization Forecast report displays amortization amounts for all currencies. When the report has amounts in more than one currency, the total amortized amount isn't a meaningful number. Filter the report by currency to view accurate amortization total amounts.

## Foreign Currency Deferred/Capitalized Expense Report {#bridgehead_N1785484}

The Deferred/Capitalized Expense report displays the total amortized and deferred expenses for a set of transactions over a period and the recognized portion of those expenses, if any. When it's customized for foreign currency, the report shows the base amount and foreign currency amounts for Amortized Expense, Deferred/Capitalized Expense, and Total. The report doesn't include any revaluation related to the original transactions or related journals.

-   **Amortized Expense Amount** - the amortized expense amounts converted to the base currency for the transaction or transaction line.
    
-   **Amortized Expense Amount (Foreign Currency)** - the amortized amount in the foreign currency related to the amortization journals for the transaction or transaction line. For base currency transactions with standard amortization schedules, the amounts in this column are the same as the Amortized Expense Amount column. The sum of this column doesn't tie to the general ledger because there may be more than one foreign currency.
    
-   **Deferred/Capitalized Expense Amount** - the capitalized expense amounts in the base currency for all amortization journals related to the transaction or transaction line. The total of this column ties to the Balance Sheet for the appropriate period.
    
-   **Deferred/Capitalized Expense Amount (Foreign Currency)** - the capitalized expense amounts in the foreign currency related to the amortization journal for that transaction or transaction line. For base currency transactions with standard amortization schedules, the amounts in this column are the same as the amounts in the Deferred/Capitalized Expense Amount column. The sum of this column doesn't tie to the general ledger because there may be more than one foreign currency.
    
-   **Total Amount** - total of amortized and capitalized amounts in the base currency.
    
-   **Total Amount (Foreign Currency)** - total of amortized and capitalized amounts in the foreign currency.
    

### Related Topics

-   [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html)
-   [Setting Up Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784923.html)
-   [Foreign Currency Amortization Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1785562.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1397082"
type: "section"
title: "Setting a Base Currency"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Setting a Base Currency"
parent: "section_N1395463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html"
anchors: ["procedure_N1397210"]
sha256: "1057faa448426cb133286f8731464be6c2e08fa420e31488f58b844622e39569"
---

When you enable the Multiple Currencies feature, your NetSuite country edition initially sets the base currency. Before you save any transactions, you can choose a different base currency.

If you use NetSuite OneWorld, your NetSuite country edition initially sets the base currency of your root parent subsidiary. Before you save any transactions, you can choose a different base currency for this subsidiary. When you create each additional subsidiary record, you must choose a base currency for that subsidiary. For more information, see [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html) and [Multiple Currencies in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269257.html).

The currency record displays **Is Base Currency** when it has been selected as the base currency for a subsidiary in OneWorld accounts, or on the Company Information page for an account. You can't edit this field on the currency record.

Although transactions default to the currency of the customer or vendor involved in the transaction, transactions post to your general ledger in your base currency. All reports and registers then display currency amounts in your base currency.

For example, if a company in Hamilton, Ontario, Canada issues an invoice to a customer in Buffalo, New York, United States of America, the invoice could be denominated in U.S. dollars (USD), but an accounts receivable report for the Hamilton company would display the amount in the company's base currency, Canadian dollars (CAD).

Be aware that you can define general ledger accounts that use foreign currencies. Typical foreign-denominated accounts include payable, receivable, and bank accounts. In addition, you can define accounts such as Foreign Currency Denominated Loans by assigning the appropriate Account Type to the Account. If you use OneWorld, you can share these accounts across subsidiaries. For information about denominating an account in a foreign currency, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).

#### To change your initial base currency: {#procedure_N1397210}

1.  Go to _Setup > Company > Company Information_.
    
    In NetSuite OneWorld, go to _Setup > Company > Subsidiaries_, and click **Edit** for the subsidiary whose base currency you want to change.
    
    Important:
    
    Make any changes to base currency before you do anything else in NetSuite. If any user has saved a record that includes a currency amount or links to a currency record, you can't change the base currency. You may be able to change the base currency if you first delete all such records.
    
2.  In the **Currency** field, select the currency you want to set as your base currency.
    
    If the **Currency** field is dimmed, another action in the system has blocked the change.
    
3.  Click **Save**.
    
    If you're using the Currency Exchange Rate Integration feature to automatically update currency exchange rates, the time of these daily updates is 6 am in the selected Update Time Zone on the base currency record. The updated rates reflect the latest exchange rates available as of 6:00 a.m. in your selected time zone. The default selection is U.S. Eastern time. See [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).
    

### Related Topics

-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html)
-   [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html)
-   [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

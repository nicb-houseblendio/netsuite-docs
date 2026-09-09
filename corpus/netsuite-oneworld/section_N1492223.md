---
id: "section_N1492223"
type: "section"
title: "Customizing Standard Journal Entries for Intercompany Elimination"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Customizing Standard Journal Entries for Intercompany Elimination"
parent: "section_N1486610"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html"
anchors: ["procedure_N1492251"]
sha256: "60f3e002f596d40bbf6750623f00a4a36d731129feca2904cc418913019beee7"
---

You should use advanced intercompany journal entries (AICJE) to record intercompany transactions.

To use journal entries, you must customize the standard journal entry form to display the To Subsidiary and Eliminate fields. When you add a journal line posting to an intercompany account, the system flags the line to be eliminated during the period close process. See [Enter Intercompany Transactions for Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501665.html).

#### To customize the journal entry form for intercompany elimination: {#procedure_N1492251}

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  Click **Customize** next to **Standard Journal Entry**.
    
3.  Enter a name for the custom journal entry form.
    
4.  On the **Screen Fields** subtab, on the **Main** subtab, check the **Show** box next to the **To Subsidiary** field.
    
5.  In the **Field Group** list, select **Classification**.
    
6.  On the **Lines** subtab, check the **Show** box for the **Eliminate** label.
    
7.  Click **Save**.
    

### Related Topics:

-   [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html)
-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)
-   [Creating Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html)
-   [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html)
-   [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

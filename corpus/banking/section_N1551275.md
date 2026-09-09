---
id: "section_N1551275"
type: "section"
title: "Intelligent Transaction Matching for Bank Data"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Bank Data Matching and Reconciliation > Intelligent Transaction Matching for Bank Data"
parent: "chapter_4842302228"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1551275.html"
anchors: ["subsect_164185356572"]
sha256: "48687acaa2d86157adb6b435a0824ed39166884352d2d7c13ea05516009ff8ad"
---

When bank data is imported into NetSuite or you manually run reconciliation rules, the Intelligent Transaction Matching feature automatically matches imported bank data with account transactions. For details on importing bank data, see [Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1550803.html). For information about running rules against imported data, see [Manually Running Reconciliation Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158991245944.html).

Intelligent Transaction Matching **uses two types of rules on new bank lines** (except for in-transit payments):

Note:

Intelligent Transaction Matching does not run rules against account transactions. Any account transactions that are currently matched can't be matched again, regardless of their reconciliation state.

-   **System Rules** - Default matching rules you can't change or remove. They automatically match imported bank lines to your account transactions. Default rules are listed in the System Rules list on the Reconciliation Rules page. For more information, see [System Reconciliation Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160374863744.html).
    
-   **User Rules** - Custom rules you can create and edit, and choose their order. They're listed in the User Rules list on the Reconciliation Rules page, and include:
    
    -   **Matching rules** - Rules that automatically match imported bank lines with account transactions if they meet the criteria you set. Matching rules are created and edited on the Reconciliation Rules page, and you can apply them to more than one account. For more information, see [Creating User Transaction Matching Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160002098350.html).
        
    -   **Auto-create rules** - Rules that automatically create and match these types of transactions automatically:
        
        -   Deposits and charges for general ledger bank accounts
            
        -   Charges and refunds for general ledger credit card accounts
            
        
        If a bank line matches the criteria in the rule, NetSuite creates an account transaction and matches it automatically. You can edit auto-create rules on the Reconciliation Rules page, but you make them from the Match Bank Data page, during a one-to-one match. You can only use each auto-create rule for one account. For details, see [Generating Auto-Create Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_84132242843.html).
        

To see how NetSuite groups transactions with these rules, see [Grouping Multiple Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_202608110008.html).

To view automatically matched transactions, go to _Transactions > Bank > Match Bank Data_ and then click **Review**.

Note:

If a rule finds two or more possible matches, NetSuite can't choose one, so you need to pick and match the correct transaction yourself.

For example, say you import a $70 bank deposit dated 03/22/2023. NetSuite finds two possibilities: a $70 deposit from 02/14/2023 and another from 01/16/2023. Because both are the right amount and at or before the imported deposit's date, the system can't decide. You need to choose and match the right transaction yourself.

On the **Review** subtab, each line item is a group of matched transactions. By default, all line items are collapsed. To view the individual transactions in the group, expand the line item.

## In-Transit Payment Matching {#subsect_164185356572}

In-transit payments are non-posting and aren't eligible for matching using system or user rules. Instead, Intelligent Transaction Matching matches in-transit payments using a built-in rule that isn't visible to you. This rule requires the transaction number and amount of the in-transit payment to match those of the imported bank line. In addition, the imported bank line must be a Payment type.

For more information about in-transit payments, see [In-Transit Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1535398724.html).

To enable the In-Transit Payments feature, see [Enabling the In-Transit Payments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1535467996.html).

### Related Topics

-   [Bank Data Matching and Reconciliation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4842302228.html)
-   [Permissions for Banking Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156289552348.html)
-   [Reconciling Bank and Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_61161354663.html)
-   [Account Reconciliation Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508786400.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

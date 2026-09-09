---
id: "section_N1486610"
type: "section"
title: "Setting Up Automated Intercompany Management"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management"
parent: "chapter_N1486105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html"
anchors: []
sha256: "ff946b7d175047af848848822e6169537fea04cbe2886c96ee5bba9d51600cad"
---

Complete the following steps to begin using the Automated Intercompany Management feature.

For information about how to run intercompany elimination, see [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html).

**Prerequisite:** You must have NetSuite OneWorld.

1.  Create elimination subsidiaries, if needed.
    
    Your NetSuite OneWorld hierarchy can include an elimination subsidiary for each level in the hierarchy. Your subsidiary hierarchy must include one or more elimination subsidiaries under the root subsidiary level before you enable this feature. See [Elimination Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268759.html).
    
2.  Enable the **Automated Intercompany Management** feature. An administrator must go to _Setup > Company > Enable Features_. Click the **Accounting** subtab. Under the Advanced Features section, check the **Automated Intercompany Management** box, and then save.
    
    Warning:
    
    The Automated Intercompany Management feature can't be disabled after it is enabled. This is true even if you have not created any intercompany entities or transactions.
    
    When you enable this feature, NetSuite adds the following fields, accounts, and more:
    
    -   NetSuite adds the system-generated Cumulative Translation Adjustment-Elimination (CTA-E) account to your chart of accounts after a user enters a qualifying transaction. For example, a user must first run the elimination process so that NetSuite creates an elimination journal entry that uses this account. See [Cumulative Translation Adjustment-Elimination (CTA-E)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498539.html).
        
    -   NetSuite adds the **Eliminate Intercompany Transactions** task as the last task in the Period Close Checklist.
        
    -   An **Eliminate** box displays for journal lines on standard and advanced intercompany journal entries.
        
        Note:
        
        You can use journal entries rather than advanced intercompany journal entries to record intercompany transactions. However, you must customize the standard journal entry form to display the **Eliminate** box. See [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html).
        
    -   NetSuite creates the Standard Intercompany Vendor Form and the Standard Intercompany Customer Form records. These records include the **Represents Subsidiary** field, which doesn't display on the standard vendor and customer records.
        
    -   NetSuite adds the **Intercompany Status** and **Paired Intercompany Transactions** fields to the Sales Order, Purchase Order, Return Authorization, and Vendor Return Authorization pages.
        
    -   NetSuite adds the **Eliminate Intercompany Transactions** box to the Account record.
        
3.  Create intercompany accounts. See [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html).
    
4.  If your account meets the prerequisites, NetSuite can automatically generate and maintain intercompany entities to represent all non-elimination subsidiaries. See [Representing Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159067444188.html).
    
    If your account doesn't meet the prerequisites, you can continue to create intercompany customers and vendors that represent your non-elimination subsidiaries. See [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html).
    
5.  Review the guidelines for inventory items for intercompany transfers. See [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html).
    
6.  For arm's length intercompany inventory transfers, verify that the **Use Item Cost as Transfer Cost** preference is not enabled. Go to _Setup > Accounting > Preferences >Accounting Preferences_ . Click the **Order Management** subtab. Under the Transfer Orders section, ensure the preference is not enabled.
    
7.  Optionally, enable the Automated Intercompany Drop Ship feature to manage intercompany drop ship orders. An administrator must go to _Setup > Company > Enable Features_. Click the **Accounting** subtab. Under the Advanced Features section, check the **Automated Intercompany Drop Ship** box, and then save. See [Intercompany Inventory Drop Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1493456.html).
    

### Related Topics:

-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)
-   [Creating Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html)
-   [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html)
-   [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html)
-   [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html)
-   [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html)
-   [Intercompany Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549982657.html)
-   [Intercompany Sales and Billing Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492389.html)
-   [Managing Intercompany Inventory Transfers - Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492766.html)
-   [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html)
-   [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html)
-   [Working with Elimination Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502129.html)
-   [Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1486105.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

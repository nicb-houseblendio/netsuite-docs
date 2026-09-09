---
id: "bridgehead_N1321151"
type: "bridgehead"
title: "Setting Initial Renewals Preferences"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Initial Setup Tasks for Contract Renewals > Setting Initial Renewals Preferences"
parent: "section_N1321054"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321151.html"
anchors: []
sha256: "624260cb8c977f6bfda5502ed5c8086e4e2164c327eb48da31d536bc735ede3c"
---

After you've created the zero price item, go to Contract Renewals > Setup > Contract Renewals Preferences. Click Edit to set these preferences:

-   On the **Contract Items Creation** subtab, set these preferences if you want to use a custom saved search to define the list of transactions that will be processed for contract item creation.
    
    -   Check the **Use CI Pending Creation Search** box.
        
    -   In the **Search: CI Pending Creation** field, specify the custom saved search that you want to use for contract item creation. For more information, see [Using a Custom Saved Search for Contract Item Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162002114965.html).
        
    
    Note:
    
    If you don't want to use a custom saved search, keep the **Use CI Pending Creation Search** box cleared. If this box is cleared, the contract item creation script (R03) will use its default search to identify the transactions to be processed for contract item creation.
    
-   On the **Contract Renewals Creation** subtab:
    
    -   Set the **Default Renewal Form ID** field to **Sales Order - Contract Renewals.**
        
    -   In the **Zero Dollar Item** field, select the zero-price item you created in the previous section. See [Creating a Zero Price Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321133.html).
        
    -   In the **Assign to Employee/Default** field, select an employee who has been marked as a sales rep.
        
-   On the **Item 'Renew With' Sync** subtab:
    
    Set the **Contract Item Search** field to **Contract Item Renew With Sync.**
    

For more information about these preferences, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

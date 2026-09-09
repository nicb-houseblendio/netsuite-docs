---
id: "section_N276203"
type: "section"
title: "Logos in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Set up NetSuite OneWorld > Logos in OneWorld"
parent: "section_N268052"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276203.html"
anchors: ["procedure_N276218"]
sha256: "c733132b12679b19c53dfd4c7b7b367cbd786410dc2be6216746a3358947908c"
---

When you set up subsidiaries in OneWorld, you can choose the logo that displays for each subsidiary when viewing pages or printing transactions. Each subsidiary can use an individual logo to distinguish itself from the others.

To use the subsidiary logo and address from the transaction record when you print, use advanced templates. For more information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html). If you print transactions using basic layouts, the logo and address are sourced from the vendor's primary subsidiary.

On each subsidiary record, use the following fields to determine which logos display on pages and which are printed on transactions.

#### To set up subsidiary logos: {#procedure_N276218}

1.  Go to _Setup > Company > Subsidiaries_, click **List**, and then click the **Edit** link for a subsidiary.
    
    -   In the **Subsidiary Logo (Forms)** field, select the logo image for all forms for this subsidiary.
        
        Click **New** to upload a logo. Logos must be in JPG or GIF format.
        
    -   In the **Subsidiary Logo (Pages)** field, select the logo image for all pages for this subsidiary.
        
        Click **New** to upload a logo. Logos must be in JPG or GIF format.
        
2.  Go to _Setup > Company > Setup Tasks > Company Information_.
    
3.  Check the **Display Logo Internally** box to display the logo selected in the **Subsidiary Logo (Pages)** field when someone logs in to an internal center. The logo shows on all pages of your NetSuite account next to the Oracle | NetSuite logo.
    
    External centers in your NetSuite account are the Partner Center, Vendor Center, and Customer Center. These external centers display the logo selected in the **Company Logo (Pages)** field. All other internal centers display the logo selected at **Subsidiary Logo (Pages)** when you enable the preference to display the logo (Company Information page).
    
4.  Go to _Home > Set Preferences_.
    
5.  Click the **Analytics** subtab to set preferences that display the subsidiary logo on reports you view or print.
    
    Check **Print Company Logo** and **Display Report Title on Screen**. The logo selected in the **Subsidiary Logo (Forms)** field displays on reports you view or print.
    

If a subsidiary doesn't have configured logo options, NetSuite checks parent subsidiaries. This check is performed in hierarchical order to find a subsidiary with logo options configured. If no subsidiary has logo settings configured, NetSuite pages display logos based on the company settings. Go to _Setup > Company > Setup Tasks > Company Information_.

### Related Topics

-   [Account Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275342.html)
-   [Payroll Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275739.html)
-   [Inventory Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275901.html)
-   [Multiple Vendors Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276076.html)
-   [Set up NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268052.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

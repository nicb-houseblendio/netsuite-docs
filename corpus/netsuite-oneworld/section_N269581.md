---
id: "section_N269581"
type: "section"
title: "Nexuses and Taxes in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiaries in OneWorld > Nexuses and Taxes in OneWorld"
parent: "section_N268563"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html"
anchors: ["bridgehead_156777721842"]
sha256: "86b0f600bde2982bb30a797eac2e28bedd9fa7264d8d9c649639862805ec1afd"
---

A nexus is a tax jurisdiction. Nexuses are part of the NetSuite Advanced Taxes feature, required for NetSuite OneWorld. Each subsidiary must be associated with at least one nexus. The first nexus is automatically assigned to a subsidiary based on the country entered for the subsidiary's address. A subsidiary can have more than one nexus. A nexus and its related tax items can be shared by multiple subsidiaries.

When you edit a subsidiary record, a Nexuses subtab is available where you can add or remove nexuses. See [Editing Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273122.html).

Important:

For U.S. subsidiaries, a state nexus is required. For Canada subsidiaries, a province nexus is required.

It is best to create and set up taxes for nexuses before you create subsidiary records. You can create a nexus at _Setup > Accounting > Nexuses > New_. See [Creating Tax Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804264.html).

You set up taxes for nexuses at _Setup > Accounting > Taxes > Set Up Taxes_. When you create a subsidiary, if a nexus doesn't exist for the subsidiary's country, it is automatically created when you save the subsidiary record. However, all that is created for the nexus is a name and description. You must still set it up at _Setup > Accounting > Taxes > Set Up Taxes_.

## Tax Features for Nexuses {#bridgehead_156777721842}

You should understand and set up the following tax features and items to set up tax nexuses:

-   **Advanced Taxes Feature** - This feature provides management of taxes for multiple tax jurisdictions and must be enabled in NetSuite OneWorld. See [Enabling Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803739.html).
    
-   **Tax Agency Vendors** - These vendors represent taxing authorities to whom you pay collected taxes. The system automatically creates a tax agency vendor when you create a tax nexus. See [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html).
    
    Multiple subsidiaries can pay taxes to the same tax agency. When a new subsidiary shares a tax nexus with an existing subsidiary, the system creates a copy of the preferred tax vendor for that nexus. The copy of the preferred tax vendor gets associated with the new subsidiary. The copy is necessary because you can't share a vendor tax agency with multiple subsidiaries. You can, however, share non-tax agency vendors with multiple subsidiaries. For more information, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
-   **Tax Control Accounts** - These are Other Current Liability Accounts that you can set up in your general ledger. These accounts post and track tax collection and payments. See [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).
    
-   **Tax Types** - These types provide categories used to link each tax code or tax group to a tax control account. Available tax types depend upon the country selected for the tax code. See [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html).
    
-   **Tax Codes and Tax Groups** - A tax code represents a tax collected from customers in a specific geographic area. It is paid on their behalf to a taxing authority. The amount collected is based on a specific percentage rate. You can create tax groups that combine taxes for all tax jurisdictions relevant to a transaction. See [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html) and [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html).
    
-   **Tax Schedules** - Tax schedules permit different calculations of taxes on items, for different nexuses. When you enable the Advanced Taxes feature, the system creates tax schedules for each tax code. See [Creating Tax Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804737.html).
    
-   **Tax Reporting Periods** - (Editions other than US and Canada) You can set up these periods to track tax reporting separately from accounting periods. In NetSuite OneWorld, the same tax reporting periods apply across all subsidiaries that use the feature. See [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html).
    

Note:

Available tax items and features vary for different NetSuite editions. See [NetSuite Editions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N270055.html).

### Related Topics

-   [Elimination Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268759.html)
-   [Subsidiary Hierarchy Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269084.html)
-   [Multiple Currencies in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269257.html)
-   [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1983547"
type: "section"
title: "Singapore Tax Setup"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Singapore Tax Setup"
parent: "chapter_N1981261"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html"
anchors: ["bridgehead_N1983610", "procedure_N1983662", "procedure_1524528893", "procedure_1524528898", "bridgehead_N1983725", "procedure_N1983756"]
sha256: "90d91fba826a8bab46f3c54e9a4c1452f6a0360916115bac6236ecdf7e9672d3"
---

If you are going to use the NetSuite Tax Audit Files, you must set up additional tax control accounts, tax types, and tax codes. Read the following topics:

-   [Singapore Tax Control Accounts](#bridgehead_N1983610)
    
-   [Singapore Tax Types](#bridgehead_N1983725)
    
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
    
-   [Singapore Customer Accounting Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html#bridgehead_1524617492)
    

## Singapore Tax Control Accounts {#bridgehead_N1983610}

The following tax control accounts are already provided in your NetSuite account:

-   GST on Sales
    
-   GST on Purchases
    
-   GST Liability
    

You must create the following new tax control accounts:

-   GST Input Disallowed
    
-   Deferred GST on Sales SG
    
-   Deferred GST on Purchase SG
    

#### To create the GST Input Disallowed tax control account: {#procedure_N1983662}

1.  Go to Setup > Accounting > Tax Control Accounts > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Provide the following information.
    
    -   **Name** : GST Input Disallowed
        
    -   **Tax Account Type** : Purchase
        
4.  Click **Save**.
    

#### To create the Deferred GST on Sales SG tax control account: {#procedure_1524528893}

1.  Go to Setup > Accounting > Tax Control Accounts > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Provide the following information.
    
    -   **Name**: Deferred GST on Sales SG
        
    -   **Tax Account Type**: Sales
        
4.  Click **Save**.
    

#### To create the Deferred GST on Purchase SG tax control account: {#procedure_1524528898}

1.  Go to Setup > Accounting > Tax Control Accounts > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Provide the following information.
    
    -   **Name**: Deferred GST on Purchase SG
        
    -   **Tax Account Type**: Purchase
        
4.  Click **Save**.
    

## Singapore Tax Types {#bridgehead_N1983725}

The following tax types are required:

-   GST\_SG (This tax type is already available in your NetSuite account.)
    
-   Disallowed GST\_SG (You must create this new tax type.)
    

#### To create the Disallowed GST\_SG tax type: {#procedure_N1983756}

1.  Go to Setup > Accounting > Taxes > Tax Types > New.
    
2.  If you are using a OneWorld account, select the **Singapore** tax nexus.
    
3.  Provide the following information:
    
    -   **Name** : Disallowed GST\_SG
        
    -   **Asset/Purchase Tax Account** : GST Input Disallowed
        
4.  Click **Save**.
    

### Related Topics

-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

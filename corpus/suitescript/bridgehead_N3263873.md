---
id: "bridgehead_N3263873"
type: "bridgehead"
title: "Tax Setup"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Preference Names and IDs > Tax Setup"
parent: "chapter_N3251359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263873.html"
anchors: []
sha256: "e8a59650d448945658808de244ed3e4d97fe3bc2ef54b3d546f7eea908cf507c"
---

The internal ID for the Set Up Taxes page is **taxpreferences**. All preference internal IDs are case-insensitive.

Preference IDs for fields on this page vary according to the country of the nexus. Field internal IDs are suffixed with the nexus country code. The format for these preferences is <field internal id><nexus country code>. Be aware that different fields are available for different nexuses.

The table below shows some scriptable tax preference fields for a US nexus. Fields are suffixed with **us**, for the US nexus. This table is provided for example purposes.

| Preference UI Label | Preference Internal ID |
| --- | --- |
| Customers Default to Taxable | defaulttaxableus |
| Charge out of District Sales Taxes | chargeoutofdistrictus |
| Per-Line Taxes on Transactions | perlinetaxesus |
| Charge Sales Tax on Store Orders | storeordertaxationus |
| Enable Tax Lookup on Sales Transactions | enabletaxlookupus |

Field IDs in your account may be suffixed with a different nexus country code. And different fields may be available. You may be able to look up field IDs in the user interface, by going to _Setup > Accounting > Set Up Taxes_, and clicking on a nexus.

-   To make field IDs available, go to _Home > Set Preferences_ and ensure that the Show Internal IDs box is checked on the General subtab, Defaults area.
    
-   Find the field in the NetSuite user interface and click the field label to display the field level help text. The field ID is displayed in the popup.
    

### Related Topics

-   [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html)
-   [General Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3251492.html)
-   [Company Information Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3253690.html)
-   [User Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3254790.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3258805.html)
-   [Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263666.html)
-   [Manufacturing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_160795960465.html)
-   [Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4695736720.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

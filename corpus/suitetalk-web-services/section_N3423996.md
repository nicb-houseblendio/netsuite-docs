---
id: "section_N3423996"
type: "section"
title: "Setting the Internal ID Preference"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Preferences > Setting the Internal ID Preference"
parent: "chapter_N3422061"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423996.html"
anchors: []
sha256: "9997e16c9041b713b4e7d38297c784d9606dfb4ee9c2bedb7850b63c9ac1f0c0"
---

NetSuite can be configured to show internal ID values in the UI. This behavior can be useful during development of your SOAP web services integration. Displaying internal IDs helps verify that SOAP requests target the correct records.

Note:

The Show Internal IDs field requires one of the following features to be enabled on your account: Client SuiteScript, Server SuiteScript, SuiteScript Server Pages, SuiteFlow, or Web Services (on the SuiteCloud subtab) or Advanced Site Customization or SuiteCommerce Advanced (on the Web Presence tab). For more information, see [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html).

#### To display internal ID values:

1.  Go to _Home > Set Preferences_. The **General** subtab is displayed by default.
    
2.  In the **Defaults** section, click **Show Internal IDs**.
    

Enabling this preference adds Internal ID to most list views. For example, when you go to _List > Relationships > Customers_, the second column is Internal ID.

Changes to this preference affect only the current user.

Note:

You can also find the internal ID in the record's URL. For instance, a record's URL might look like this: https://webservices.netsuite.com/app/common/entity/custjob.nl?id=272. In this example, the internal ID is 272.

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3422061.html)
-   [Company-Wide Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3422217.html)
-   [One-Time Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423112.html)
-   [Caching Behavior in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512050046.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

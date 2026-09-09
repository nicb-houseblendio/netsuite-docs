---
id: "section_N672926"
type: "section"
title: "Mass Updates of Global Subscription Status"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Mass Updates > Mass Updates of Global Subscription Status"
parent: "article_1103335211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N672926.html"
anchors: ["procedure_N673155"]
sha256: "9cdff537f13eb0f602eebc3d712c4dd1ec66f760aed3e7537964cfcdeafefbce"
---

You can use the Global Subscription Status field to help manage marketing email campaigns. This field, which has replaced the formerly used Unsubscribe field, is available for mass updates on Company, Contact, Customer (including Leads and Prospects), Partner, and Vendor records. Be aware that mass updates can only set the value of this field to Soft Opt-In or Soft Opt-Out. Only users themselves can change their status to Confirmed Opt-In or Confirmed Opt-Out. The following mass updates are permitted:

| If Current Status Is: | Mass Update Can Set Status to: |
| --- | --- |
| Confirmed Opt-In | **Soft Opt-In or Soft Opt-Out** |
| Soft Opt-In | **Soft Opt-Out** |
| Soft Opt-Out | Soft Opt-In |
| Confirmed Opt-Out | (NO MASS UPDATE AVAILABLE) |

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

#### To perform a mass update of global subscription status: {#procedure_N673155}

1.  Go to Lists > Mass Update > Mass Updates.
    
2.  Expand General Updates, then click Company, Customer, Partner, or Vendor.
    
3.  Set criteria for the users you want to update.
    
4.  On the **Mass Update Fields** subtab, check the **Global Subscription Status** box.
    
5.  Select the status you want to set: Soft Opt-In or Soft Opt-Out
    
    All records that match the criteria you have set and that are permitted to be changed through mass updates will be set to the selected status.
    
6.  Click Save.
    

### Related Topics

-   [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html)
-   [Defining a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N667342.html)
-   [Entering Formulas for a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668091.html)
-   [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html)
-   [Translations for Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668849.html)
-   [Example Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669099.html)
-   [Available Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669340.html)
-   [Performing Mass Deletes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098351672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

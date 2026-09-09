---
id: "section_N3422217"
type: "section"
title: "Company-Wide Preferences"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Preferences > Company-Wide Preferences"
parent: "chapter_N3422061"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3422217.html"
anchors: ["bridgehead_4169324605", "bridgehead_4169972284", "bridgehead_4394647795", "bridgehead_4169243447", "bridgehead_4169319604"]
sha256: "972a59d66ce9a8c10726d1e6b09f0541d99151eceb590561d375e3615d9078b5"
---

You can set company-wide preferences for SOAP web services. These changes apply to all users.

You can set these preferences at _Setup > Integration > SOAP Web Services Preferences_.

Some of these preferences can be overridden when you send individual SOAP web services requests. For details, see [One-Time Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423112.html). Note that more preferences are available for individual requests.

Note:

The SOAP Web Services Preferences page shows whether concurrency governance is enabled and the available limit for your account. For information about web services and RESTlet concurrency governance, see [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html)

Company-wide preferences include:

-   [Disable Mandatory Custom Field Validation](#bridgehead_4169324605)
    
-   [Run Server SuiteScript and Trigger Workflows](#bridgehead_4169972284)
    
-   [Require Approval During Auto-Installation of Integration](#bridgehead_4394647795)
    
-   [Search Page Size](#bridgehead_4169243447)
    
-   [Treat Warnings as Errors](#bridgehead_4169319604)
    

## Disable Mandatory Custom Field Validation {#bridgehead_4169324605}

This preference impacts mandatory custom fields in the UI. Setting this to true makes the fields are **not** required during SOAP web services requests. Setting this to false makes the fields required. Omitting required values returns a USER\_ERROR with instructions to provide value for the field.

When deciding whether to enable this preference, consider if the provided data comes from a system that equivalent fields to the custom field.

This preference can be overridden at the request level. For details, see [disableMandatoryCustomFieldValidation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_4170224592).

## Run Server SuiteScript and Trigger Workflows {#bridgehead_4169972284}

This preference applies company-wide. However, you can overwrite this preference in each SOAP web services request. For details, see [Request-Level Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html).

This preference enables server SuiteScripts and triggers workflows and is selected by default. If this preference is not selected, all SuiteScript scripts and workflows are disabled.

Disabling this option has two effects:

-   Disable server SuiteScripts that otherwise would have been triggered by SOAP web services requests.
    
-   Disable workflows that otherwise would have been triggered by SOAP web services requests.
    

When importing historical data into NetSuite, consider disabling this option for faster processing and block executions of additional logic performed automatically by executed scripts and workflows. For live data sync or partner apps like Outlook Sync, use the default option, Server. In other words, consider enabling server SuiteScript to run your business logic for integrated apps. Note that enabling server SuiteScript may negatively affect performance.

Important:

To ensure that your business logic is fully executed, always use the default option, Server. Additionally, changing the default option can potentially break your working integration. Avoid this unless you're an advanced SOAP web services user.

## Require Approval During Auto-Installation of Integration {#bridgehead_4394647795}

Auto-installation creates an integration record in your NetSuite account automatically. For instance, a partner may provide you with an updated version of an application. This update may include a new application ID created by using an integration record. The first time you send a request using this application, a new integration record is created in your account.

The **Require Approval during Auto-Installation of Integration** determines if the new record is enabled automatically. If set to false, the State field on the new application is set to Enabled, and requests are allowed. If set to true, the Set field on the new integration record is set to Waiting for Approval. You must then manually set the state to Enabled. Until enabled, all requests from the application are blocked.

## Search Page Size {#bridgehead_4169243447}

The Search Page Size preference controls the number of returned search results. It applies to both synchronous and asynchronous searches. Company-wide, valid values range from 5 to 1,000. The default value is 1,000.

You can override this preference for individual searches. For individual searches, asynchronous searches have a higher maximum than the company-wide limit. For more details, see [pageSize](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423764).

## Treat Warnings as Errors {#bridgehead_4169319604}

Enabling this preference treats warning messages generated by NetSuite as errors that cause an exeption, rejecting the request. For more information about the difference between errors and warnings, see [SOAP Web Services Warnings, Errors, and Faults](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536574.html).

This preference can be overridden per request. For details, see [warningAsError](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_4170211767).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3422061.html)
-   [One-Time Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423112.html)
-   [Setting the Internal ID Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3423996.html)
-   [Caching Behavior in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512050046.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

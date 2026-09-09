---
id: "section_N3478008"
type: "section"
title: "SOAP Web Services Standard Operations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > SOAP Web Services Standard Operations"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html"
anchors: []
sha256: "b065df30cef078ac3ab1ea23a016fa1d7c7438e18f93a3b965f33b472c151022"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The following operations are supported in SOAP web services. They are organized in alphabetical order:

| Operation / API | Summary |
| --- | --- |
| [add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) **/** [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | Use to add one or more records into the system. The system returns a NetSuite identifier (internalId) that is unique for each record created within a record type. |
| [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | Use to attach or detach another record or file to/from another record. |
| [changeEmail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3484955.html) | Use to change the email address for the account. |
| [changePassword](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3485424.html) | Use to change the password for the account. |
| [checkAsyncStatus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3485891.html) | Use to check the status of an asynchronous SOAP web services submission. |
| [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) **/** [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | Use to delete one or more records in the system. The records to be deleted are identified by either the internal or external ID and the record type. |
| [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) / [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | Use to query the system for one or more records. You must provide either the internal or external ID and the record type for each query item. |
| [getAccountGovernanceInfo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158142198604.html) | Use to retrieve the account concurrency limit and the unallocated concurrency limit. |
| [getAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html) | Use to return a list of records that do not have a search interface. |
| [getAsyncResult](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489563.html) | Use to retrieve the results of an asynchronous SOAP web services submission. |
| [getBudgetExchangeRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489718.html) | Use to get and filter all data related to the Budget Exchange Rates table. |
| [getConsolidatedExchangeRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3491080.html) | Use to get and filter all data related to the Consolidated Exchange Rates table. Important: The exposure of the consolidated exchange rate record prompted the removal of the getConsolidatedExchangeRate operation from the 2017.1 endpoint. You can still use the getConsolidatedExchangeRate operation on earlier endpoints. For more information about working with consolidated exchange rates on endpoints starting from 2017.1, see [Consolidated Exchange Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4847555414.html). |
| [getCurrencyRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3492280.html) | Use to get currency exchange rates from the Currency Exchange Rate table. |
| [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | Use to retrieve the internalIds, externalIds, and scriptIds of all custom objects of a specified type. |
| [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) | Use for dynamic discovery of the correct URL for SOAP web services requests. Important: All SOAP web services integrations **must** include logic to dynamically discover the correct URL. Important: As of the 2019.1 SOAP web services endpoint, you must use account-specific domains with SOAP web services. You can use the SOAP getDataCenterUrls operation to obtain the correct domain. Or, go to _Setup > Company > Setup Tasks >Company Information_ in the NetSuite UI. Your domains are listed on the Company URLs subtab. |
| [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | Use to retrieve a list of deleted records of a particular type during a specified period. |
| [getIntegrationGovernanceInfo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158142272877.html) | Use to retrieve the concurrency limit for the specific integration and the limitType. With this information the integration can identify how many concurrent requests it can send. |
| [getItemAvailability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3498308.html) | Use to retrieve the inventory availability for a specific list of items. |
| [getPostingTransactionSummary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3500304.html) | Use to retrieve a summary of the actual data in an account. |
| [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | Use to retrieve a list of existing saved searches for each record type. Specify the search record type to get a list of record references of the saved search. |
| [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | Use to retrieve valid values for a particular recordRef field where the referenced record type is not yet exposed in the SOAP web services API or when the logged in role does not have permission to the instances of the record type. Important: The getSelectValue operation is not supported for record types which can't be created with SuiteScript, for example Inventory Number or Period End Journal Entry. |
| [getServerTime](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508018.html) | Use to get server time, resulting in more accurate and reliable sync'ing of data than using using local client time. The client will use the time from server to determine if the record has changed since the last synchronization. |
| [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | Use to emulate the UI workflow by pre-populating fields on transaction line items with values from a related record. The initializeList operation can be used to run batch processes to retrieve initialized records. |
| [mapSso](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3513702.html) | Warning: As of the NetSuite 2021.1 release, the mapSso operation is no longer available. This affects all endpoints, and even though the SOAP schema remains for older endpoints, the method is not working. For SOAP web services you must use token-based authentication instead. For more information, see [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html). |
| [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | Use to search for a set of records based on specific search criteria. This operation supports pagination, so that large result sets can be retrieved in smaller sets. For more information about how to control pagination, refer to [SOAP Web Services Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3422061.html). |
| [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | Use to retrieve search results for users who send requests to NetSuite by providing request-level credentials, rather than by invoking login. |
| [ssoLogin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3526370.html) | Warning: As of the NetSuite 2021.1 release, the ssoLogin operation is no longer available. This affects all endpoints, and even though the SOAP schema remains for older endpoints, the method is not working. For SOAP web services you must use token-based authentication instead. For more information, see [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html). |
| [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) **/** [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | Use to update one or more existing records in the system by providing new values for the fields to be updated for each record. The records to be updated are identified by either the internal or external ID and the record type. |
| [updateInviteeStatus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3531056.html) / [updateInviteeStatusList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3531763.html) | Allows event invitees to accept or decline NetSuite events. After invitees have responded to the event, the Event record is updated with their response. |
| [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) / [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html) | Use to add new records and update existing records in a single operation. Records are identified by external ID and record type. If a record of the specified type with a matching external ID exists in the system, it is updated. If it does not exist, a new record is created. |

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3448861"
type: "section"
title: "Enabling Web Services Concurrent Users with SuiteCloud Plus"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Platform Features > Enabling Web Services Concurrent Users with SuiteCloud Plus"
parent: "chapter_N3448700"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448861.html"
anchors: ["procedure_N3448986"]
sha256: "f9812018f844f7ea9e34ce29bb779584e7f467342eab984087d9e6375a171d35"
---

Your account must have the web services feature enabled before you can assign a user to be a web services concurrent user. See [Enabling the SOAP Web Services Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419926.html) for details.

Any user can be designated as concurrent web services user if one or more SuiteCloud Plus license has been purchased.

Generally, you can purchase one SuiteCloud Plus license per NetSuite account. Contact your sales representative to discuss any need for additional licenses.

Web services and RESTlet concurrency is also governed per account. The new account governance limit applies to the combined total of web services and RESTlet requests. Due to this change, if a designated user makes 10 concurrent web services requests, the number of successful requests depends on other web services or REST requests that are being processed. Each SuiteCloud Plus license increases the account base limit for concurrent web services requests by 10. The account base limit depends on your service tier.

Note:

The account limit is lenient, and it is possible to temporarily exceed the limit.

Important:

If you use token-based authentication with SOAP web services, a single user can send concurrent requests up to the account limit. For more information, see [SOAP Web Services Governance for Token-Based Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4502013915.html).

For more information about account base limits and the concurrency governance, see [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html).

Note:

SuiteCloud Plus provides other benefits. It increases the number of scheduled script processors. For details, see [SuiteCloud Processors Supported Task Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505167691.html). It allows the use of multi-threading for CSV import jobs and increases the number of import jobs that can be run in parallel. For details, see [Use Multiple Threads and Multiple Queues to Run CSV Import Jobs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347015.html). For a summary of SuiteCloud Plus capabilities, see [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html).

#### To designate a user as a concurrent web services user: {#procedure_N3448986}

1.  Open the employee record.
    
2.  Click the **Access** subtab.
    
3.  Check the **Concurrent Web Services User** box.
    
4.  Click **Save**.
    

### Related Topics

-   [Platform Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3448700.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [Operations and Their Internal ID Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3449174.html)
-   [Using SOAP web services to Send Data from a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4488980213.html)
-   [Searching for SOAP Web Services Log Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738049812.html)
-   [SOAP Web Services Operations Search Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738050787.html)
-   [SOAP Web Services Record Processing Search Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738051114.html)
-   [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N3950559"
type: "section"
title: "SuiteTalk Web Services Integration"
branch: "release-notes"
category: "what-s-new"
breadcrumb: "What's New > Release Notes > NetSuite 2026.2 Release Notes > SuiteTalk Web Services Integration"
parent: "article_72152418635"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3950559.html"
anchors: ["subsect_57132844971", "subsect_0525013110"]
sha256: "14d9fcf9ed378e029911fb414d00a616077e0d5395f3d7197d82af7a4780ef72"
---

NetSuite 2026.2 includes the following enhancements to web services features:

-   [Support for Bound Parameters in REST SuiteQL Search](#subsect_57132844971)
    
-   [Support for Sequential Processing of Batch Operations in REST Web Services](#subsect_0525013110)
    

## Support for Bound Parameters in REST SuiteQL Search {#subsect_57132844971}

You can now use anonymous bound parameters when performing SuiteQL search operations through REST web services.

A bound parameter is a placeholder in a SuiteQL query whose value is supplied separately at execution time. Using bound parameters, you can submit queries containing user input in a secure way.

REST web services support using one or multiple bound parameters in a request.

The following example shows a SuiteQL query in REST that uses two bound parameters:

            `POST {{REST_SERVICES}}/query/v1/suiteql  Prefer: transient  {     "q": "SELECT * FROM item WHERE id BETWEEN ? AND ?",     "params": [ "-7", "0"] }` 
          

For more information about using SuiteQL queries in REST, see [Executing SuiteQL Queries Through REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157909186990.html).

## Support for Sequential Processing of Batch Operations in REST Web Services {#subsect_0525013110}

Sequential batch operations are useful for cases that involve record dependencies. Sequential batch operations run in the order specified in the REST request. This approach is useful in the following cases:

-   For parent-child record creation, when a parent record and its child records are created in a single batch operation, and the child records reference the parent record's external ID
    
-   For processing inventory adjustments, transfers, or builds where the order of operations directly impacts inventory availability and allocation
    

In general, batch operations reduce the number of network requests by processing multiple records in one request, minimizing latency and server load. This approach is useful for large-scale data imports, updates, and deletions, because it improves system performance and user experience. Batch operations in REST web services run asynchronously.

For more information, see [Batch Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0127092747.html).

For information about every available operation in REST web services, see [SOAP Web Services and REST Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_3101500486.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

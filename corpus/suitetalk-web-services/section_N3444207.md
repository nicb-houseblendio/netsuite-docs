---
id: "section_N3444207"
type: "section"
title: "Synchronous Versus Asynchronous Request Processing"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Processing > Synchronous Versus Asynchronous Request Processing"
parent: "chapter_N3444088"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html"
anchors: []
sha256: "b29968a2973ad28d118f63e16593f78b7ee6f9f299c641267506985fc8da9ebb"
---

SOAP web services requests can be processed synchronously or asynchronously.

With synchronous requests, your client application sends a request to NetSuite, and the client waits until the request is processed and a response is returned. That is, the application does not proceed with other work until receiving the response.

With asynchronous requests, your client application sends a request to SOAP web services, where it is placed in a processing queue and handled asynchronously with other requests. Your client application does not wait for a response but goes on to other work. After a job is submitted, a job Id is returned in the SOAP web services response. Your client application can then check on the status and result of the request by referencing the job Id.

Asynchronous processing may be advantageous in the following situations:

-   If you expect your connection to NetSuite to be slow or unstable.
    
-   If your job is large, and its processing can be postponed until off-peak hours.
    

Be aware that asynchronous responses may not be returned immediately. Before committing to using asynchronous operations, you should consider this factor and decide whether it fits in with your business logic.

### Related Topics

-   [Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770809638.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [Synchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444684.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

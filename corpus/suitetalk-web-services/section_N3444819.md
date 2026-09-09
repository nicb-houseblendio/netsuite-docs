---
id: "section_N3444819"
type: "section"
title: "Using the SOAP Web Services Usage Log"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Processing > Synchronous Request Processing > Using the SOAP Web Services Usage Log"
parent: "section_N3444684"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444819.html"
anchors: []
sha256: "6b02d13ef7b6beb8f38228fedf2501060abde6b389ea4b990eda81499c079097"
---

Use the SOAP Web Services Usage Log to monitor synchronous requests. This page can be accessed at _Setup > Integration > SOAP Web Services Usage Log_.

Only administrators can access the SOAP Web Services Usage Log. Assigning the SOAP Web Services permission to a role does not provide access to this log. Access is provided to administrators only because access to this log could allow users to see data they do not have permission to view.

The SOAP Web Services Usage Log allows users to filter their SOAP web services requests by specified date and time periods, record type, and action (operation). The SOAP requests and responses for each job are accessible in the Request and Response columns. Both in production and sandbox environments, requests and responses are accessible for **21 days**.

Note:

In case of heavy SOAP web services activity, the logs might be purged earlier than 21 days.

Results can be filtered down to the minute. The results returned provide second-level granularity.

Note that lengthy requests and responses are not saved by the system and therefore are not available for your review. The system imposes the following limits:

-   The system does not save requests that are larger than 100 MB.
    
-   The system does not save responses that are larger than 10 MB.
    

For each request, the log includes details such as the following:

-   The request job ID.
    
-   The date and time that the request was made.
    
-   The duration of the request.
    
-   Information about the requests that were rejected due to a violation of the concurrency governance.
    
-   The integration record used for the request.
    
-   The type of action used in the request.
    
-   The record type that was the subject of the request.
    
-   The email address of the user who sent the request.
    
-   The status of the request.
    
-   The number of records included in the request.
    
-   The number of request records that have finished.
    
-   The number of request records that failed.
    
-   The number of records returned in the request's query.
    
-   Links to the SOAP request and response.
    

Note:

The SOAP Web Services Usage Log does not show asynchronous requests. For details, see [Monitoring Asynchronous Jobs from the UI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445354.html).

### Related Topics

-   [Synchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444684.html)
-   [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html)
-   [Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770809638.html)
-   [Creating Integration Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445008.html)
-   [Handling of Lengthy Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4078474279.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N2535212"
type: "section"
title: "status"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > status"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2535212.html"
anchors: []
sha256: "af4aaa1d4e25111050ed105e13bb8dcef762a7460f61d9a0cac3bd5f8f39ffaf"
---

Each JSON object returned by a shopping function has an embedded status object that provides business logic validation of the web store order. The caller of a shopping function, in addition to checking the request status, should also check the status object to determine whether the object can be submitted to the backend and whether there are messages to display.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| code | string | Code of the status Following values are supported:
-   error = object contains error
-   incomplete = object is not complete, so cannot be handled by backend
-   ready = object is complete and ready to be submitted to backend
-   success = object successfully processed by backend

 |  |  |
| fieldstatuses | array of status objects | Status for object fields |  |  |
| messages | array of [message](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2524192.html) objects | Status messages |  |  |
| reasoncode | string | Code of possible reason for the current status |  |  |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

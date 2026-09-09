---
id: "chapter_N3269064"
type: "chapter"
title: "Task IDs"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Task IDs"
parent: "chapter_1494647249"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3269064.html"
anchors: []
sha256: "d793ff4fae1df0c8841a66a77934f1851a9dca70d246b14cfcfd9ec1ce3449a6"
---

Task IDs identify NetSuite pages. Each NetSuite page has a unique task ID.

You can reference task IDs when using the [url.resolveTaskLink(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358672296.html) and [redirect.toTaskLink(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4424988740.html) methods.

#### To find a task ID for a NetSuite page:

1.  Right-click in the NetSuite page, and select **View Page Source** from the context menu. Note that the exact command varies by browser.
    
2.  Press Ctrl+F to open the search popup, and enter **taskId** in the search field. Note that the search mechanism varies by browser.
    
3.  Press Enter, use the down arrow, or click **Find Next** until you reach the occurance of `taskId` as part of a line of code. For example: `"taskId":"LIST_EMPLOYEE_RECORD"` is included on a line of code on the Employees page.
    

### Related Topics

-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)
-   [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html)
-   [Feature Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3247851.html)
-   [Preference Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3251359.html)
-   [Button IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3265696.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

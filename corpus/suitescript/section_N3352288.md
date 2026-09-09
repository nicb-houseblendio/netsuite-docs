---
id: "section_N3352288"
type: "section"
title: "Search Result Limits"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Governance and Limits > Search Result Limits"
parent: "chapter_N3350651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352288.html"
anchors: []
sha256: "8a483714ac73ef140563abee4eb5b64888020146e2d3d76b16a03ac3efdd9d25"
---

-   Search results are limited to 1,000 records when you execute SuiteScript searches using the [N/search Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345764122.html). For information about working with SuiteScript searches in NetSuite, see the help topic [N/search Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345764122.html).
    
-   If you load a saved search using [search.load(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345775360.html), and then call [Search.run()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_452292724609.html) to return a result set of [search.ResultSet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345767679.html) objects, you may get up to 4,000 results returned. For more information, see the help topic [ResultSet.each(callback)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_457160888671.html).
    
-   Text columns in search results have a 4000-byte limit, or about 4000 characters in English. Using intricate character sets can lower this limit, since they need more bytes per character.
    

### Related Topics

-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html)
-   [Script Type Usage Unit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html)
-   [Monitoring Script Usage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html)
-   [Governance on Script Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html)
-   [Script Execution Time Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161591009480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

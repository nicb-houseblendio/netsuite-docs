---
id: "chapter_N3350651"
type: "chapter"
title: "SuiteScript Governance and Limits"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Governance and Limits"
parent: "book_14946590423"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html"
anchors: []
sha256: "655eaee4254187b5597aaafa27b9c7362a507a00bec4182159e1b33ceb0ebe1d"
---

NetSuite uses a SuiteScript governance model to optimize performance, based on usage units. If the number of allowable usage units is exceeded, script execution is terminated.

Usage units are tracked in two ways: by script type and by API. Each script type and each SuiteScript API has a set number of usage units.

In map/reduce scripts, keys are limited to 3,000 characters (specifically, in mapContext or reduceContext objects). You'll also see error messages if a key is longer than 3,000 characters or a value is larger than 10 MB. Keys longer than 3,000 characters will return the error KEY\_LENGTH\_IS\_OVER\_3000\_BYTES. Values larger than 10 MB will return the error VALUE\_LENGTH\_IS\_OVER\_10\_MB.

When using mapContext.write() or reduceContext.write(), keep your key strings under 3,000 characters and value strings under 10 MB. Also, consider the potential length of any dynamically generated strings, which might exceed these limits. It's also a good idea to avoid using keys to pass data - use values instead.

You can find governance limits for each SuiteScript 2.1 API in their respective method topics. Methods are organized by modules, and all modules are listed in the help topic [SuiteScript 2.1 Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4220488571.html). Also see [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html).

Important:

SuiteScript thresholds are based on the volume of activity that a company's users can manually generate. However, automated functions that generate excessive levels of activity may trigger metering of script execution as referenced in the [NetSuite Main Terms of Service](https://www.oracle.com/corporate/contracts/cloud-services/netsuite/) (TOS).

See the following help topics for more information:

-   [Script Type Usage Unit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html)
    
-   [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html)
    
-   [Monitoring Script Usage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html)
    
-   [Governance on Script Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html)
    

Governance limits are also enforced on certain aspects of script execution. When you run a search using the N/search module, the number of search results you receive is limited. There are also limits on how long a script can run, based on the script type. See the following help topics to learn about these limits:

-   [Search Result Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352288.html)
    
-   [Script Execution Time Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161591009480.html)
    

### Related Topics

-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [Setting Up Your SuiteScript Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2903520.html)
-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html)
-   [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html)
-   [SuiteScript Monitoring, Auditing, and Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494642209.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

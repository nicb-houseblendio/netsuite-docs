---
id: "section_N3014224"
type: "section"
title: "SuiteScript Debugger Overview"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Debugger > SuiteScript Debugger Overview"
parent: "chapter_N3014215"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3014224.html"
anchors: []
sha256: "8deb19551cf70af5a7eb85eaf592775baa5f74bc35ff24fbbda2882d77df991c"
---

SuiteScript offers a script debugger for SuiteScript 1.0, SuiteScript 2.0, and SuiteScript 2.1 server scripts, core plug-in implementations, and on-demand debugging.

Important:

You can't use the SuiteScript Debugger to debug SuiteScript 2.1 scripts. You can still test critical parts of your script in the SuiteScript Debugger as a SuiteScript 2.0 script before you run the script as a SuiteScript 2.1 script. For more information about SuiteScript 2.1, see [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html).

You can debug SuiteScript 2.1 scripts with the new 2.1 Script Debugger. This debugger uses Chrome DevTools directly within NetSuite so you can debug scripts much like you would in Google Chrome.

You can't debug client scripts with the SuiteScript Debugger, but you can use your browser's tools. To debug client scripts, use the Chrome DevTools for Chrome and the Firebug debugger for Firefox. For more information, see your browser's documentation.

Note:

Currently, only one script can be debugged at a time in a given debug session, regardless of the version of the script.

The following table shows which server script types are supported in each debugger. On-demand debugging is also supported. Client scripts are debugged on the client browser.

| Script Type | Script Debugger (SuiteScript 1.0) | Script Debugger (SuiteScript 2.0) | 2.1 Script Debugger (SuiteScript 2.1) |
| --- | --- | --- | --- |
| Bundle Installation | ✓ | ✓ | \- |
| Map/Reduce | \- | \- | \- |
| Mass Update | ✓ | ✓ | \- |
| Portlet | ✓ | ✓ | \- |
| RESTlet | ✓ | ✓ | \- |
| Scheduled | ✓ | ✓ | ✓ |
| SDF Installation | \- | This script type runs on the client browser. | \- |
| Suitelet | ✓ | ✓ | ✓ |
| User Event | ✓ | ✓ | ✓ |
| Workflow Action | ✓ | ✓ | \- |
| Custom Plug-in | ✓ | ✓ | \- |

The following table shows which custom plug-ins are supported in each debugger. Support for SuiteScript 2.1 scripts will increase in future releases.

| Core Plug-in | Script Debugger (SuiteScript 1.0) | Script Debugger (SuiteScript 2.0) | 2.1 Script Debugger (SuiteScript 2.1) |
| --- | --- | --- | --- |
| Platform Extension | \- | ✓ | Not available |
| GL Plug-in | ✓ | \- |
| Payment Gateway | ✓ | \- |
| Consolidated Rate Adjustor | ✓ | \- |
| Promotions | ✓ | \- |
| Tax Calculation | ✓ | \- |
| Shipping Partners | ✓ | ✓ |
| Email Capture | ✓ | \- |
| Advanced Rev Rec | ✓ | ✓ |
| Bank Connectivity | ✓ | \- |
| Test Plug-in | ✓ | ✓ |

For more information about using each debugger, see the following help topics:

-   [Debugging Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418473843.html)
    
-   [Debugging SuiteScript 1.0 and SuiteScript 2.0 Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418113411.html)
    
-   [Debugging SuiteScript 2.1 Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418115436.html)
    

### Related Topics

-   [Debugging Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418473843.html)
-   [Debugging SuiteScript 1.0 and SuiteScript 2.0 Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418113411.html)
-   [Debugging SuiteScript 2.1 Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418115436.html)
-   [Script Debugger Metering and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3018263.html)
-   [Debugging Client Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157437352479.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

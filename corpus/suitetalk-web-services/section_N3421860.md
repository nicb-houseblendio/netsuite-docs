---
id: "section_N3421860"
type: "section"
title: "Enumerations, Special Characters, and Character Encoding"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Setup > SOAP Web Services Development Considerations > Enumerations, Special Characters, and Character Encoding"
parent: "section_N3421363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421860.html"
anchors: ["subsect_157069421340"]
sha256: "db3e4151130f963b6ad44895a4f9a4dc2b1385f8c7e04526c45209692086505e"
---

When enumerations contain either special characters (letters with diacritics or non alphanumeric characters) or reserved keywords ('private' or 'public' for example), both .NET and Axis may generate less usable code on the client side. To resolve this, prefix all enumerated values in NetSuite SOAP web services with an underscore '\_', except for enumerated values from the platformCore, platformCoreTyp, platformFaults, platformFaultsTyp, and platformMsgs XSDs. For example, without the '\_', .NET prepends an '@' symbol to the variable, as in '@private'.

## Character Encoding {#subsect_157069421340}

SOAP web services and the NetSuite UI support UTF-8 character encoding.

### Related Topics

-   [Development Considerations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421458.html)
-   [NetSuite Features in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421552.html)
-   [SOAP Web Services Reliability Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540364662.html)
-   [Effects of Account Configuration in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421585.html)
-   [Image References in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "chapter_N3784994"
type: "chapter"
title: "Country, State, and Language Enumerations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Country, State, and Language Enumerations"
parent: "book_156388697975"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3784994.html"
anchors: []
sha256: "9014b42c180754a5d5efc384d971bc452cb754f39fae49a83ffda831c2ae7e6b"
---

The following sections list all country and language enumerations defined in SOAP web services, as well as explain how to set and validate state values in your SOAP web services requests:

-   [Country Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3785183.html)
    
-   [Setting State Values in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3796175.html)
    
-   [Language Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3796595.html)
    

Important:

Be aware that NetSuite uses country/state validation. This means that if the _Allow Free-Form States in Addresses_ preference is set to FALSE, the state value is validated against the country. For example, you would not be able to set **CA** for **UK** since California is not a state that exists within the United Kingdom. For information about setting the _Allow Free-Form States in Addresses_ preference, see [Setting the Allow Free-Form States in Addresses Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3796175.html#bridgehead_N3796390).

As a general rule, enumerations are camel-cased concatenations of the country name as defined in the NetSuite UI.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

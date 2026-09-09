---
id: "section_N2497278"
type: "section"
title: "Input Parameters/Return Values for Shopping Object Methods"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > Shopping Objects > Input Parameters/Return Values for Shopping Object Methods"
parent: "section_N2496577"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497278.html"
anchors: ["bridgehead_N2497288", "bridgehead_N2497306"]
sha256: "ae760d6b6703391e15d6f05dd1b7813b51d3212f060f1207b989441371987e23"
---

## Set Functions {#bridgehead_N2497288}

Either a primitive string or a JSON object can be passed in to **set** methods, depending on their implementation. A primitive string would be used primarily to hold an object key, whereas a JSON object would provide a flat representation of an object's name/value pairs.

## Get Functions {#bridgehead_N2497306}

An optional array can be passed in as a filter to **get** methods. If field names are passed in to a **get** method, only the name/value pairs for the passed field names are returned. If no field names are passed, all name/value pairs for the expected object are returned. If no value is available for a field, null is returned for that field.

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

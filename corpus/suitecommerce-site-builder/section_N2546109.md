---
id: "section_N2546109"
type: "section"
title: "Working with Field Changed Client Events"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > SuiteScript for Scriptable Cart > Working with Field Changed Client Events"
parent: "section_N2545233"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html"
anchors: []
sha256: "0f4bd784f79e4987ed04083c49c050b6957c5d110bfc35b283f8bc6693344ff2"
---

Sometimes, a change to one field triggers an automatic update to another field. For example, a change to a shipping address can trigger a change in the list of shipping methods available. In this example, the shipping address field is the **controlling** field, and the field that shows the list of shipping methods is the **dependent** field.

In NetSuite, field change events on a controlling field are triggered before a dependent field is automatically updated. If you modify the value in a dependent field using a field change script, the post-field change automatic update can override your changes.

Note that the **post sourcing event handler** is triggered only after the dependent field is updated by the system. Using this event will guarantee that your field changes are not overridden. Also note that the post sourcing event handler is triggered only if a dependent field exists.

For more information, see [Client Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html).

For more information about controlling fields and dependent fields, see [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html).

### Related Topics

-   [Creating Custom Functions for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545908.html)
-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

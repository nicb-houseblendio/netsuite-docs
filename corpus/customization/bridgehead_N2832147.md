---
id: "bridgehead_N2832147"
type: "bridgehead"
title: "Dynamic Hyperlinks"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Dynamic Defaults and Dynamic Hyperlinks > Dynamic Hyperlinks"
parent: "section_N2832010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832147.html"
anchors: []
sha256: "eb848e4c2827ac658db1d4bf3d4814a6a22387cbbaa688feb4a9bb7557d1f1cd"
---

For hyperlink fields, you can create a link to a website by defining dynamic defaults. Dynamic defaults are especially useful when the exact URL is unknown until information is collected for the record. You may also want to use information specific to the current logged in session as part of a URL parameter. When creating a dynamic hyperlink, in the Default Value field enter the http address as usual followed by **?=** and the required NetSuite tags embedded in curly braces.

For example, suppose that you want to include an address lookup feature on a customer form. Create a custom Entity field with the following parameters specified:

-   Label: Map
    
-   ID: \_map
    
-   Type: Hyperlink
    
-   Store Value: Not checked
    
-   Applies To: Customer
    
-   Display / Subtab: Main
    
-   Display / Link Text: Click Here for Google Map
    
-   Validation & Defaulting / Default Value:
    
    http://maps.google.com/maps?q={billaddr1}%20{billcity}%20{billstate}%20{billzip}
    
-   Validation & Defaulting / Formula: Not checked (after you save the field, return to the custom field configuration page and ensure that Formula is cleared)
    

The default value includes NetSuite tags that identify the specific address of the current customer. These tags are resolved when the page is loaded so that the URL will direct the user to the customer's address as defined in the current customer record.

Note:

When creating dynamic hyperlinks, ensure that NetSuite tags embedded in the default value definition represent required fields. If the fields **aren't** required, and the associated form **doesn't** include a value for the tag, then the resulting URL will be not be valid.

### Related Topics

-   [Dynamic Defaults and Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832010.html)
-   [NetSuite Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832058.html)
-   [Setting the Store Value Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762215.html)
-   [Setting the Formula Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762294.html)
-   [Predefined Formula Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_160492514847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

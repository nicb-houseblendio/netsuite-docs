---
id: "bridgehead_N2832058"
type: "bridgehead"
title: "NetSuite Tags"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Dynamic Defaults and Dynamic Hyperlinks > NetSuite Tags"
parent: "section_N2832010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832058.html"
anchors: []
sha256: "316c1e18fca86ec185868b5c208dda164a4f67cd03914f4e86fe69c2e8e5aa4e"
---

Currently any field on the page that has a custom code ID can be used in a NetSuite tag. You can find the code ID for standard NetSuite fields in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/account.html).

To determine the code ID of custom fields on your forms, go to the Custom Field list page for the field type, for example, _Customization > Lists, Records, & Fields > CRM Fields_. The code ID is displayed in the ID column.

You can also use these special tags that work only when the Formula box **is not** checked:

-   **{useremail}** - Email of the user currently logged in
    
-   **{now}** - Current date
    
-   **{today}** - Current date
    
-   **{nlversion}** - The full internal NetSuite release number
    
-   **{nlsessionid}** - The browser's session ID, which could be used when creating a hyperlink for passing a session to a web service
    
-   **{nluser}** - ID of the user currently logged in
    
-   **{nlrole}** - Role ID of the user currently logged in
    

### Related Topics

-   [Dynamic Defaults and Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832010.html)
-   [Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832147.html)
-   [Setting the Store Value Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762215.html)
-   [Setting the Formula Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762294.html)
-   [Predefined Formula Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_160492514847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

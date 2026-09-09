---
id: "bridgehead_N2879618"
type: "bridgehead"
title: "Prevent Access to a Custom Record Type through the User Interface"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Specifying Permission and UI Settings > Setting Permissions for a Custom Record Type > Prevent Access to a Custom Record Type through the User Interface"
parent: "section_N2879388"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2879618.html"
anchors: []
sha256: "0ede39190480558a2656c16258238a0f571bd0641a21dd5888624f6946dd131c"
---

This topic describes how you can block access to custom record types from the NetSuite user interface to enhance security, permitting record access only through programmatic means such as SuiteScript and web services.

You can clear the **Allow UI Access** box for a custom record type, to indicate that it can only be accessed programmatically. For example, you can access it using SuiteScript or web services. The **Allow UI Access** box is checked by default.

When this box is cleared:

-   You can't access the custom record type from the NetSuite user interface.
    
-   If you attempt to list, search, view, edit, or create a record of this type in the user interface, the following error message appears: Access to that record type from the user interface isn't allowed.
    
-   The following custom record options are locked as disabled: Allow Mobile Access, Allow Quick Search, Allow Quick Add, and Include in Search Menu.
    

Important:

You need to take additional steps to control access to custom record data through searches. For more information, see [Limiting Search Access to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880332.html).

### Related Topics

-   [Setting Permissions for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879388.html)
-   [Define the Permission Model for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2879432.html)
-   [Changes to 'No Permission Required' Access on Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0816050536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

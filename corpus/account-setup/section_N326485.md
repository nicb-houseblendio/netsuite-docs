---
id: "section_N326485"
type: "section"
title: "Permissions Documentation"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > Permissions Documentation"
parent: "chapter_N284861"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html"
anchors: ["subsect_1518122070"]
sha256: "fc3a2c200ebe54f94725ea00525b33afb5e489fd394bfeb3b6c71ac9a2a7b989"
---

The following link provides access to a Microsoft Excel worksheet that lists how most NetSuite permissions are used. You can use this list to see what happens when you assign a specific permission, or to find the permission required to provide access to a specific task or page. The spreadsheet format lets you search and sort fields however works best for you. Each column has autofilters you can use.

To access the worksheet, click this link: [NetSuitePermissionsUsage.xls](https://system.netsuite.com/core/media/media.nl?id=476506172&c=NLCORP&h=rSpTfWUNDHFfLRF8wETfpPkE66jAIyo1Ojt3eoer-YN82cVG&_xt=.xls).

For information about standard roles and their associated permission levels, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html). For information about permissions required to access specific NetSuite features, see [Feature Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html).

Note:

Most browsers will download this file in 'Protected View' mode to your Downloads folder. If the Autofilters aren't working, click the **Enable Editing** button on the yellow bar in the worksheet header.

The NetSuitePermissionsUsage.xls file includes the following columns:

-   **SUBTAB** - Subtab of the Roles page Permissions subtab where each permission is listed: Lists, Reports, Setup, and Transactions (sorted alphabetically)
    
-   **PERMISSION NAME** - Name of each permission (sorted alphabetically)
    
-   **USAGE DESCRIPTION** - Description of how each permission is used, meaning the record types, tasks, and pages that each permission makes accessible (sorted alphabetically)
    
-   **MINIMUM SELECTABLE LEVEL** - The minimum selectable level (view, create, edit, or full) for each permission.
    
-   **MINIMUM SYSTEM LEVEL** - Contains the minimum valid level of permissions in the system. This level takes precedence in case it differs from the level in the Minimum Selectable Level column. This column is blank from most rows.
    

Note:

This worksheet doesn't show how different access levels affect each permission usage; it simply lists the minimum level required. Some permissions follow an access model where each level (view, create, edit, full) gives you more access to the related record type, task, or page, as described in [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html). But some permissions don't fit exactly into this model. For some permissions, you only need the minimum view level, and other levels don't give you any additional capabilities. In general, any user with at least VIEW access to a transaction type on the Transactions subtab, or to a record type on the Lists subtab, can print records of that type.

The worksheet lists some permissions multiple times because they give access to different record types, tasks, and pages. Note that some permissions depend on other permissions, and this spreadsheet doesn't include these dependencies.

Important:

The contents of NetSuitePermissionsUsage.xls are subject to change. Data is current as of the date listed in the worksheet footer. This worksheet shows how each permission works on its own. But since most roles include many different permissions, it's important to review permission changes in the context of each role and to test them before deploying them to users in your account.

For a list of permission IDs to use with SuiteScript, see [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html).

## Two-Factor Authentication (2FA) is Required for Specific Permissions {#subsect_1518122070}

Standard and custom roles with certain permissions need 2FA. For more information, see [Permissions Requiring Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515446005.html)..

### Related Topics

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [NetSuite Access Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285060.html)
-   [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html)
-   [Roles and Permission Considerations for APIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0320025211.html)
-   [Feature Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html)
-   [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html)
-   [NetSuite Users Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N321756.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

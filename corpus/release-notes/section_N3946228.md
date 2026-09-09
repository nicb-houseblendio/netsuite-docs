---
id: "section_N3946228"
type: "section"
title: "SuiteBuilder - Customization"
branch: "release-notes"
category: "what-s-new"
breadcrumb: "What's New > Release Notes > NetSuite 2026.2 Release Notes > SuiteBuilder - Customization"
parent: "article_72152418635"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3946228.html"
anchors: ["subsect_31132340614", "subsect_47124627700", "subsect_70133444116"]
sha256: "63e3deb448bcd9a4ccc5b2828a330e0cc6ed01493d785ef5c6d9a65755aa44f0"
---

NetSuite 2026.2 includes the following enhancements to SuiteBuilder features:

-   [Manage Records with Advanced Record Customization](#subsect_31132340614)
    
-   [New Currency Context for Currency Custom Fields](#subsect_47124627700)
    
-   [AI Description Field Added for Custom Records, Fields, and Transactions](#subsect_70133444116)
    

## Manage Records with Advanced Record Customization {#subsect_31132340614}

Advanced Record Customization (ARC) provides a centralized layer where administrators can review, manage, and override record definitions from a single location.

ARC supports overrides not only for custom record type and custom transaction types but also for selected standard record types. ARC applies overrides at the account level. When an ARC override exists, changes made elsewhere in NetSuite or through installed partner solutions are not applied.

The first record definition attribute that administrators can override is AI Description.

To access ARC, go to **Customization > Advanced Record Customization**.

Administrators can currently use ARC to:

-   View and filter a list of existing record types, including details such as the name, ID, record family, record type source, and effective AI description.
    
-   View effective AI descriptions across supported record types.
    
-   Identify record types that use ARC AI description overrides.
    
-   Create or update AI description overrides.
    
-   Add AI descriptions for SuiteApps and bundles when no description is provided by the SuiteApp owner or bundle owner.
    
-   Compare default and override AI descriptions.
    
-   Revert overrides to restore the default AI description.
    
-   Use the Optimize for AI feature when editing descriptions.
    

When an ARC AI description override exists, the override becomes the effective AI description used by AI features.

For more information about AI Description, see [AI Description for Custom Object Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0109014837.html).

## New Currency Context for Currency Custom Fields {#subsect_47124627700}

You can now configure a currency context for currency custom fields. A new Currency Symbol Field is available on a new Currency Context subtab for Currency type custom fields. This field lets you associate a currency with values stored in these fields by selecting a currency symbol field as the source.

Previously, currency custom fields stored numeric values without currency context. With this enhancement, reports and analytics tools can display values with the correct currency and apply currency-aware processing. Other areas, such as transaction forms and saved searches, are not affected.

Setting a currency context affects how values are displayed and summarized for both existing and future data. If you clear the currency context, the field reverts to numeric-only behavior.

This feature is optional and doesn't require changes to existing custom fields. Existing configurations and current reporting experiences remain unchanged unless currency context is configured.

Currency context configuration supports SuiteApps and bundles, including export and import of the configuration. If the selected currency source field is removed during SuiteApp or bundle uninstallation, the reference is automatically cleared.

To use this feature, go to Customization > Lists, Records, & Fields > \[Field Type\], and create or edit a Currency custom field type.

## AI Description Field Added for Custom Records, Fields, and Transactions {#subsect_70133444116}

AI Description fields have been added for custom records, custom fields, and custom transactions definitions for all customers. These fields appear in the main body section of each definition page. Administrators can use this field to provide concise, meaningful descriptions (up to 280 characters) of custom objects. The Optimize for AI action enhances the description for AI use. AI features use the description to understand the meaning of the custom object. This enables them to deliver relevant, meaningful answers to user questions about the object.

Descriptions added in the AI Description field are used by NetSuite AI features, such as NetSuite AI Connector Service. This service uses Model Context Protocol (MCP) to connect external AI platforms (such as ChatGPT or Claude) to your NetSuite data, enabling smarter responses and integrations. For more information, see [NetSuite AI Connector Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7200233106.html).

For more information, see [AI Description for Custom Object Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0109014837.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

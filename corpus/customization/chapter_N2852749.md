---
id: "chapter_N2852749"
type: "chapter"
title: "Custom Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms"
parent: "book_N2823893"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html"
anchors: ["bridgehead_N2852774", "bridgehead_N2852806", "bridgehead_3920803592", "bridgehead_1540403146"]
sha256: "d14ce8215d60b88819b69ff9701fce7cb548dd6872d31fbb693dfee4283d8576"
---

Forms are the pages used to enter information into the NetSuite database. The standard set of forms provided with your NetSuite account can be customized to better suit your business needs. For example, you may want to reorganize subtabs or rename fields to better match your business workflow and terminology. After you create a custom form, you can set it as the preferred or default form for a page or select it as needed from a custom form list.

Note the following details:

-   Form preferences are controlled by settings on the custom forms page as well as settings defined for each role.
    
-   The Manage Translations feature enables you to manage your language translations using translation collections. You should edit translations for custom forms using a translation collection because it's more efficient than making the edits on the Translation subtabs in the user interface. For more information, see [Managing Translation Collections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161581766777.html).
    
    Translations used in custom forms are primarily taken from custom field and custom segment definitions. You can override a field label on the custom form definition page, but it's often not the best approach. When you translate a field label on the Translation subtab of a custom field, the translated label overrides the language set up in Home > Set Preferences. Language changes will be visible only to users with the same language preference. For example, if you change the language from English (US) to English (International), only users with the English (International) language preference will see the changes. For more information about translations, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).
    
-   If you use SDF and the Multi-Language feature is enabled, you can enter translations in forms in SDF XML. You should define translations using a translation collection. For more information, see [Translation Collections as XML Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1552071708.html).
    
    If you modify a form and enter a translation string directly in the form, the translations aren't connected to terms or translations collections. They are visible only to users with the same language preference. If you change your language preference, then you must also define the translations for that language.
    
-   Any settings defined for a specified role override the preferred form settings on the forms page. For Employee Center roles, only one form is ever made available to this type of role.
    

Important:

SuiteScript does not support direct access to the NetSuite UI through the Document Object Model (DOM). You should access the NetSuite UI only by using SuiteScript APIs. For information about using SuiteScript APIs to customize the UI, see [SuiteScript 2.1 Custom Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1518456405.html).

Custom forms are supported in SuiteCloud Development Framework (SDF). SDF is a development framework that you can use to create SDF SuiteApps, or to customize NetSuite accounts, using an integrated development environment (IDE) on your local computer. SuiteCloud projects are file-based and use XML definitions of custom NetSuite objects. For more information, see [SDF Custom Object and File Development in SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4715411907.html).

## Custom Entry Forms {#bridgehead_N2852774}

You use entry forms to enter information into NetSuite. To create your own custom entry forms, start with an existing standard form and customize it. On the custom form, you can rearrange, rename, hide, or disable fields, subtabs, and buttons. You can also make specific fields required, add custom fields, or apply custom code.

For detailed information about how to customize an entry form, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html) and [Customizing Address Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874310.html).

After you've created a custom entry form, you can set it as the default form or preferred form for specific user roles. For more information, see [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html) and [Setting Default Forms for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N290202.html).

## Custom Transaction Forms {#bridgehead_N2852806}

You use transaction forms to enter and print transactions in NetSuite. To create your own custom transaction form, start with an existing standard form and customize it. On your custom form, you can rearrange, rename, hide, or disable fields, subtabs, and buttons. You can also make specific fields required, add custom fields, or apply custom code.

For detailed information about how to customize a transaction form, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

After you create a custom transaction form, you can set it as the default or preferred form for specific user roles. For more information, see [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html) and [Setting Default Forms for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N290202.html).

You can also link transaction forms together to create transaction workflows. For more information, see [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html).

## Important Note about New Fields and Custom Forms {#bridgehead_3920803592}

Be aware that as part of a new release, new fields are sometimes added to NetSuite standard record types. When new fields are added to a record type, they're automatically added to your customized forms for that record type. These fields are set to show on customized forms. If you don't want new fields to show on your customized forms, you'll need to modify them after an upgrade to remove or hide the fields. Keep in mind that newly created fields are typically coupled with forms and can be needed for some forms to function properly. You should test any customized forms where you remove or hide fields, to ensure that the forms still function properly.

## Optimizing Custom Form Performance {#bridgehead_1540403146}

To optimize form performance, use a minimalist approach with your custom forms. Ensure that you:

-   Limit the number of fields and sublists.
    
-   Keep client scripts and workflows on forms to a minimum and manage them carefully. For more information, see [SuiteScript 2.1 Client Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387798404.html).
    
-   Implement server callbacks only when needed.
    
-   Use the browser built-in code inspection tools to audit the scripts on a form page.
    

For information about form templates for customizing entry and transaction forms, see [Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163605126400.html).

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2823893.html)
-   [Customization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html)
-   [Customization Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163039950342.html)
-   [Customizing Field Level Help for Standard Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1530729846.html)
-   [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html)
-   [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html)
-   [Advanced Templates Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates.html)
-   [Basic Printing Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453552264.html)
-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Custom Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4172599049.html)
-   [Custom Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4313464438.html)
-   [Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2890160.html)
-   [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

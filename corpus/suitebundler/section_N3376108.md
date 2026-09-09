---
id: "section_N3376108"
type: "section"
title: "Bundle Object Preferences"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Bundle Object Preferences"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html"
anchors: ["bridgehead_N3376370", "bridgehead_N3376768", "bridgehead_N3376797"]
sha256: "12f4388e8d61485477bb73cde09e6f27591e11ff89cb4a30b2f38e853a6c29d4"
---

For customization bundles, preferences are available for some object types. These preferences, which are applied during bundle installations and updates in target accounts, help to properly set up bundle objects. You set these preferences on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder when you create or edit a bundle, by choosing from options displayed in Preference column dropdown lists.

You can control preferences for pushed and managed bundle accounts, and you can supply default preferences for other install base accounts. The bundle preference options you choose are applied directly to target accounts during managed bundle and other pushed bundle installations and updates. For other bundles, target account administrators can override these preferences before bundle installation or update.

The Bundle Builder offers preferences for the following object types:

-   **Dashboards**
    
    For any dashboard, you can set a preference to indicate whether updates to the bundled dashboard should be applied to the dashboards of target account users to whom the dashboard has been published. (Updates are always applied to the target account dashboard definition.)
    
    This setting is applied during bundle updates, when the dashboard is updated in the target account.
    
    The default option is not to apply updates to users, allowing target account administrators to publish updates to users' dashboards as desired after bundle updates. See [Applying Changes to Published Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N634404.html).
    
-   **Custom Fields**
    
    For any custom field, you can set a preference to choose whether the field should be shown or hidden on existing custom forms in target accounts. The default option is to hide the field.
    
    This setting is applied during bundle installations and updates, whenever the field is first added to a target account. This setting does not affect bundled forms, because all custom fields in a bundle are always shown on all custom forms included in that bundle.
    
-   **Custom Lists**
    
    For any custom list, you can set a preference, applied during bundle updates, to choose whether: the bundled custom list data should replace data in the target account custom list, the target account custom list data should be preserved, or data from the bundled custom list and target account custom list should be merged. The default option is to preserve data.
    
    This preference is also available, during both installations and updates, for conflicting custom lists that have the **Replace Existing Object** option chosen. See [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).
    
-   **Custom Records**
    
    For any custom record that includes data, you can set a preference, applied during bundle updates, to choose whether: the bundled custom record data should replace data in the target account custom record, the target account custom record data should be preserved, or data from the bundled custom record and target account custom record should be merged. The default option is to preserve data.
    
    This preference is also available, during both installations and updates, for conflicting custom records that include data and have the **Replace Existing Object** option chosen. See [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html).
    
-   **Custom Segments**
    
    For any custom segment that includes data, you can set a preference, applied during bundle updates, to choose whether: the target account custom segment data should be preserved, or data from the bundled custom segment and target account custom segment should be merged. The default option is to preserve data.
    
    When the **Preserve Data** option is selected, the bundle update does not make any changes to target account custom segment values. When the **Merge Data** option is selected, the bundle update merges custom segment values, without deleting any values from the target account custom segment. The avoidance of target account custom segment value deletion is due to the possibility that a custom segment may have GL impact. In addition, no option is provided to replace data for a custom segment, also to avoid unintentional changes to GL impact.
    
    For more information about bundling custom segments, see [Adding a Custom Segment to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4520725557.html).
    
    Note:
    
    If a custom record's data is referenced by another custom record for which the Include Data preference is enabled, data for the referenced custom record is included as well, even if the Include Data preference is not enabled for that referenced custom record.
    

-   **Custom Forms**
    
    For any custom form, you can set a preference to choose whether the form should be set as the preferred form for the record type in target accounts. The default option is not to set the form as preferred.
    
    Warning:
    
    This setting is applied during pushed installations only. Unlike other preferences, bundle installers cannot override this preference's Bundle Builder setting.
    
-   **SuiteScripts**
    
    For any SuiteScript, you can set a preference, applied during bundle updates, to choose whether target account script deployments should be updated with deployments from the bundled scripts. The default option is to not update target account script deployments, leaving them unchanged after the bundle update.
    
    If the update deployments option is applied, bundled script deployments completely overwrite target account script deployments, except for script deployment audience definitions. Bundle updates implement an intelligent merge of audience definitions in source and target accounts when the update deployments option is applied. For details, see [Bundle Update Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400349.html).
    
    Note that changes to an icon associated with a dashboard SuiteApp portlet are always copied during a bundle update. This overwrite of the icon in the target account occurs even if the bundle preference is set to prevent the update of script deployments. See [Giving Users Dashboard Access to a SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html#bridgehead_4852122809).
    
    Note:
    
    Bundle updates do not change the values of script deployment parameters that have a user or company preference set, even if the bundle preference for the script is set to Update Deployments. For more information, see [Script Parameter Preference Updates in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html).
    

## Bundle Object Preferences Table {#bridgehead_N3376370}

The following table provides a quick reference to customization bundle object preferences:

| Object | Options (\*\* = Default) | Applied During |
| --- | --- | --- |
| Dashboards | 
Do Not Update Users\*\*

Update Users



 | updates |
| Custom Fields | 

Hide on Existing Custom Forms\*\*

Show on Existing Custom Forms



 | 

installations,

updates (if new fields)

Note: This setting is applied whenever the field is first added to a target account. This setting does not affect bundled forms, because all custom fields in a bundle are always shown on all custom forms included in that bundle. |
| 

Custom Lists

Custom Records (Include Data only)



 | 

Preserve Data\*\*

Replace Data

Merge Data



 | 

installations,

updates

(for conflicting objects with Replace Existing Objects chosen and for objects to be updated)



 |
| Custom Segments | 

Preserve Data\*\*

Merge Data



 | updates |
| Custom Forms | 

Not Preferred\*\*

Preferred Form for Record Type



 | installations (push only) |
| SuiteScripts | 

Do Not Update Deployments\*\*

Update Deployments



 | updates |

## Preferences in Bundles Created Prior to Version 2011 Release 1 {#bridgehead_N3376768}

Most bundle object preferences became available to bundle authors as of Version 2011 Release 1. After your account was upgraded to this release, any bundles that you created prior to this release have the default option set for each preference. If you want one of these bundles to use any non-default options, you need to edit the bundle in the Bundle Builder and explicitly set the preference(s). See [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html).

Note:

The preference for dashboards became available as of Version 2012 Release 1.

## Preferences in Copied Bundles {#bridgehead_N3376797}

Preferences set for a bundle are not applied in an account where the bundle is copied. Note that data is always replaced and script deployments are always updated during an update of a bundle copy. However the preferences set for a bundle are maintained as the defaults on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the copied bundle, and are applied in target accounts where the copied bundle is installed, unless the preferences are edited in the copied bundle. See [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html).

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

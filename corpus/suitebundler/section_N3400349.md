---
id: "section_N3400349"
type: "section"
title: "Bundle Update Reference"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Installed Bundle Updates > Bundle Update Reference"
parent: "section_N3397927"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400349.html"
anchors: ["bridgehead_4405440698", "bridgehead_4405380817"]
sha256: "aaa4c5f31b5d92a7dacd4896b73bfebcc318af065d3c6e4f0d4339e6ce1de3ec"
---

In general, updating a bundle causes unlocked bundle objects in the target account to be updated to match source account bundle objects. If you change any of the unlocked elements of an installed bundle, a bundle update may overwrite or merge the changes. If a bundle update overwrites target account objects, you must redo the changes after each bundle update.

The following table describes possible changes to target account objects during a bundle update:

| Bundle Object | Description |
| --- | --- |
| Custom field names | Changes to custom field names are copied into the source account. For example, you install a bundle that includes a custom record with a field labeled **Name**, which is set to **Include Data**. You change the name of the **Name** field to **Company**. The bundle creator revises the bundle and then adds it to a deployment account. When you install the updated bundle, the field label changes from **Company** back to **Name**. |
| **Inactive** property on custom fields | You can use Customization to set custom fields to **Inactive** instead of deleting the custom field. However, if a custom field in a bundle is inactive, SuiteBundler may not set the custom field to inactive in the target account when you update the bundle. If the custom field is inactive in a bundle but active in the target account, and you update the bundle, the custom field remains active in the target account after the bundle update. For more information about the **Inactive** property for custom fields, see [Inactivating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4352401817.html). |
| Custom form preferences | Generally, If a bundle update includes any custom forms that are set as preferred for one or more roles, these preferences overwrite any custom forms previously set as preferred in the target account. However, a custom form set as preferred for a custom record in a bundle only carries over after a bundle update if the custom record did not previously have a preferred form set in the target account. If after bundle installation a preferred form was set for the custom record in the target account, a bundle update does not change this preferred form. |
| **Access Type** property on custom records | If the **Access Type** value for a bundled custom record is edited in a target account, that new value is kept after a bundle update, if the custom record is not locked in the bundle. For example, you install a bundle that contains a custom record with an **Access Type** of **Use Permission List**. In the target account, you change the access type for the custom record to **No Permission Required**. A bundle update does not overwrite the target account value of **No Permission Required** with the bundle value of **Use Permission List**. If a custom record is locked in a bundle, a bundle update overwrites the **Access Type** value in the target account with the value from the bundle. |
| Permissions for standard roles on custom records, custom transactions, and custom segments | Changes to standard role permissions for custom records, custom transactions, and custom segments in a bundle may not be reflected in a target account after a bundle update. There is no way to determine whether a difference in permissions between the bundle and the target account is a result of a change in the bundle or of a manual change in the target account. To avoid overwriting changes made in the target account, the bundle update does not modify these permissions. |
| Workflows | The update of a workflow in a target account depends on the difference between the states and transitions in the source and target accounts. For more information, see [Workflow Handling on Bundle Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4405461304.html). Workflow instances and history logs from the source account are not copied to target accounts when a bundle is updated. Workflow release status is not updated in the target account when a bundle is updated or copied. You can set your preferred workflow release status in the target account manually. |
| Audiences | Generally, bundle updates implement an intelligent merge of bundle object audience definitions in source and target accounts. If the **Select All** box is checked for employees, customers, vendors, or partners in the source object audience, this selection overwrites the target object audience. If the **Select All** box is not checked for the source object audience, employees, customers, vendors, and partners are not deleted from the target object audience. However, the target object audience may still be overwritten during the merge. For details about how the merge is done, see [Object Audience Handling on Bundle Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4405459556.html). |
| Hierarchical custom record data | SuiteBundler updates the custom record data in the target account depending on the bundle preference that you specify when you update an existing bundle. See [Hierarchical Custom Record Data Handling on Bundle Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4403771811.html). |
| Center category links | If a custom category in the target account came originally from a bundle, a bundle update removes all existing custom record links from that custom category in the target account and adds any custom record links in the updated bundle to that custom category in the target account. If a user in the target account creates a custom category in the target account with links to custom records, a bundle update does not remove these links from the custom category, even if they link to custom records that came initially from the bundle. A bundle update does not remove any links to standard categories from the target account, because it is not possible to determine whether these links originated from the bundle or not. Important: Be aware that the handling of bundled links described above may result in unexpected links in the target account after bundle update. For example, a change of links in the source account may result in these changed links being installed in the target accounts when the bundle is updated, whereas existing links in the target account are preserved. In this case, duplicate links may occur in target accounts. |
| SSP application files | During a bundle update, conflicts between bundle files and target account files in the SSP Application folder are detected. In case of such a conflict, the bundle update deletes the target account file and replaces it with the file from bundle. |

## Exceptions to Bundle Update Overwrites {#bridgehead_4405440698}

The following table describes exceptions to the bundle overwrite rules:

| Bundle Object | Exception |
| --- | --- |
| Custom field display order | A bundle update does not impact the display order of custom fields in a target account. The display order is left as is after a bundle update. It is not changed to match the display order of custom fields in the source account. |
| Script parameters | Script parameters defined as user, company, or portlet preferences are not overwritten in the target account unless the type of the preferences changes in the bundle. If the default value of the preference in a script deployment changes in the bundle, the default is carried over without affecting the preferences specified in the target account. |
| Script deployment audience definitions | Script deployment audience definitions in target accounts are not overwritten by definitions in an updated bundle, even if the Update Deployments option is selected for the update. |
| Custom lists | Custom lists updated by a bundle author are replicated in the target account. If the developer removed items from the list, then this item will also be removed from your account. To preserve Custom List options in the target, choose the **Update Data** or **Preserve Data** preference. See [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html). |
| Custom records converted to custom lists | For objects installed from bundles as custom lists and converted in target accounts to custom records, the record is not converted back to a custom list when the bundle is updated, even if the object is locked as a custom list in the source account. Similarly, you cannot convert custom records to custom lists in the NetSuite UI. |

## Guidelines for Changing Bundle Objects in a Target Account {#bridgehead_4405380817}

You should use the following guidelines when editing bundle objects in the target account:

-   If you plan to update a bundle with changes from source, do not update bundle objects such as forms, scripts, or custom fields, because updates will overwrite these changes.
    
-   If you want to make changes to a custom object from an installed bundle, create a copy of the object before making the changes and make changes to the copy, so that future updates do not overwrite the changes.
    

### Related Topics

-   [Installed Bundle Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397927.html)
-   [Choosing a Bundle to Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399359.html)
-   [Reviewing the Preview Bundle Update Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3399556.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

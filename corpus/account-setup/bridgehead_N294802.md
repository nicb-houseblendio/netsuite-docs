---
id: "bridgehead_N294802"
type: "bridgehead"
title: "Adding Custom Role Fields to be Mass Update Filter Criteria"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Mass Updating a Permission on Custom Roles > Adding Custom Role Fields to be Mass Update Filter Criteria"
parent: "section_N293188"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N294802.html"
anchors: ["procedure_N294837"]
sha256: "71640b147f72b126356f7aabfaae1af4cc11954f474c6f71567ba73899039c16"
---

To increase the effectiveness of the Add/Edit Permission on Roles mass update, you can add one or more custom fields to the role record. This kind of field can be used to categorize roles and provide filter criteria for the mass update. The type of custom field that can be added to role records is the Other Custom Field type.

The steps below provide steps for creating this type of field. For further details, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html) and [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html).

#### To create a custom field to be added to the role record: {#procedure_N294837}

1.  Go to _Customization > Lists, Records, & Fields > Other Record Fields > New_.
    
2.  From the **Record Type** dropdown list, select **Role**.
    
3.  In the **Label** field, enter a name for the field.
    
4.  From the **Type** dropdown list, select the type of field.
    
    For example, you can choose **List/Record** if you want the field to be a dropdown list with multiple options. For this choice, you need to select the list or record that supplies dropdown list options. You may need to first create a custom list of these options, then return to creating this custom field. See [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html).
    
5.  To add the field to the role page, select a value in the **Insert Before** field.
    
6.  Complete other fields as necessary.
    
7.  Click **Save**.
    

After you have created this custom field, you can set its values on role records as desired, then use it as a filter criteria for the Add/Edit Permission on Roles mass update.

The following screenshots show the record for a sample custom field, its associated custom list, and the field on the role record:

![Other Custom Field page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/AccountSetup/NewOthCustField.png) ![Custom List page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/AccountSetup/CustListRole.png) ![Role page with the Role type list.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/AccountSetup/CustRoleField.png)

### Related Topics

-   [Mass Updating a Permission on Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N293188.html)
-   [To Mass Update a Permission for Multiple Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N293248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

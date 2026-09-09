---
id: "section_N2879931"
type: "section"
title: "Setting Up a Permissions List for a Custom Record Type"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Setting Up a Permissions List for a Custom Record Type"
parent: "section_N2876492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879931.html"
anchors: ["procedure_N2880017"]
sha256: "0e105dacab7744240807704e1633b7c622ab902826c9ee617f2cfe99cb6f65d7"
---

You can manage access to a custom record type's data by setting up a permissions list on the Permissions subtab of the record type page.

The Permissions subtab lets you restrict access by role to your custom records and the forms used to enter the records. By restricting access to custom records, you can have greater control over who sees the information specific to your business. By restricting access to the entry form, you can control the entry form used by your employees to enter custom records.

When you set permissions for your custom records, you restrict access to the record entries, **not** the record type. To edit, view, or enter a custom record type, you must have a role with permission to access to custom record types.

If you **don't** set permissions here, anyone with access to custom record entries can view, edit, and enter custom records for this type.

The role-based restrictions you set on this subtab are also available on the record for each role. Changes made on role records related to this custom record's permissions are reflected here.

Important:

For the permission settings in the Permissions subtab to take effect, the Use Permission List option must be selected for Access Type. These permission settings don't restrict search access to custom record data. You can limit search access to custom record data on a per-field or per-search basis. You can limit searches' access to custom record data on a per-field or per-search basis. For more information, see [Limiting Search Access to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880332.html).

#### To set up a permissions list for a record type: {#procedure_N2880017}

1.  On a custom record type page, click the **Permissions** subtab.
    
    Note:
    
    If the custom record type is associated with a custom segment, the Permissions subtab isn't available. The permissions must be set on the custom segment configuration page.
    
2.  In the **Role** column, select the role you want to have access to custom record entries of this type.
    
3.  In the **Level** column, select a level of access for this role. Available options include:
    
    -   **None**: People with this role can't use custom records of this type.
        
    -   **View**: People with this role can view custom records of this type.
        
    -   **Create**: People with this role can view and create custom records of this type.
        
    -   **Edit**: People with this role can view, create, and edit custom records of this type.
        
    -   **Full**: People with this role can view, create, edit, and delete records of this type.
        
4.  Select a value in the **Restrict** column to limit the access of users with the selected role to custom records of this type:
    
    -   To restrict users with this role to viewing or editing the records of this type that only they or their subordinates created, select **Viewing and Editing**.
        
    -   To permit users with this role to view all records of this type but restrict them to editing the records that only they or their subordinates created, select **Editing Only**.
        
    -   To permit users with this role to view and edit all records of this type, leave this column blank.
        
5.  In the **Default Form** column, select a default entry form for this role to use when entering records of this type.
    
    Note:
    
    The default form you set here for a role takes precedence over the preferred form setting on the **Forms** subtab.
    
    For example, you set Custom Record Form A as the preferred form on the **Forms** subtab. On the **Permissions** subtab, you set the default form for the Sales Rep role to Custom Record Form B. When a sales rep creates a new record, Custom Record Form B is selected by default.
    
6.  To make the default form the only entry form available to this role, check the box in the **Restrict Form** column.
    
7.  From the **Search Form** list, select a custom search form to be used for searches of this record type, if one is available.
    
8.  From the **Search Results** list, select a custom search to be used to limit results for searches of this record type, if one is available.
    
9.  From the **List View**, **Dashboard View**, and **Sublist View** lists, select a custom search to limit displayed results for these lists, if one is available. To make the selected view the only one available to this role, check a box in one of the **Restricted** columns.
    
10.  Click **Add**.
     
11.  Repeat these steps for each role you want to give access to.
     
12.  Click **Save**.
     

### Related Topics

-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
-   [Creating a New Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860307.html)
-   [Entering Name and Display Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860247.html)
-   [Specifying Permission and UI Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860092.html)
-   [Configuring File and Child Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859968.html)
-   [Defining Search and Edit Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859705.html)
-   [Adding Fields to Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878340.html)
-   [Limiting Search Access to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880332.html)
-   [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html)
-   [Adding Subtabs to a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2877748.html)
-   [Choosing an Icon for a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2881257.html)
-   [Numbering Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878042.html)
-   [Adding Custom Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878636.html)
-   [Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882522.html)
-   [Creating Links to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880942.html)
-   [Adding Translations for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882154.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

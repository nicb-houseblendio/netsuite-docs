---
id: "section_N2598904"
type: "section"
title: "Audience Permissions for Hosted Sites"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Website Hosting with Site Builder > Audience Permissions for Hosted Sites"
parent: "chapter_N2598224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598904.html"
anchors: ["procedure_N2598927"]
sha256: "6da04a57204a731fc76f50e685a1d0073660c567ae51976122987fbe077b94d8"
---

You can limit access to hosted sites for internal use, by granting access to specific users, roles, or groups.

NetSuite supports audience permissions on hosted sites through an Audience subtab on the root hosting folders in the Web Site Hosting Files folder.

When you select an audience for a website, all pages, associated tabs, images, and other files for that website can only be accessed by members of the audience that you select. These pages are protected from unauthorized access. Any user not included in the audience receives a 'Page Not Found' error message when trying to access the website URL.

This feature is typically used to limit access to an internal site, such as a sales or a professional services portal, on a NetSuite website tab.

#### To set up an internal hosted site for a select audience: {#procedure_N2598927}

1.  Go to _Commerce > Hosting > Website Hosting Files_.
    
2.  Click **New Folder** to create a new folder in the Web Site Hosting Files folder.
    
    For more information, see [Creating File Cabinet Folders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N541665.html).
    
3.  On the **Audience** subtab, clear the **Display in Web Site** box.
    
    When this box is cleared, files in the folder are no longer displayed to visitors on the website. Files will only display to members of the audience you select.
    
4.  Select the audience that is allowed to visit this site.
    
    You can base your audience on the following criteria. To view this site, a user must meet only one of the criteria you set in each category.
    
    -   Roles
        
    -   Departments
        
    -   Subsidiaries
        
    -   Groups
        
    -   Employees
        
    -   Customers
        
    -   Vendors
        
    -   Partners
        
    
    To select more than one item in each of these fields, press and hold CTRL.
    
5.  Click **Save**.
    

Now, you can upload the HTML files for your hosted site into the folder you created above, for more information on setting up a hosted site, see [Hosting HTML Websites with NetSuite Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598355.html).

### Related Topics

-   [Creating an HTML Intranet Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599141.html)
-   [Website Staging Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599525.html)
-   [External Catalog Site (WSDK) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600392.html)
-   [Example for Building a Combination Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599702.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

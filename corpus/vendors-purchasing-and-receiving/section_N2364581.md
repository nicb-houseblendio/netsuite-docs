---
id: "section_N2364581"
type: "section"
title: "Giving Vendors Access to Time Tracking"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Configuration > Giving Vendors Access to Time Tracking"
parent: "article_161952107343"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364581.html"
anchors: ["bridgehead_N2364683", "procedure_N2364738", "bridgehead_162341107283", "bridgehead_N2364887"]
sha256: "1c1eefdd56923fa212b94e0d8a455a323538a5af86aeb68f46280daa242905e3"
---

Giving vendors access to time tracking allows them to enter the hours they spend working on a project.

There are three steps to complete to give vendors access to time tracking:

1.  An administrator must enable the Time Tracking features and set time tracking preferences. For more information, see [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html).
    
2.  Create a vendor record for any vendor that you want to give access to time tracking. For more information about creating vendor records, see [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html).
    
3.  Do one of the following:
    
    -   [Give a Vendor Access to Vendor Center](#bridgehead_N2364683)
        
    -   [Assign a Custom Role With the Track Time Permission](#bridgehead_162341107283)
        

## Give a Vendor Access to Vendor Center {#bridgehead_N2364683}

If you enable project features required to use job costing and project budgeting, note the following. Vendors can enter time using the Vendor Center if the vendor is identified as a resource on the Resource subtab of a Project.

For information about the required features, see [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html).

For information about how to identify a vendor as a project resource, see [Identifying a Vendor as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188644.html).

You should follow this procedure to let vendors set a NetSuite password themselves. However, if you prefer to set their passwords yourself, see the procedure in [Manually Setting a Vendor's Password](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162341016930.html) instead.

#### To give the vendor access to the Vendor Center: {#procedure_N2364738}

1.  Go to _Lists > Relationships > Vendors_.
    
2.  Click **Edit** next to the vendor you want to give access to.
    
3.  Enter the vendor's email address.
    
4.  Click the **Access** tab.
    
5.  Check the **Give Access** box.
    
6.  Check the **Send New Access Notification Email** box to notify your vendor of this new access. The notification email includes the email address (used for logging in to NetSuite) and explains login procedures. It also contains a URL so that the vendor can set up a NetSuite password.
    
    Checking this box means is not necessary for you to enter a password or check the **Require Password Change on Next Login** box.
    
    Note:
    
    You should let the vendor create a password for NetSuite from the URL in the notification email. However, if you prefer to assign a password for the vendor, see [Manually Setting a Vendor's Password](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162341016930.html).
    
7.  In the **Role** column, select **Vendor Center**.
    
8.  Click **Add** to assign the vendor this role.
    
9.  Click the **Time Tracking** subtab.
    
10.  In the **Time Approver** field, select an employee to approve any time tracked by this vendor.
     
     If this field is blank, tracked is automatically approved unless entered against a project with project time approval preferences defined. For more information, see [Approving Time and Expenses for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html).
     
11.  Click **Save**.
     

## Assign a Custom Role With the Track Time Permission {#bridgehead_162341107283}

Alternatively, you can assign a custom role with proper permissions.

#### To assign a custom role with track time permission: {#bridgehead_N2364887}

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Click **Customize** next to the role you want to assign with time tracking permission.
    
3.  Enter a name for this custom role.
    
4.  Check the **Restrict Time and Expenses** box to only allow vendors to enter time for themselves.
    
5.  On the **Transactions** subtab, select **Track Time** in the **Permission** column.
    
6.  In the **Level** column, select **Full**.
    
7.  Click **Add**.
    
8.  Click **Save**.
    

Now you can assign this role on the Access tab of vendor records to give access to time tracking. When assigning your custom role, you must also assign a time approver on the Time Tracking subtab of the vendor's record. If you do not assign a time approver, any time tracked is automatically approved unless entered against a project with project time approval preferences defined.

### Related Topics

-   [Enabling the Vendor Access Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952527878.html)
-   [The Vendor Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369118.html)
-   [Assigning a Role to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2363606.html)
-   [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html)
-   [Vendor Credit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365918.html)
-   [Associating a Vendor With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367376.html)
-   [Associating a Vendor With a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367472.html)
-   [Importing a Vendor Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368077.html)
-   [Preferred Transaction Delivery on Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368449.html)
-   [The Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369578.html)
-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

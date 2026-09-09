---
id: "section_N1168834"
type: "section"
title: "Assigning the Advanced Partner Center Role"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Managing Partners > Assigning the Advanced Partner Center Role"
parent: "chapter_N1166465"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168834.html"
anchors: ["subsect_1533243458", "procedure_1533243458", "subsect_1533243579"]
sha256: "cfbd88a73952f7dbedc8f8fdd526558d58a5400d5c05bd9fc4b66d306d79fdd0"
---

On partner records, you can assign partners the Standard Partner Center role or the Advanced Partner Center role. Or you can create a role by customizing the Advanced Partner Center role. For information about the Advanced Partner Center, see [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html).

When you assign partners the Advanced Partner Center role, they have access to the default records, transactions, and reports available in the Advanced Partner Center.

## Assign the Advanced Partner Center Role {#subsect_1533243458}

To assign the Partner Center role to a partner, the Partner Access feature must be enabled. An administrator can enable the Partner Access feature at _Setup > Company > Enable Features (Administrator)_ > Web Presence subtab. Under the Access section, check both the Partner Access and the Advanced Partner Access boxes.

#### To assign the Advanced Partner Center role: {#procedure_1533243458}

1.  Go to _Lists > Relationships > Partners_.
    
2.  Click **Edit** on the required partner record.
    
3.  Click the **Access** subtab.
    
4.  Check the **Give Access** box.
    
    In the **Role** field, **Advanced Partner Center** is selected, by default. If you have customized the Advanced Partner Center role for this partner, select the name of that custom role here.
    
5.  Check the **Send New Access Notification Email** box to inform the user how to access your NetSuite account. The standard user access notification includes the email address to use for logging in to NetSuite. It also contains a URL so that the user can set up a NetSuite password.
    
6.  If you want to allow this partner to give access to subpartners, check the **Can Give Login Access to Subpartners** box.
    
7.  Click **Save.**
    

Now, your partner can access information in your NetSuite account. When your partner logs in, the partner can update the profile and view reports based on sales related to your partnership.

You can preview what your partner sees by clicking **View** next to the partner record from the Partners list. Click the **Access** subtab, click the **Log in as partner** link.

It's best to let partners set up a NetSuite password for themselves. But if you prefer to assign user passwords yourself, see [Manually Assign a Password to an Advanced Partner Center Role](#subsect_1533243579) instead.

Important:

If you use the Log in as partner link and make changes in your partner's account, NetSuite saves the changes.

### Manually Assign a Password to an Advanced Partner Center Role {#subsect_1533243579}

You should use the procedure in [Assign the Advanced Partner Center Role](#subsect_1533243458) that lets users set up a NetSuite password for themselves. However, if you prefer to assign a user's password yourself, use the following procedure.

#### To manually assign a password:

1.  Go to _Lists > Relationships > Partners_.
    
2.  Click **Edit** next to the user that you want to assign a role to.
    
3.  Click the **Access** subtab.
    
4.  Check the **Give Access** box.
    
    In the **Role** field, **Advanced Partner Center** is selected by default. If you have customized the Advanced Partner Center role for this partner, select the name of that custom role here.
    
5.  Do not check the **Send New Access Notification Email** box.
    
6.  Check the **Manually Assign or Change Password** box.
    
7.  Enter a password for your user. As you type, NetSuite validates the characters against the password policy criteria and displays the results.
    
    Note:
    
    If you need more information, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
8.  Enter the password again for verification.
    
9.  Check the **Require Password Change on Next Login** box to require the user to change the password on the next log in to NetSuite.
    
    On the next log in, users see the Change Password page. Users cannot access other NetSuite pages until they create and save a new password.
    
    This option protects your account from unauthorized access with generic passwords, and prepares your account for an audit.
    
    Important:
    
    The **Require Password Change on Next Login** box never displays with a check mark. When you check this box and save the record, NetSuite sets an internal flag. When the password is changed, the flag clears. If you check the box again and save, NetSuite resets the flag to require another password change.
    
10.  If you want to allow this partner to give access to subpartners, check the **Can Give Login Access to Subpartners** box.
     
11.  When you have finished entering information, click **Save**.
     
12.  Tell your user the appropriate login page, email address to use for log in, and the assigned password. For security reasons, do not email the password.
     
     The NetSuite login page for Partners is `https://system.netsuite.com/pages/customerlogin.jsp` or `https://system.netsuite.com/pages/login.jsp`. Users can enter `system.netsuite.com` in a browser, which resolves to the standard NetSuite login page.
     

Your partner now has access to everything they need without gaining access to anything you don't want them to see. You can use the Partner Activity Summary and Partner Activity Detail reports to view what communication each partner has with customers.

Note:

With the Advanced Partner Center, you can give partners access to specific item records. On each item record, check the **Available in Partner Center** box. This option makes the item available to partners with permission to view, edit or create items. This box is clear by default.

You can customize the Advanced Partner Center role to allow access to any other transactions, records, and reports in NetSuite. Each time you customize the Advanced Partner Center role, you create a new role that you can assign to a partner. Customized Advanced Partner Center roles let you decide which partners can view, edit, or create specific records, transactions, and reports. To learn how to customize a role, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

You can preview what your partner sees by clicking **View** next to the partner record from the Partners list. Click the **Access** subtab, and then the **Log in as partner** link.

Important:

If you use the Log in as partner link and make changes in your partner's account, NetSuite saves the changes.

Note:

The Customize Role page for the Advanced Partner Center has a Partner Restriction field. This field lets you set the general level of access to give to partners. The field is set to **own and subordinates only** by default. If you use classifications, you can also set restrictions for departments, locations, and classes.

You can publish a specialized dashboard to the Advanced Partner Center. This dashboard would be available to all partners with the Advanced Partner Center role, and to all of their contacts. See [Publishing Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N633149.html).

### Related Topics

-   [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html)
-   [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html)
-   [Records as Multiple Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099012.html)
-   [The Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html)
-   [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N1167882"
type: "section"
title: "The Partner Center Role"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Managing Partners > The Partner Center Role"
parent: "chapter_N1166465"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html"
anchors: ["subsect_1533242150", "procedure_1533242319", "subsect_1533243121"]
sha256: "c4c6476e0d30cb7d39b7f07b3c9300ca655c63a7c8119a577f575a3f1c50570f"
---

NetSuite offers a standard Partner Center role for partners. The Partner Center role lets your partners view the Sales by Partner and Sales by Promotion Code reports, partner records and promotion codes. If you use the Partner Commission & Royalties feature, your partners can also view commission reports.

If you use the Advanced Partner Access feature, a Advanced Partner Center role is also available. This role gives partners access to more records, transactions, and reports. For information on the Advanced Partner Center role, see [Assigning the Advanced Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168834.html).

## Assign the Partner Center Role {#subsect_1533242150}

To assign the Partner Center role to a partner, the Partner Access feature must be enabled. An administrator can enable the Partner Access feature at _Setup > Company > Enable Features (Administrator)_. Click the Web Presence subtab. Under the Access section, check the Partner Access box, and then save.

#### To assign the Partner Center role: {#procedure_1533242319}

1.  Go to _Lists > Relationships > Partners_.
    
2.  Click **Edit** on the required partner record.
    
3.  Click the **Access** subtab.
    
4.  Check the **Give Access** box.
    
5.  In the **Role** field, select **Partner Center**.
    
6.  Check the **Send New Access Notification Email** box to inform the user how to access your NetSuite account. The standard user access notification includes the email address to use for logging in to NetSuite. It also contains a URL so that the user can set up a NetSuite password.
    
7.  If you want to allow this partner to give access to subpartners, check the **Can Give Login Access to Subpartners** box.
    
8.  Click **Save.**
    

Now, your partner can access information in your NetSuite account. When your partner logs in, they can update their profile and see reports on sales tied to your partnership.

You can preview what your partner sees by clicking View next to the partner record from the Partners list. Click the **Access** subtab, click the **Log in as partner** link.

Best practice is to let partners set up a NetSuite password for themselves. If you prefer to assign partners' passwords, see [Manually Assign a Password to a Partner](#subsect_1533243121) instead.

Important:

If you use the Log in as partner link and make changes in your partner's account, NetSuite saves the changes.

### Manually Assign a Password to a Partner {#subsect_1533243121}

You should use the procedure in [Assign the Partner Center Role](#subsect_1533242150) that lets users set up a NetSuite password for themselves. However, if you prefer to assign a user's password yourself, use the following procedure.

#### To manually assign a password:

1.  Go to _Lists > Relationships > Partners_.
    
2.  Click **Edit** next to the user that you want to assign a role to.
    
3.  Click the **Access** subtab.
    
4.  Check the **Give Access** box.
    
5.  In the **Role** field, select **Partner Center**.
    
6.  Do not check the **Send New Access Notification Email** box.
    
7.  Check the **Manually Assign or Change Password** box.
    
8.  Enter a password for your user. As you type, NetSuite validates the characters against the password policy criteria and displays the results.
    
    Note:
    
    If you need more information, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
9.  Enter the password again for verification.
    
10.  Check the **Require Password Change on Next Login** box to require the partner to change the password on the next log in to NetSuite.
     
     On the next log in, the partner sees the Change Password page. Partners cannot access other NetSuite pages until they create and save a new password.
     
     This option protects your account from unauthorized access with generic passwords, and prepares your account for an audit.
     
     Important:
     
     The **Require Password Change on Next Login** box never displays with a check mark. When you check this box and save the record, NetSuite sets an internal flag. When the password is changed, the flag clears. If you check the box again and save, NetSuite resets the flag to require another password change.
     
11.  Click **Save**.
     
12.  Tell your user the appropriate login page, email address to use for log in, and the assigned password. For security reasons, do not email the password.
     
     The NetSuite login page for Partners is `https://system.netsuite.com/pages/customerlogin.jsp` or `https://system.netsuite.com/pages/login.jsp`. Partners can enter `system.netsuite.com` in a browser, which resolves to the standard NetSuite login page.
     

### Related Topics

-   [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html)
-   [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html)
-   [Records as Multiple Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099012.html)
-   [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html)
-   [Assigning the Advanced Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168834.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

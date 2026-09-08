---
id: "procedure_N323191"
type: "procedure"
title: "To assign a customer a role and provide access to NetSuite"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Users Overview > Giving Customers Access > Provide Access to Individual Customers > To assign a customer a role and provide access to NetSuite"
parent: "subsect_1536683902"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N323191.html"
anchors: []
sha256: "f2a94277c050c8de563e5743a3cd864ca1f1ba4ab69a11b1f5f751ee9e9f9b2c"
---

1.  Go to _Lists > Relationships > Customers_.
    
2.  Click **Edit** next to the customer that you want to assign a role to.
    
3.  In the **Email** field, enter the customer's email address.
    
    The customer uses this email address to log in to NetSuite.
    
4.  Click the **Access** subtab.
    
5.  Click the **Give Access** box.
    
6.  If you run multiple websites, you can restrict a customer's login access to a specific website (for example, the website that the customer registered on). To assign a customer to a website, in the **Assigned Web Site** field, select a website. For more information, see [Assign Customers to Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1510949098.html).
    
7.  To assign the standard Customer Center role, in the **Role** field, select **Customer Center**. If you customized the Customer Center role, select the name of the custom role. For more on customizing this role, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).
    
8.  Check the **Send New Access Notification Email** box to notify your customer of this new access. As of 2018.2, the new access notification email includes the user's email address (used for logging in to NetSuite), the administrator's email address, and explains login procedures. It also contains a URL so that the customer can set up a NetSuite password. The email containing the link is sent as secure email, and comes from NetSuite `<nlmailer@netsuite.com>`.
    
    Note:
    
    The URL sent in the notification email expires, by default, in 24 hours after sending. A user with the Administrator role can change the number of hours of expiration. For more information, see the Help for the **User Registration Link Expiration In Hours** field at [Setting General Customer Access Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_3131752828.html).
    
    To customize the email message, go to _Setup > Company > System Email Templates_. Next to **Standard Customer Center Access Email**, click **Edit**.
    
9.  To assign individual logins to the customer's contacts, on the **Access** subtab, check the **Access** box next to the contacts you want to grant access to.
    
    Note:
    
    If this is a new customer, you might need to save the record before you can view contacts on the **Access** subtab.
    
    1.  Make sure that an email address is listed for each of the contacts that you want to assign login access to.
        
    2.  Check the Manually Assign Password box and enter a password for each of the contacts.
        
    3.  Check the Notify box for the contacts that you want to notify by email.
        
        For security reasons, the contact's password is not included in the email message.
        
10.  Click **Save**.
     

Important:

To revoke access, you should clear the **Give Access** box. If you want to inactivate all roles of the customer, and the customer is also a vendor, partner, or employee, you must revoke access and inactivate those records, too.

### Related Topics

-   [NetSuite Users Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N321756.html)
-   [Giving Customers Access](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322750.html)
-   [Provide Access to Individual Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1536683902.html)
-   [Set a Customer's Password Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_1531263196.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

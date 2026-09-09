---
id: "section_N1166599"
type: "section"
title: "Creating a Partner Record"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Managing Partners > Creating a Partner Record"
parent: "chapter_N1166465"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html"
anchors: ["procedure_N1166615", "bridgehead_N1166797", "procedure_N1166839", "bridgehead_N1166875", "procedure_N1166891", "procedure_N1166930", "subsect_1533239759"]
sha256: "a1a3c42ce2155d49336f07e3d0c25eba9a7e67bdad6d4df460c5ba37352dd856"
---

You can create partner records for companies and individuals that bring business to your company.

Partners are associated with sales transactions and with new leads, giving you information into your partnerships.

Important:

Don't give access to email addresses or partners you don't recognize. It's also not safe to use generic email addresses like test@test.com.

#### To add a partner record: {#procedure_N1166615}

1.  Go to _Lists > Relationships > Partners > New (Administrator)_.
    
2.  Under Primary Information:
    
    1.  Select the custom form you want to use to create this partner record.
        
        For information on custom forms, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).
        
    2.  To enter the name of this partner:
        
        -   If this partner is a company, enter the name of the partner in the **Company Name** field.
            
        -   If this partner is an individual, enter the name of the partner in the **Name** fields. You can also enter the partner's company in the **Company Name** field.
            
        
        NetSuite uses the name to generate the partner ID in the **Partner ID** field. To enter a partner ID manually, clear the **Auto** box, and then enter the ID.
        
    3.  The **Partner Code** field displays the name entered in the **Partner** field. You can change this code.
        
        When you associate customers with this partner, this code determines what customers see in your website, and what promotion codes they can use.
        
    4.  In the **Type** field, select either Company or Individual.
        
    5.  If this is an individual, enter the partner's job title.
        
    6.  Enter the name of this partner as it should appear on checks made to this partner.
        
    7.  If this partner is a subpartner, select the parent partner in the **SubPartner of** field.
        
    8.  In the **Subsidiary** field, select the subsidiary to associate with this partner.
        
        You cannot enter transactions for this partner until you assign a subsidiary.
        
        This field appears only if you use NetSuite OneWorld.
        
        When you select this partner on a transaction, NetSuite associates the transaction with this subsidiary. The partner can only see info tied to that subsidiary.
        
        Note:
        
        When a transaction posts for this partner, you can't change the subsidiary selected on this partner record.
        
    9.  In the **Category** field, select a category for this partner.
        
        To create new partner categories, go to _Setup > Sales > Setup Tasks > CRM Lists (Administrator)_.
        
    10.  In the **Comments** field, enter information about this partner.
         
3.  Under Email | Phone | Address, enter the phone number, fax number and email address for this partner.
    
4.  Under Classification, enter the department, location, and class associated with this partner.
    
5.  On the **Relationship** subtab, attach a new contact to this record. Enter the contact information, and then click **Add**.
    
    Note:
    
    If you want to attach an existing a contact, you must first save the record.
    

#### Communication {#bridgehead_N1166797}

1.  Use the **Phone Calls**, **Tasks**, and **Events** subtabs to quickly create and add activities associated with this customer.
    
    See [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
    
2.  On the **Files** subtab, select and add files from the File Cabinet associated with this customer.
    
    Select **\-New-** to upload a new file to the File Cabinet.
    
3.  On the **User Notes** subtab, add any notes about this customer.
    

#### Address {#procedure_N1166839}

1.  Enter the partner's address.
    
    For information about entering addresses on records, see [Entering an Address on a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099791.html).
    
2.  Click **Add/Edit** after each address.
    

## Marketing {#bridgehead_N1166875}

In the **Global Subscription Status** field, select the status you want to assign this partner.

If this partner has not subscribed or has unsubscribed to campaigns, set this status to **Soft Opt-In** or **Soft Opt-Out**. You cannot change a status set to **Confirmed Opt-Out**.

Note:

Certain jurisdictions, such as the European Union (EU), have regulations about contacting entities without their explicit permission. Make sure your global subscription status follows the rules in the recipient's country or region.

#### Financial {#procedure_N1166891}

1.  In the **Tax ID** field, enter the partner's tax ID number.
    
2.  If you use the **Partner Commissions/Royalties** feature, check the **Eligible for Commission** box to award commission to this partner.
    
    When you check this box, NetSuite creates a new vendor record for this partner.
    
    See [Partner Commissions & Royalties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1169123.html).
    

#### Preferences {#procedure_N1166930}

1.  In the **Email Preference** field, select the email format you want to use when you send email to this partner.
    
2.  Enter the name as you want it printed on checks made to this partner.
    

If you use the Partner Access feature, you can give a partner access to your NetSuite account. An administrator can enable this feature at _Setup > Company > Setup Tasks > Enable Features (Administrator)_. Click the Web Presence subtab, and under the Access section, check the Partner Access box.

#### Access

1.  Click the **Access** subtab.
    
2.  In the **Role** field, select the role you want to assign.
    
    For information on partner roles, see [The Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html) and [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html).
    
3.  Check the **Give Access** box.
    
4.  Check the **Send New Access Notification Email** box to inform the user how to access your NetSuite account. The standard user access notification includes the email address to use for logging in to NetSuite. It also contains a URL so that the user can set up a NetSuite password.
    
5.  If you want to let this partner give access to its sub-partners, check the **Can Give Login Access to Subpartners** box.
    
6.  Click **Save**.
    
    Note:
    
    After you save the record, you can preview the account. To preview the account, go to the **Access** subtab, and click the **Log in as partner** link.
    
    You can use the preview to ensure the role given to the partner is set up correctly.
    

Best practice is to let users set up a NetSuite password for themselves. If you prefer to assign users' passwords, see [To manually assign a password:](#subsect_1533239759)

Important:

To revoke access, you should clear the **Give Access** box. If you want to inactivate all roles of the partner, and the partner is also a vendor, customer, or employee, you must revoke access and inactivate those records, too.

#### To manually assign a password: {#subsect_1533239759}

1.  Click the **Access** subtab.
    
2.  Check the **Give Access** box.
    
3.  In the **Role** field, select the role you want to assign.
    
    For more information on partner roles, see [The Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html) and [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html).
    
4.  Do not check the **Send New Access Notification Email** box.
    
5.  Check the **Manually Assign or Change Password** box.
    
6.  Enter a password for your user. As you type, NetSuite validates the characters against the password policy criteria and displays the results.
    
    Note:
    
    If you need more information, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
7.  Enter the password again for verification.
    
8.  Check the **Require Password Change on Next Login** box to require the user to change the password on the next log in to NetSuite.
    
    On the next log in, users see the Change Password page. Users cannot access other NetSuite pages until they create and save a new password.
    
    This option protects your account from unauthorized access with generic passwords, and prepares your account for an audit.
    
    Important:
    
    The **Require Password Change on Next Login** box never displays with a check mark. When you check this box and save the record, NetSuite sets an internal flag. When the password is changed, the flag clears. If you check the box again and save, NetSuite resets the flag to require another password change.
    
9.  If you want to let this partner to give access to its sub-partners, check the **Can Give Login Access to Subpartners** box.
    
10.  Click **Save**.
     
     Note:
     
     After you save the record, you can preview the account. To preview the account, go to the **Access** subtab, and click the **Log in as partner** link.
     
     You can use the preview to ensure the role given to the partner is set up correctly.
     
11.  Tell your user the appropriate login page, email address to use for log in, and the assigned password. For security reasons, do not email the password.
     
     The NetSuite login page for Partners is `https://system.netsuite.com/pages/customerlogin.jsp` or `https://system.netsuite.com/pages/login.jsp`. Users can enter `system.netsuite.com` in a browser, which resolves to the standard NetSuite login page.
     

#### System Information

1.  Go to _Lists > Relationships > Partners_ to display list of partners.
    
2.  To see the partners you no longer do business with, check the **Show Inactives** box and then save. This record no longer appears in the Partners list.
    

### Related Topics

-   [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html)
-   [Records as Multiple Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099012.html)
-   [The Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html)
-   [The Advanced Partner Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168130.html)
-   [Assigning the Advanced Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1168834.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

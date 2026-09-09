---
id: "section_N1242506"
type: "section"
title: "Giving Customers Access to Invoices"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Invoicing Billable Customers > Giving Customers Access to Invoices"
parent: "section_N1241287"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242506.html"
anchors: ["procedure_N1242568", "subsect_160692813998", "procedure_N1242681", "subsect_1531424710", "procedure_1531424751"]
sha256: "9d7fba7678f2da4fef06237e24c2b6091f930283f006da5209127db855e58354"
---

Giving customers access to their invoices allows them to view past invoices. If you set up the appropriate preferences, you can also allow your customers to pay their open invoices online.

Follow these steps to give customers access to their invoices.

#### To enable features: {#procedure_N1242568}

1.  Go to _Setup > Company > Enable Features_ (Administrator).
    
2.  Click the **Transactions** subtab.
    
3.  Under Payment Processing, check the **Credit Card Payments** box to let customers pay their invoices online.
    
4.  Click the **Web Presence** subtab.
    
5.  Under Access, check the **Customer Access** box.
    
6.  Click **Save**.
    
7.  Go to _Setup > Accounting > Preferences > Accounting Preference_.
    
8.  Click the **Items/Transactions** subtab.
    
9.  To let customers pay their invoices online, under Payment Processing, check the **Customers Can Pay Online** box.
    
10.  Click **Save**.
     

## Setting Up Access on Customer Records {#subsect_160692813998}

You can use customer records in NetSuite to give access to customers and assign roles.

Check the **Send New Access Notification Email** box to send an email so customers can set up their own NetSuite password. However, if you prefer to set their passwords yourself, use the procedure in [Manually Set a Password](#subsect_1531424710) instead.

#### To set up access on customer records: {#procedure_N1242681}

1.  Go to _Customers > Lists > Customers_.
    
2.  Click **Edit** next to the name of the customer you want to give access to.
    
3.  Under Email | Phone | Address, enter your customer's email address.
    
4.  Click the **Access** subtab.
    
5.  In the **Role** field, select the Customer Center role you want to assign to this customer.
    
6.  Check the **Give Access** box.
    
7.  To let your customer know about their new access, check the **Send New Access Notification Email** box. The email includes their login email address, explains login procedures, and gives them a link to set up their NetSuite password.
    
8.  When you're done, click **Save**.
    

## Manually Set a Password {#subsect_1531424710}

Use the **Send New Access Notification Email** feature to let customers set up a NetSuite password for themselves. However, if you prefer to set their passwords yourself, follow these steps.

#### To manually set a password: {#procedure_1531424751}

1.  Go to _Lists > Relationships > Customers_.
    
2.  Next to the customer to whom you want to assign a role, click **Edit**.
    
3.  In the **Email** field, enter the customer's email address.
    
    The customer uses this email address to log in to NetSuite.
    
4.  On the **Access** subtab, check the **Give Access** box.
    
5.  In the **Role** field, select the Customer Center role you want to assign to this customer.
    
6.  Clear the **Send New Access Notification Email** box.
    
7.  Check the **Manually Assign or Change Password** box.
    
8.  Enter a password for your customer.
    
    Note:
    
    For details about password requirements, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
9.  Enter the password again for verification.
    
10.  When you're done, click **Save**.
     
11.  Next, ask your customer to go to your customer center login page. To find the URL, a user with an Administrator role can go to Setup > Company > Company Information. The URL is in the **Customer Center Login** field. Your customer can log in with the email address and the password you entered on the customer's record. Don't send the customer the password by email.
     

After your customers log in to NetSuite, they can view and pay their invoices.

### Related Topics

-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

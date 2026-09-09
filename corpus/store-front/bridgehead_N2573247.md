---
id: "bridgehead_N2573247"
type: "bridgehead"
title: "Select Email Templates for your Web Site"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Marketing > Communications > Email Management > Website Email Settings > Select Email Templates for your Web Site"
parent: "section_1530697974"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2573247.html"
anchors: ["bridgehead_N2573372", "bridgehead_N2573580", "bridgehead_N2573796", "bridgehead_N2573860", "bridgehead_N2574603", "bridgehead_1511206336"]
sha256: "33789708abac4950e8db30d3440b321143727fdee5abed9bdb1173d64bef297f"
---

Email templates define the content used in your website email.

See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.

On the Web Site Setup page, use the subtabs on the Email tab to set preferences and to choose content for each of the following types of web store email message:

-   [Order Emails](#bridgehead_N2573372)
    
-   [Digital Delivery Email](#bridgehead_N2573580)
    
-   [Other Emails](#bridgehead_N2573796)
    

## Order Emails {#bridgehead_N2573372}

On the Order Emails subtab, you can set preferences for email messages generated at each stage of a web order: Order Received, Order Approved, Order Canceled, and Order Fulfilled. The Order subtab contains a section for each email type and the following procedure applies for all of them.

#### To set preferences for web store order email:

1.  Select the **Send Email** box, to send an email message to customers when an order is received, approved, canceled or fulfilled.
    
    If the shopper is a business customer that has one or more contacts placing orders on its behalf, the email preference **CC Customer on All Emails Related to Orders Placed by Contacts** determines the email addresses to which the order email message is sent. See [Identify Order Creator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542387318.html#subsect_1543853552) for more information.
    
2.  In the **Email From Address** field, enter the email address to use as the email's From address.
    
    Note:
    
    Ensure that you have set up a DKIM key for the domain from which you want to send email. See [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) for more information.
    
3.  If you want to receive copies of the order email messages sent to your customers, select the **Send BCC Emails** box and enter the email address in the following field.
    
    You can enter more than one address separated by a comma.
    
4.  Select the email template you want to use from the **Select a System Email Template** list. If you use multiple languages in your site, you can define multiple language versions in the same email template. See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.
    
5.  (Optional) Click on the Preview icon to see what your email will look like when it's sent. You can preview only those email that are based on system email templates. See [Preview Website Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541438310.html) for information about the preview options available.
    

## Digital Delivery Email {#bridgehead_N2573580}

On the Digital Delivery emails subtab, you can set preferences for email messages generated when a customer orders an item or a gift certificate to download.

#### To set preferences for web store digital delivery email:

1.  Select the **Send Email** box, in the appropriate section, to send an email message to customers.
    
    If the shopper is a business customer that has one or more contacts placing orders on its behalf, the email preference **CC Customer on All Emails Related to Orders Placed by Contacts** determines the email addresses to which the order email message is sent. See [Identify Order Creator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542387318.html#subsect_1543853552) for more information.
    
2.  In the **Email From Address** field, enter the email address to use as the email's From address.
    
    Note:
    
    Ensure that you have set up a DKIM key for the domain from which you want to send email. See [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) for more information.
    
3.  If you want to receive copies of the message sent to your customers when a gift certificate is purchased on your website, select the **BCC Gift Certificate Emails** box and enter the email address in the following field.
    
    You can enter more than one address separated by a comma.
    
    Note:
    
    On the digital delivery subtab, you only have the option to BCC gift certificate email messages.
    
4.  Select the email template you want to use from the **Select a System Email Template** list. If you use multiple languages in your site, you can define multiple language versions in the same email template. See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.
    
5.  (Optional) Click on the Preview icon to see what your email will look like when it's sent. You can preview only those email that are based on system email templates. See [Preview Website Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541438310.html) for information about the preview options available.
    

## Other Emails {#bridgehead_N2573796}

On the Other Emails subtab, you can set up the following email notifications:

-   [Checkout Error Alerts](#bridgehead_N2573860)
    
-   [Web Store Password Recovery Email Messages](#bridgehead_N2574603)
    
-   [Registration Confirmation Email Messages](#bridgehead_1511206336)
    

### Checkout Error Alerts {#bridgehead_N2573860}

You can receive alerts if an order isn't submitted because of an error that occurred at checkout.

Email alerts sent to you, include a ticket number that refers to the error logged in NetSuite. If you receive several alerts, please contact NetSuite Customer Support with these ticket numbers to expedite a resolution.

#### To set preferences for checkout error alerts:

1.  Select the **Send Email** box, to accept email alerts if a customer is unable to submit an order because an error was logged from your website.
    
2.  In the **Email From Address** field, enter the email address to use as the email's From address.
    
    You can use this field to filter the alert messages you receive. For example, this can be useful if you choose to forward error alerts to your mobile phone.
    
    Note:
    
    Ensure that you have set up a DKIM key for the domain from which you want to send email. See [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) for more information.
    
3.  In the **Email To** box, enter the email address where you want to receive web store alert messages. You can enter multiple email addresses separated by commas.
    
4.  Select the email template you want to use from the **Select a System Email Template** list. If you use multiple languages in your site, you can define multiple language versions in the same email template. See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.
    
5.  (Optional) Click on the Preview icon to see what your email will look like when it's sent. You can preview only those email that are based on system email templates. See [Preview Website Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541438310.html) for information about the preview options available.
    

### Web Store Password Recovery Email Messages {#bridgehead_N2574603}

You can customize the password recovery email message delivered when web store customers want to reset the passwords they use to login on your website. By creating a custom email template specifically for password recovery purposes, you can apply the same company branding that you apply to other messages customers receive from your site.

Note:

The password recovery link expires one hour after it's sent.

#### To set preferences for web store password recovery email messages:

1.  Select the **Send Email** box, to send an email message when a customer on your site makes a request to reset a password.
    
2.  In the **Email From Address** field, enter the email address to use as the email's From address.
    
    Note:
    
    Ensure that you have set up a DKIM key for the domain from which you want to send email. See [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) for more information.
    
3.  Select the email template you want to use from the **Select a System Email Template** list. If you use multiple languages in your site, you can define multiple language versions in the same email template. See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.
    
4.  (Optional) Click on the Preview icon to see what your email will look like when it's sent. You can preview only those email that are based on system email templates. See [Preview Website Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541438310.html) for information about the preview options available.
    

## Registration Confirmation Email Messages {#bridgehead_1511206336}

You can set preferences for registration confirmation email messages on the Other Emails subtab of the Web Site Setup page.

#### To set preferences for registration confirmation email messages:

1.  Select the **Send Email** box, to send a registration confirmation email message to customers who sign up on your website.
    
2.  In the **Email From Address** field, enter the email address to use as the email's From address.
    
    If you operate multiple sites, you can enter a different address for each site.
    
    Note:
    
    Ensure that you have set up a DKIM key for the domain from which you want to send email. See [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) for more information.
    
3.  If you want to receive copies of the registration confirmation email message, select the **BCC Registration Confirmation Email** box and enter the email address in the following field .
    
    You can enter more than one address separated by a comma.
    
4.  Select the email template you want to use from the **Select a System Email Template** list. If you use multiple languages in your site, you can define multiple language versions in the same email template. See [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html) for more information.
    
5.  (Optional) Click on the Preview icon to see what your email will look like when it's sent. See [Preview Website Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541438310.html) for information about the preview options available.
    

### Related Topics

-   [Email Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503333654.html)
-   [Set Website Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572962.html)
-   [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html)
-   [Change Email Address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503333705.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

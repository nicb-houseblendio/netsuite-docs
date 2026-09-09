---
id: "section_N993465"
type: "section"
title: "Optimizing Email Campaigns"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Optimizing Email Campaigns"
parent: "chapter_N992514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993465.html"
anchors: ["bridgehead_N993572", "bridgehead_N994500", "bridgehead_N993205", "bridgehead_N993224", "bridgehead_N994575", "bridgehead_N994626"]
sha256: "478a845966a4478df95a6a330e90a2c239ab6e2edc21f2434072c4f0259e7eb2"
---

NetSuite gives your marketing team the tools they need to boost your email deliverability and build your reputation with ISPs as a legitimate marketer.

The NetSuite Marketing Application Terms of Service specifically prohibit the use of email marketing campaigns for sending spam. **Spam is defined as any email that is sent to recipients who don't want to receive it.**

Spam is not restricted to email with inappropriate or harmful content. Spam is defined only by whether the recipient has agreed to receive it. For example, email sent to a list purchased from a third party is considered spam.

You can make sure people who use campaigns irresponsibly don't hurt your legitimate marketing efforts. NetSuite uses criteria to separate appropriate email campaigns from email that might be spam.

Email campaigns that meet the standards for legitimate marketing get sent at a higher priority than those that don't. Additionally, email that meets these characteristics has a higher delivery rate because it's less likely an ISP would consider it spam.

NetSuite email policies abide by the standards set by the Messaging Anti-Abuse Working Group (MAAWG), of which Oracle is a supporting member. For more information, visit [MAAWG's Web site](http://www.maawg.org/home).

These standards apply only to the following types of email in NetSuite:

-   campaign email
    
-   bulk merge email
    
-   email initiated by SuiteScript (by the [N/email Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358552361.html) in SuiteScript 2.x or by the **nlapiSendEmail()** or **nlapiSendFax()** API calls in SuiteScript 1.0)
    

Important:

If you use the UK Edition, NetSuite complies with UK law. NetSuite includes the name of your business address and VAT number in the footer of all email you send to those outside of your company.

In accordance with the CAN-SPAM act, NetSuite campaign email is not sent to email addresses with wireless domains. Recipients whose email addresses have domains that are listed on the [Federal Communications Commission (FCC) Web site](https://www.fcc.gov/consumer-governmental-affairs/domain-name-downloads) won't receive campaign email.

This section provides an overview of how you can maximize the deliverability of your email campaigns.

## Characteristics of Legitimate Campaign Email {#bridgehead_N993572}

Campaign email that abides by our Terms of Service is sent with a higher priority than those that don't meet the criteria below.

Legitimate marketing emails have the following characteristics:

-   Your recipients have opted in to your campaigns. **This is the most important indicator in determining whether an email message is spam.**
    
    For information about opting in to campaigns, see [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html).
    
-   Your campaign recipients have purchased or responded to your campaigns in the past.
    
-   The email uses a campaign email domain.
    
    For information about campaign email domains, see [Campaign Email Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996559.html).
    
-   The email uses DomainKeys Identified Mail (DKIM).
    
    You can use the same domain for both your campaign email and DKIM. For more information, see [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html).
    
-   You've built a positive sender reputation through your previous campaigns.
    
    For more information, see [Developing a Positive Email Sender Reputation](#bridgehead_N994575).
    

## Characteristics of Possible Spam {#bridgehead_N994500}

Emails that don't meet the standards for legitimate marketing get sent with much lower priority.

Email that might be spam has some or all of the following characteristics:

-   The recipients have **not** opted in to the campaign. **This is the strongest indication that a campaign might be spam**.
    
    To make sure your recipients list includes only those who want to receive your email, send campaign subscription invitations. For information about how to have your customers opt in to your campaigns, see [Opt-In Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995837.html).
    
    Note:
    
    Some jurisdictions have regulations regarding whether you can contact entities if you do not have their explicit permission to do so. For example, the European Union (EU). Ensure that you adhere to these regulations when you send both subscription invitations and campaign email.
    
-   You've built a poor sender reputation from past campaigns.
    
-   The recipients haven't bought from you or responded to your past campaigns.
    

To improve the speed at which your email is sent and the rate at which it's delivered, see [Improving the Deliverability of Your Campaign Email](#bridgehead_N994626).

## Campaign Email Limits {#bridgehead_N993205}

If you haven't set up DKIM and an email domain, you're limited to 10,000 messages per campaign.

Your system administrator can set up DKIM and campaign email domains. Your company must first purchase a domain from a domain provider like GoDaddy.com or Network Solutions. DKIM and email domains are required to send more than 10,000 email messages per campaign (email merge), or more than 100,000 bulk email per month.

If you have DKIM set up, there is no limit to the number of email messages you can send in a single merge or campaign. The only limit's the monthly allotment of email messages you have purchased. Email that is sent by NetSuite servers is counted toward your monthly allotment even if it does not reach its target recipient.

Subscription opt-in emails don't count against your monthly email allotment.

## Choosing Email Recipients {#bridgehead_N993224}

After you create your email template, it's time to set up a group of recipients for your marketing campaign. For best results, you should only send email campaign messages to:

-   Customers who've subscribed to your marketing campaigns with a Confirmed Opt-In status.
    
-   Email addresses that aren't on the bounced email list.
    

For more information about how to create a group of recipients, see [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html).

Before you add a customer to a recipient group in NetSuite, make sure you give them a chance to subscribe to your campaigns. Campaigns sent to subscribed customers have a much higher delivery success rate than those who have not explicitly subscribed. NetSuite provides a variety of tools you can use to invite recipients to opt in. For more information about subscriptions, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

Repeatedly sending email to an invalid email address damages your sender reputation. To help with this, NetSuite automatically logs when email messages return hard bounce responses. NetSuite won't send emails to those addresses for a set period of time. For more information, see [Managing Bounced Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869562023.html).

To make sure you only send emails to valid addresses, set a suitable time period for bounced email addresses. Go to _Setup > Marketing > Preferences > Marketing Preferences > Subscription_.

Select the right group of recipients is important in to ensure that your email is delivered quickly and successfully. When you create a target group with search criteria, consider adding the following criteria to the other criteria you use to select your recipients:

-   **Global Subscription Status** is **Confirmed Opt-In**
    
    Send to recipients who have confirmed that they want to receive your email. This is the most important factor to determine if your email meets the Marketing Automation Terms of Service.
    
    You can send email campaigns to recipients with the status of Soft Opt-In. However, your email might not be delivered as quickly or as successfully as it would be to Confirmed Opt-In customers.
    
-   Bounced is **false**.
    
    If you use the **Remove email addresses from Bounced Email Addresses list** preference, these email addresses are not sent email. However, when you add this criterion you do not incur a charge for these messages.
    
-   **Campaign Response Fields: Campaign Response Filter: Response** is none of **Failed: spam**
    
    This criterion filters recipients who have flagged your email as spam.
    

Careful management of your recipient lists improves your campaigns' performance, and it also creates trust between you and those with whom you do business. For more information about creating searches, see [Search Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N635877.html).

## Developing a Positive Email Sender Reputation {#bridgehead_N994575}

NetSuite uses your email history to determine whether your email meets best practice criteria. This includes:

-   The percentage of campaign email that is replied to.
    
-   The percentage of email sent to invalid email addresses.
    
-   The percentage of your campaign email that leads to spam complaints from recipients and ISPs.
    
-   The purchase and response history of recipients.
    

When you maintain a positive sender reputation, your email campaigns receive faster delivery.

## Improving the Deliverability of Your Campaign Email {#bridgehead_N994626}

If you want your email sent at the optimal rate of delivery, you should do the following:

-   **Invite recipients to opt in to your campaigns**.
    
    You can send campaigns to recipients with the Soft Opt-In status. However, letting recipients subscribe can increase the deliverability of your email.
    
    You can invite your customers to opt in by going to _Campaigns > Other > Mass Updates_. Under the Marketing heading, select the Send Subscription Message update you want to perform. For more information, see [Opt-In Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995837.html).
    
-   Only send campaign email to customers who have purchased from you or responded to prior campaigns. For tips on creating recipient groups, see [Choosing Email Recipients](#bridgehead_N993224).
    
-   Set up a campaign email domain.
    
-   Set up domain key identified mail (DKIM).
    

### Related Topics

-   [Opt-In Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995837.html)
-   [Campaign Email Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996559.html)
-   [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html)
-   [Using the Sent Email List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156569944168.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

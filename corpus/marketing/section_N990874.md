---
id: "section_N990874"
type: "section"
title: "Bounced Email"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Managing Campaigns > Campaign Metrics > Bounced Email"
parent: "section_N990085"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990874.html"
anchors: ["bridgehead_3886922433", "bridgehead_3886922684"]
sha256: "843f3528af9e44bb0abdfa796efba42ce6b0a15b93be9bcb0039b3f8e8584afd"
---

There are several reasons why an email message might not be delivered, or bounce. Some are temporary and result in soft bounces. Others can be the result of permanent issues and result in hard bounces. A hard bounce generates the **Failed - invalid address** campaign response.

Note:

If an email address generates a **hard bounced** response, NetSuite restricts its inclusion in subsequent campaigns for 30 days or 90 days. The day length depends on whether DKIM and an email domain are set up. Attempts to send to the bounced address before the time elapses results in an unsent message, and the campaign response: **Failed - invalid address**.

You can access all saved searches from Lists > Search > Saved Searches. The following saved searches are available to assist administrators who work with bounced emails:

-   You can also access the Sent Email List from Setup > Company > Communication > Sent Email List. See [Using the Sent Email List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156569944168.html).
    
-   You can also access the Undelivered Emails from Lists > Mailing > Undelivered Emails. See [Managing Bounced Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869562023.html).
    
-   The Bounced Email Addresses list is more inclusive. See [Viewing the Bounced Email Address List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3884410517.html).
    

## Hard Bounce Reasons {#bridgehead_3886922433}

-   Unknown User
    
-   Bad Domain
    
-   Address Error
    
-   Account Closed
    
-   Receiver Error
    
-   Hard Bounced - Other (used when unable to determine one of the five preceding reasons)
    

## Soft Bounce Reasons {#bridgehead_3886922684}

-   Mailbox Full
    
-   Disabled Account
    
-   Greylisted
    
-   Server Too Busy
    
-   Soft Bounce - Other (used when unable to determine one of the four preceding reasons)
    

For information about excluding email addresses that returned hard bounce responses, see [Choosing Email Recipients](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993465.html#bridgehead_N993224).

### Related Topics

-   [Email Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993117.html)
-   [Tracking Campaign Responses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990539.html)
-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N994827"
type: "section"
title: "Subscription Management"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Subscription Management"
parent: "chapter_N992514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html"
anchors: ["bridgehead_4448349320"]
sha256: "c20bf75279545933ba86b6e7a1051a29ad46db1eb23f0716483de750994d207a"
---

NetSuite provides you with the tools you need to manage the email preferences of those with whom you do business.

Every email you send through campaigns or bulk email merges includes a footer with a link and instructions to unsubscribe. For more information, see [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html).

Email recipients can have one of four subscription statuses:

-   **Confirmed Opt-In**: When an email recipient subscribes to your marketing campaigns or bulk email merge operation, NetSuite assigns this subscription status. Only a lead or customer can set their subscription status to **Confirmed Opt-In**. For more information, see [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html).
    
    Getting recipients to opt in leads to better and faster delivery because ISPs are less likely to mark these messages as spam.
    
-   **Soft Opt-In**: Recipients with this status receive all email marketing campaigns or bulk emails received by recipients with the **Confirmed Opt-In** status. They also receive opt-in messages that enable them to confirm whether they want to receive the email campaigns or bulk emails.
    
    Recipients can't set their own status to **Soft Opt-In**. You can set this status in NetSuite manually or with a mass update.
    
-   **Soft Opt-Out**: Soft Opt-Out: Recipients with this status don't get campaign or bulk emails, but they do get opt-in messages.
    
    You can change this subscription status to **Soft Opt-In** manually or through a mass update. If you set a recipient's status to **Soft Opt-Out**, NetSuite unsubscribes them from all subscription categories.
    
-   **Confirmed Opt-Out**: Only the recipient can set their subscription status to **Confirmed Opt-Out**.
    
    Recipients with this status don't receive email campaigns, bulk emails, or opt-in messages. Recipients with this status can opt in again through the Customer Center or by clicking the link in a campaign message they got before opting out.
    

| Status | Receive campaigns? | Receive opt-in message? | Set by |
| --- | --- | --- | --- |
| Confirmed Opt-In | **yes** | **yes** | recipient only |
| Soft Opt-In | **yes** | **yes** | manual or mass update |
| Soft Opt-Out | no | **yes** | manual or mass update |
| Confirmed Opt-Out | no | no | recipient only |

You can set new records to one of the soft statuses when you create them manually or with a CSV import, but you can't set confirmed statuses this way.

Note:

Certain jurisdictions have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. For example, the European Union (EU). You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.

NetSuite tracks subscription status in the **Global Subscription Status** field on each record. This field is located in the Subscriptions subtab of the Marketing subtab. The Subscription Message History subtab contains information about all subscription invitation and confirmation email messages sent to the entity after June 2018.

You can set the default global subscription status at _Setup > Marketing > Preferences > Marketing Preferences_.

If you use the Duplicate Detection and Merge feature, when you merge two records, NetSuite maintains the subscription statuses from the primary record on the final merged record.

To begin managing campaign subscriptions, see [Setting Up Campaign Subscriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995376.html).

## Creating Subscriber Lists Using Saved Searches {#bridgehead_4448349320}

You can use search filters to track your campaign subscriptions and build mailing lists you can export. NetSuite uses saved searches to build these lists, and lists can apply to both customers or contacts. A list of the most commonly used filters is as follows. For more information about creating saved searches, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).

| Filter | Options | Comments |
| --- | --- | --- |
| Global Subscription Status | Soft Opt-In Soft Opt-Out Confirmed Opt-In Confirmed Opt-Out | Refine your list to target the more receptive (confirmed opt-in) customers. |
| Inactive | Either, Yes, No | Set to No to only search for active customers or contacts. |
| Subscription | Select item from Campaign Subscriptions list. | First enable Subscription Categories, at _Setup > Company > Enable Features_. |
| Subscription Status | Either, Yes, No | Set to Yes and use with subscription filter to return positive instances of that Campaign Subscription. |

When you set up the saved search, you can export the search results in the required format. Supported formats include CSV, Excel, and PDF.

### Related Topics

-   [Setting Up Campaign Subscriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995376.html)
-   [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html)
-   [Opt-In Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995837.html)
-   [Sending Subscription Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996083.html)
-   [Campaign Subscription Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996344.html)
-   [Mass Updates of Global Subscription Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N672926.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

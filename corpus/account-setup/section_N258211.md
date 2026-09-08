---
id: "section_N258211"
type: "section"
title: "Setting Up Duplicate Detection"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Setting Up Duplicate Detection"
parent: "chapter_N239909"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html"
anchors: []
sha256: "1d5903aeb62e38e4d7524b3a0991fc8b3440f47d9026bea21bd6fc219a01efb8"
---

After you enable the Duplicate Detection feature at _Setup > Company > Enable Features_, you need to set the criteria for finding duplicates before records can be flagged. By default, NetSuite looks for duplicates by email address.

You can change how NetSuite searches for duplicates on the Duplicate Detection page. You can have NetSuite search for duplicates among customer, contact, partner, or vendor records and look for matches in certain fields.

Go to _Setup > Company > Duplicate Detection_.

Note:

You may have to scroll down the Company menu to see Duplicate Detection in the Company Management section.

The following topics describe the duplicate preferences on each subtab of the Set Up Duplicate Detection page.

-   [Duplicate Detection Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N258228.html)
    
-   [Duplicate Detection Excluded Domains Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1126080506.html)
    
-   [Duplicate Detection Other Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1126080527.html)
    

Use the Duplicate Entity Management permission to specify which users can access the Manage Record Duplicates page. For more information, see [Duplicate Entity Management Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491767.html).

After you set the duplicate detection preferences, NetSuite starts searching for duplicate records based on your criteria.

Note:

The initial search can take some time, depending on how many customer and contact records you have in your account. You won't see duplicate alerts or be able to merge records until this first search is done.

After the search is complete, possible duplicate records are flagged with a notice and a link to a page where you can decide how to handle them. For more information, see [Duplicate Record Notification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N258370.html) and [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html).

You can only merge records if they have the same tax registration number or if neither record has a tax registration numbers entered. This restriction prevents you from merging records that aren't duplicates. If you use NetSuite OneWorld, you can't merge records with different subsidiaries.

Note:

Merging records also merges their transaction histories. The original data, such as entity name, is retained to preserve a transaction's history. You should limit who can merge records to specific roles or to a user with the Administrator role. This is particularly important if audit requirements discourage merging transaction records.

You can also go to _Lists > Mass Update > Entity Duplicate Resolution_ to search for all possible duplicate contact and customer records based on the criteria you've set.

### Related Topics

-   [NetSuite Company Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N239909.html)
-   [Change Record and Transaction Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252023.html)
-   [Setting Printing and Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253916.html)
-   [NetSuite Account Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1487792254.html)
-   [Activating System Alert Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258424.html)
-   [Searching Bulk Processing Jobs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495464846.html)
-   [Administrative Notification Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258657.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

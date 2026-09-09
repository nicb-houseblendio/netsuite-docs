---
id: "section_N2877583"
type: "section"
title: "Enabling Optimistic Locking for Custom Records"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Defining Search and Edit Settings > Enabling Optimistic Locking for Custom Records"
parent: "section_1501859705"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2877583.html"
anchors: []
sha256: "b09acf6c87d5204415ff9846e027c0177a26dfa07ba79372f3dd42c770bbf3ef"
---

Each custom record type has a Enable Optimistic Locking option that can be enabled to protect custom record data integrity.

![Sample Custom Record Type record with Enable Optimistic Locking box highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/PrevConflictUpdates.png)

Important:

Optimistic locking prevents concurrent updates of custom record entries. This includes updates done by a single user (or script) if they're done in concurrent manner (for example, through two browser tabs).

Be aware that when you update a parent record, the child records associated with this parent may also update. If the child record has enabled optimistic locking, an error will appear if you try to concurrently update the child record entry and its parent.

Enabling this option causes the system to check for conflicting updates whenever a user or script attempts to save updates to an instance of this custom record type. If another user, script, or action has saved updates to the same custom record instance during the time that the first user, script, or action was entering updates, one of the following message is returned:

-   "Record has been changed."
    
-   'Unable to save record. Record was changed by a different user. Please reload and try again.'
    

The Enable Optimistic Locking option is enabled by default for all custom record types created as of 2012.2 and later. For backward compatibility, this option is disabled by default for custom record types created prior to 2012.2. You should enable this option, but first review any scripts that may be affected by this change and edit them as needed.

This support for optimistic locking makes custom records' concurrency control consistent with the optimistic locking used generally for NetSuite standard records. Optimistic locking assumes that multiple concurrent transactions can usually complete without affecting each other, so data resources don't have to be locked during the time that transactions are in process. Instead, a check for conflicts occurs before each transaction is committed. For more information about optimistic locking, you can review a related article at [http://en.wikipedia.org/wiki/Optimistic\_concurrency\_control](http://en.wikipedia.org/wiki/Optimistic_concurrency_control).

### Related Topics

-   [Defining Search and Edit Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859705.html)
-   [Defining Hierarchies among Custom Record Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4362612928.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

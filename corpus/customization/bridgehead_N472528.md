---
id: "bridgehead_N472528"
type: "bridgehead"
title: "Sublists and Subtabs"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Form Layout Enhancements > Sublists and Subtabs"
parent: "section_N472127"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html"
anchors: ["bridgehead_163553051053", "bridgehead_N472930"]
sha256: "7866cc27b511e064234e6bc207f6ef2069e170df98ac1d2e3f3870c0d566740b"
---

After administrators deploy a form with the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) applied, the subtabs and sublists that appear on the form will change. End users will notice that new subtabs and sublists have been added. For more information, see [Added Subtabs and Sublists](#bridgehead_163553051053). They will also notice that certain subtabs and sublists have been removed. For more information, see [Removed Subtabs and Sublists](#bridgehead_N472930).

The subtab and sublist changes associated with the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) were implemented by NetSuite to create more consistency across the application. Across all records, subtabs and sublists now have a more consistent pattern of naming and placement.

## Added Subtabs and Sublists {#bridgehead_163553051053}

If you are viewing forms with the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) applied, you will notice that the following subtabs have been added:

-   **Access** (appears on all entity records when the record is in View or Edit mode)
    
-   **Accounting** (appears on certain entity, item, and transaction forms)
    
-   **Billing** (appears on certain transaction forms)
    
-   **Builds** (appears on certain transaction forms)
    
-   **Communication** (appears on certain entity, item, and transaction forms and will contain these subtabs in a consistent order)
    
    -   Messages (appears when record is in View or Edit mode)
        
    -   Activities (appears when record is in View or Edit mode)
        
    -   Events (appears when record is in New)
        
    -   Tasks (appears when record is in New)
        
    -   Calls (appears when record is in New)
        
    -   Files
        
    -   User Notes
        
    -   Bulk Merge (often hidden by default)
        
-   **Fulfillments and Credits** (appears on certain transaction forms)
    
-   **Fulfillments and Receipts** (appears on certain transaction forms)
    
-   **Journal** (appears on certain transaction forms)
    
-   **Locations** (appears on certain item forms)
    
-   **Message** (appears on certain CRM forms)
    
-   **Preferences** (appears on certain entity and item forms)
    
-   **Purchasing / Inventory** (appears on certain item forms)
    
-   **Receipts and Refunds** (appears on certain transaction forms)
    
-   **Relationships** (appears on certain entity and transaction forms and will contain all entities associated with the primary record. The entities appearing on this subtab will vary depending on the primary record you are on.)
    
-   **Related Records** (appears on certain entity, item, CRM, and transaction forms, and will contain transactions and other records associated with the primary record. The records appearing on this subtab will vary depending on the primary record you are on.)
    
-   **Sales** (appears on certain transaction forms)
    
-   **Subscriptions** (appears on certain entity forms)
    
-   **System Information** (appears on certain entity, item, CRM, and transaction forms, and will contain these subtabs in a consistent order)
    
    -   System Notes (appears when record is in View or Edit mode)
        
    -   Workflow
        
    -   Translation (appears only on certain items)
        
-   **Time Tracking** (appears on some entity records)
    
-   **Vendors** (appears on some item records)
    
    Important:
    
    Be aware that the Date Created field and the Inactive field both appear on the System Information subtab after the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) have been deployed to your account.
    

## Removed Subtabs and Sublists {#bridgehead_N472930}

If your account administrator has not yet deployed [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) to your account, you will notice that there are no changes to the organization of the fields or subtabs on a page.

However, if you are viewing forms with the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) applied (meaning that your account administrator has deployed the upgraded forms to your account), you will notice the following subtabs have been removed:

**Entity Forms:**

-   General
    
-   Info
    

**Item Forms:**

-   Basic
    
-   History
    
-   Rev Rec / Amort (note: subtab fields have been moved to the Revenue Recognition / Amortization subtab)
    
-   Specials (the fields on this subtab are moved to the Web Store subtab when you deploy the upgraded form)
    

**CRM Forms:**

-   General
    
-   History
    

**Transaction Forms:**

-   Carrier
    
-   General
    
-   History
    
-   International
    
-   Packages
    
-   Revenue (the fields on this subtab are moved to the new Accounting subtab when you deploy the upgraded form)
    

**Other subtabs not removed but relabeled:**

-   Related Info (CRM forms) relabeled to Related Records
    

Fields that used to reside on these subtabs have been moved to new locations on the form or to another subtab.

Important:

If you are a SuiteScript developer and you have referenced any of these unsupported tabs in your scripts, you will need to modify your scripts to reference existing subtabs. Note that the IDs for all new subtabs are provided in the SuiteScript Records Browser.

### Related Topics

-   [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html)
-   [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

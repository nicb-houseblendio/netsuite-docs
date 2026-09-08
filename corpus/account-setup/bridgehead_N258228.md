---
id: "bridgehead_N258228"
type: "bridgehead"
title: "Duplicate Detection Preferences"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Setting Up Duplicate Detection > Duplicate Detection Preferences"
parent: "section_N258211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N258228.html"
anchors: ["procedure_N258240", "subsect_1126085742"]
sha256: "af9009e471aa17c36a9de0fc880ad867555477993455ffc46b6761b01b5d9ef0"
---

On the **Detection** subtab, you set the criteria for marking records as duplicates, such as which records and fields to check.

#### To set duplicate detection preferences: {#procedure_N258240}

1.  Go to _Setup > Company > Duplicate Detection_.
    
2.  Click the **Detection** subtab.
    
3.  Check **Near Match Detection** to help identify duplicates based on similar but not exact match criteria. This preference may improve duplicate detection by catching duplicates created from misspellings, typos and other minor variations in data.
    
    Note:
    
    This preference is available to customers whose accounts use Latin or Cyrillic characters only.
    
    When potential duplicates are detected, you see a notification banner highlighting records that could be merged into one entity record.
    
    Clear the box at any time to revert to exact match detection.
    
4.  Check the **Detect Duplicates Across Subsidiaries (Customers and Vendors Only)** box to search for duplicate customers and vendors, even if they are in different subsidiaries.
    
5.  Check the box next for each type of record you want to use duplicate detection with.
    
    For example, check the **Detect Customer Duplicates** box to get alerts for possible duplicate customer records.
    
    There are four types of records you can detect duplicates for:
    
    -   Customer
        
    -   Vendor
        
    -   Partner
        
    -   Contact
        
6.  In the **Fields to Match On** field, select the fields from the record type you want to use when searching for similar information.
    
    Select the **Company Name** field for a customer record type to look for duplicate matches in the **Company Name** field.
    
    Depending on your settings in _Home > Set Preferences_, you may see all fields listed in the form, or you may have to click the Select Multiple icon ![Select Multiple icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/AccountSetup/icon_SelectMultiple_2014_2.png), and select your fields from there.
    

## Notes on the Fields To Match On Preferences {#subsect_1126085742}

-   Records have to match in **all** the fields you select to be returned as possible duplicates.
    
    For example, you check the **Detect Customer Duplicates** box and then select phone and email in the **Fields to Match On** field. Customers need to have both a matching phone number **and** email address to be considered duplicates.
    
-   You can base duplicate detection criteria on custom fields. The list of fields for each entity type includes any custom fields you've created for those record types. Check the **Store Value** box when creating a custom entity field to make it available as criteria in duplicate detection.
    
-   Duplicate detection doesn't support the following entity custom field types: Time Of Day, Rich Text, Password, and Date/Time. These fields don't appear in the **Fields to Match On** field.
    

### Related Topics

-   [Setting Up Duplicate Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html)
-   [Duplicate Detection Excluded Domains Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1126080506.html)
-   [Duplicate Detection Other Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1126080527.html)
-   [Duplicate Entity Management Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491767.html)
-   [Duplicate Record Notification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N258370.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

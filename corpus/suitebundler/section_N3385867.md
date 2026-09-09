---
id: "section_N3385867"
type: "section"
title: "Sharing a Bundle"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Bundle Availability > Sharing a Bundle"
parent: "section_N3385668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html"
anchors: ["procedure_N3385906"]
sha256: "4225b2d456b7c13179a58a79c7b3c43188454d9ad2b177b4d9ad41e41914144c"
---

New bundles are private by default, accessible only to accounts where you're an administrator. You can choose to share a bundle with a selected list of accounts or make it publicly available to all NetSuite accounts.

For shared and publicly available bundles, you can also indicate whether the bundle is visible in basic search results for all users, including those who do not have access to install the bundle.

Note:

Only administrators and users with the SuiteApp Marketplace permission can share bundles.

#### To share a bundle: {#procedure_N3385906}

1.  Go to _Customization > SuiteBundler > Create Bundle > List_.
    
2.  In the **Action** list for the bundle you want to share, click **Set Availability**.
    
3.  On the Bundle Availability page, choose a value for the **Level** field:
    
    -   **Private** - A private bundle is only accessible to other accounts to which you have administrator access. This is useful during development and testing, before you are ready to share the bundle with others.
        
        It is a best practice that bundles in sandbox or other development accounts have a **Level** of **Private**.
        
        The **Visible By All** option is disabled and cannot be edited for a private bundle.
        
    -   **Shared** - Administrators of accounts that you list in the **Shared Account IDs** field can view and install a shared bundle from a deployment account if the bundle is copied there.
        
        If **Visible By All** is checked, all users can see the bundle in search results. This visibility advertises the bundle to users who do not have install access and enables users with install access to find the bundle, as they do not need to know an account ID.
        
    -   **Public** - Any NetSuite administrator can view and install a public bundle from a deployment account if the bundle is copied there.
        
        If the **Visible By All** box is checked, all users can view the bundle in basic search results, so they do not need to know an account ID to install the bundle.
        
    
    Important:
    
    You cannot make a configuration bundle public.
    
4.  If you have set the **Level** to **Shared**, enter the account IDs of the NetSuite accounts with which you want to share your bundle.
    
    You can find your NetSuite account ID at the beginning of the NetSuite URL. For example, if the URL is https://1234566.app.NetSuite.com/, your account ID is 1234567. Account IDs are typically 6 or 7 digits. You can separate account IDs with commas.
    
5.  If you have set the **Level** to **Shared** or **Public**, you can clear the **Visible By All** box if you do not want the bundle to be returned in basic search results.
    
    -   If this option is enabled, the bundle is visible in all users' basic search results, which for shared bundles, includes users who do not have access to install the bundle.
        
    -   If this option is disabled, the bundle is not returned in basic search results. Users with install access can find the bundle using an advanced search.
        
6.  Click **Save**.
    

Note:

A bundle that is shared with a production account is automatically shared with the first sandbox account associated with that production account because the two accounts share an ID. However, you must explicitly share the bundle with any additional sandbox accounts associated with that production account because they have different account IDs.

### Related Topics

-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
-   [Implementing Phased Updates by Setting Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3387345.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

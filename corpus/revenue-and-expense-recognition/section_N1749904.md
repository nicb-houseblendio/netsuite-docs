---
id: "section_N1749904"
type: "section"
title: "How Can I Get This Feature?"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > How Can I Get This Feature?"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html"
anchors: ["bridgehead_N1749943", "procedure_N1750080", "procedure_N1750116", "procedure_N1750172", "procedure_N1750363", "procedure_N1750460"]
sha256: "5afc8cd8dc1040df447ff2634b53e482bd0f0c94b1159938cd002c3b5e2f71b9"
---

EITF 08-01 Revenue Recognition is a managed SuiteApp created by NetSuite. After you install this SuiteApp, NetSuite automatically upgrades the SuiteApp when changes are available. For information about managed SuiteApps, see [Using Managed Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3400741.html).

Contact your account manager for information about how to purchase this feature. Professional Services can assist you with implementation.

If you're upgrading a previous EITF 08-01 bundle version, see [Upgrading EITF 08-01 Bundle Version](#bridgehead_N1749943) for instructions on how to correctly install the bundle.

## Upgrading EITF 08-01 Bundle Version {#bridgehead_N1749943}

If you're upgrading from an earlier bundle version, your current bundle version determines what you need to do to install the latest EITF 08-01 Revenue Recognition SuiteApp (Bundle ID: 29321).

Important:

You should work with NetSuite Account Management and Professional Services to guarantee a smooth upgrade.

-   If your current EITF 08-01 installation consists of bundles 8406 and 8407, update bundle 8407 to install bundle 29321. See [To install bundle 29321:](#procedure_N1750116)
    
-   If your current EITF 08-01 installation consists of bundles 9511, 8406, and 8407, complete the following to upgrade to EITF-08-01 Platform Feature Bundle 29321:
    
    -   Uninstall bundle 9511. See [To uninstall bundle 9511:](#procedure_N1750080)
        
    -   Upgrade bundle 8407 to bundle 29321. See [To install bundle 29321:](#procedure_N1750116)
        
    -   Configure the following bundle components:
        
        -   [To add fields to the Multiple Allocation Price List:](#procedure_N1750172)
            
        -   [To change preference name for Transaction is Allocation Bundle:](#procedure_N1750363)
            
        -   [To add Quantity Internal ID preference:](#procedure_N1750460)
            

#### To uninstall bundle 9511: {#procedure_N1750080}

1.  Go to Customization > SuiteBundler > Search & Install Bundle > List.
    
2.  From the **Action** dropdown for bundle 9511, select **Uninstall**.
    
3.  In the confirmation popup, click **OK**.
    

#### To install bundle 29321: {#procedure_N1750116}

1.  Go to Customization > SuiteBundler > Search & Install Bundle > List.
    
2.  From the Action dropdown for bundle 8407, select **Update**.
    
3.  On the Preview Bundle Update page, select **Update and Preserve Data** under Action for the following:
    
    -   EITF 08-01 M/S Models
        
    -   Item Categories \[R\]
        
4.  Click **Install Bundle**.
    

#### To add fields to the Multiple Allocation Price List: {#procedure_N1750172}

1.  Go to Customization > Lists, Records, & Fields > Record Types.
    
2.  Click **Multiple Allocation Price**.
    
3.  On the **Fields** subtab, click **New Field** and add the **ESP Price % Lower Limit** field:
    
    1.  Label: ESP Price % Lower Limit
        
    2.  ID: custrecord\_e81\_esp\_lower. **Note:** Type only '\_e81\_esp\_lower', 'custrecord' is automatically generated.
        
    3.  Type: Percent
        
    4.  Check the **Store Value** and the **Show in List** boxes.
        
    5.  On the **Validation & Defaulting** subtab, check the **Mandatory** box and enter 0.0% for Default Value.
        
    6.  Click **Save**.
        
4.  Click **New Field** and add the **ESP Price % Upper Limit** field:
    
    1.  Label: ESP Price % Upper Limit
        
    2.  ID: custrecord\_e81\_esp\_upper
        
    3.  Type: Percent
        
    4.  Check the **Store Value** and **Show in List** boxes.
        
    5.  On the **Validation & Defaulting** subtab, check the **Mandatory** box and enter 0.0% for Default Value.
        
    6.  Click **Save**.
        
5.  Click **New Field** and add the **IsVSOE** field:
    
    1.  Label: IsVSOE
        
    2.  ID: custrecord\_e81\_esp\_isvsoe
        
    3.  Type: Check Box
        
    4.  Check the **Store Value** and the **Show in List** boxes.
        
    5.  On the **Validation & Defaulting** subtab, check the **Mandatory** box.
        
    6.  Click **Save**.
        

#### To change preference name for Transaction is Allocation Bundle: {#procedure_N1750363}

1.  Go to Customization > Lists, Records, & Fields > Record Types.
    
2.  Enable display for Preference Name:
    
    1.  On the Record Types page, click **EITF-08-01 Preferences**.
        
    2.  On the **Fields** subtab, click **Preference Name**.
        
    3.  On the **Display** subtab, change Display Type to **Normal**.
        
    4.  Click **Save**.
        
3.  Change the preference name of Transaction is Allocation Bundle:
    
    1.  On the Record Types page, click the **List** link for **EITF-08-01 Preferences**.
        
    2.  Click **Edit** next to Transaction is Allocation Bundle.
        
    3.  Change the Preference Name to **Transaction is EITF-08-01**.
        
    4.  Click **Save**.
        
4.  Disable display for Preference Name:
    
    1.  On the Record Types page, click **EITF-08-01 Preferences**.
        
    2.  On the **Fields** subtab, click **Preference Name**.
        
    3.  On **Display** subtab, change Display Type to **Disabled**.
        
    4.  Click **Save**.
        

#### To add Quantity Internal ID preference: {#procedure_N1750460}

1.  Go to Customization > Lists, Records & Fields > Record Types.
    
2.  Enable display for **Preference Name**, **Preference Script ID**, and **Preference Field ID**:
    
    1.  On the Record Types page, click **EITF-08-01 Preferences**.
        
    2.  On the **Fields** subtab, click **Preference Name**.
        
    3.  On the **Display** subtab, set Display Type to **Normal**, and then click **Save**.
        
    4.  Repeat the steps for **Preference Script ID** and **Preference Field ID**.
        
3.  Add a new preference for EITF-08-01 Preferences:
    
    1.  On the Record Types page, click New Record for **EITF-08-01 Preferences**.
        
    2.  Add a new preference with the following information:
        
        -   Preference Name: Quantity Internal ID
            
        -   Preference Value: quantity
            
        -   Preference Script ID: custscript\_eitf81\_cs\_item\_qty\_id
            
        -   Preference Field ID: custpage\_eitf81\_cs\_item\_qty\_id
            
    3.  Click **Save**.
        
4.  Disable display for **Preference Name**, **Preference Script ID**, and **Preference Field ID**:
    
    1.  On the Record Types page, click **EITF-08-01 Preferences**.
        
    2.  On the **Fields** subtab, click **Preference Name**.
        
    3.  On the **Display** subtab, set Display Type to **Disabled**, and then click **Save**.
        
    4.  Repeat the steps for **Preference Script ID** and **Preference Field ID**.
        
5.  Click **Save**.
    

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [EITF 08-01 Allocation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

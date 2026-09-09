---
id: "section_N1746357"
type: "section"
title: "Implementing EITF 08-01 Revenue Recognition"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > Implementing EITF 08-01 Revenue Recognition"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html"
anchors: ["procedure_N1746438", "bridgehead_N1746607", "procedure_N1746621", "bridgehead_N1746683", "bridgehead_N1746774", "procedure_N1746809", "procedure_N1746857", "procedure_N1746934"]
sha256: "b9f6e4e52e1d49504596bbe69dc08bc25d92d822f337332276445c4369b4abea"
---

Important:

EITF 08-01 Revenue Recognition is a managed SuiteApp (Bundle ID: 29321).

Use the EITF 08-01 Assistant to set up the custom records used to calculate and track multiple estimated selling prices for items you sell. You also use the Assistant to establish the Multiple Allocation Prices list and to set the date you'll begin calculating EITF 08-01 price allocations.

The EITF 08-01 Assistant guides you through the following setup areas:

-   Multiple Allocation Price Definition
    
-   Multiple Allocation Price Dimensions
    
-   Formulas based on Item Categories
    
-   EITF 08-01 Preferences
    
-   Confirmation
    

#### To set up custom records for allocation: {#procedure_N1746438}

1.  Go to Setup > Custom > EITF 08-01Assistant.
    
2.  By default, there are two required dimensions for revenue allocation: ESP Item and ESP Price. Enter the number of additional dimensions you want to create. Enter at least one, and then click **Next**.
    
3.  For each dimension you add, enter a label and a description. Select the type of dimension and specific list or record.
    
4.  Set the item category formula for each calculation that you use. You can modify the seeded formula during setup or at any time.
    
    Formulas available are: License-Perpetual, License-Term, Maintenance/Support, Services, Training, Hardware, and Other. Click **Next**.
    
    Note:
    
    Maintenance/Support is abbreviated as M/S in preferences and other settings.
    
5.  Set the EITF 08-01 preferences. Enter the date to start calculating allocations.
    
    In the **Maintenance/Support** field, select the revenue model for Maintenance/Support items:
    
    -   **Itemized M/S Price** - The revenue amount is calculated based on the unit price and the number of deliverable units.
        
        Important:
        
        When the **Itemized M/S Price Model** is selected, by default the Maintenance/Support item category formula sets to the License - Term formula. You can change this formula in each custom record of the Maintenance/Support item category formulas after setup at Customization > Lists, Records & Fields > Record Types > EITF Item Category Formulas List > Edit EITF Item Category Formulas (see [Modifying Implementation Settings](#bridgehead_N1746607)). Note that {CUSTOME81MSPERCENT} is only valid for **M/S as a % of License** formulas.
        
    -   **M/S as a % of License** - The revenue amount is calculated as a percentage of the license revenue. If selected, complete the following fields with the required values:
        
        -   **M/S as a % of License File ID** - Enter the ID for the file used to calculate M/S as a % of License.
            
        -   **M/S as a % of License Function Name** - Enter the name of the server-side function used to calculate M/S as a % of License.
            
        -   **M/S as a % of License Client Function Name** - Enter the name of the client-side function used to calculate M/S as a % of License.
            
            If you use the percentage mode, contact NetSuite Professional Services for more information.
            
            Important:
            
            When using the **M/S as a % of License** model, always place M/S transaction lines after License - Term line items. When transaction lines are ordered otherwise, the calculated amounts for the M/S transaction lines don't show in the VSOE field.
            
6.  Click **Next**, and then review your selections.
    
7.  Click **Finish** to save your settings.
    

After you complete the EITF 08-01 Assistant, you can enter estimated selling prices for your items. See [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html).

## Modifying Implementation Settings {#bridgehead_N1746607}

You can access the EITF 08-01 Assistant only one time to set up EITF 08-01 Revenue Recognition. To change item category formulas, dimensions, and other preferences after using the assistant, you must modify the custom records that store this information.

#### To modify custom records: {#procedure_N1746621}

1.  Go to Customization > Lists, Records & Fields > Record Types.
    
2.  Select a record type:
    
    -   EITF Item Category Formulas
        
    -   EITF-08-01 Preferences
        
    -   Multiple Allocation Prices
        
3.  Make the necessary changes. Click **Change ID** if you need to change the ID for the record.
    
    Note:
    
    When changing formulas for the Maintenance/Support item category, note that {CUSTOME81MSPERCENT} is only valid for **M/S as a % of License** formulas.
    
4.  Click **Save**.
    

## Setting EITF 08-01 Preferences {#bridgehead_N1746683}

#### To set preferences:

1.  Go to Setup > Company > Preferences > General Preferences.
    
2.  Click the **Custom Preferences** subtab.
    
3.  Under EITF-08-01 Platform Feature, you can set the following preferences:
    
    -   **Allow Contingent Revenue Handling** - Check this box to prevent over-allocating revenue when the ratio of the estimated selling price of professional services items on the sales order is greater than the ratio of the selling price of those items. When enabled, this preference adds the Contingent Revenue Handling Triggered and Contingent Revenue Handling Run fields to sales orders. For information, see [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html).
        
    -   **Auto Calculate Revenue Allocation** - Check this box to calculate allocations for the VSOE field for transaction lines automatically when you edit a transaction. By default, this preference is checked. For more information, see [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html).
        
    -   **Apply Price Range** - Check this box to use a range of estimated selling prices to determine how to allocate revenue for an item. By default, this preference box is clear. See [Using Estimated Selling Price Ranges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html#bridgehead_N1748877).
        
    -   **Always Calculate EITF-08-01** - Check this box to calculate the Allocation Price and Calculated Amount for information purposes only. Revenue for transaction items isn't allocated. By default, this preference box is clear. See [Previewing Allocation Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html#bridgehead_N1749710).
        
4.  To set the **Two-Step Revenue Allocation** preference, go to Customization > Lists, Records & Fields > Record Types.
    
5.  Click the **List** link for the EITF 08-01 Preferences record.
    
6.  Click **Edit** next to Two-step Revenue Allocation.
    
7.  In the **Preference Value** field, type **T** to enable Two-Step Revenue Allocation.
    
    Two-Step Revenue Allocation calculates revenue allocation amounts for multiple element sales where both the EITF 08-01(ESP) and SOP 97-2 (VSOE) accounting rules apply to items on a single sales order. The default Preference Value is F. For more information, see [Two-Step Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1744063.html).
    
8.  Click **Save**.
    

## Setting Roles and Permissions for EITF 08-01 Custom Records {#bridgehead_N1746774}

Use roles and permissions to determine which users can access the custom records for item category formulas, multiple allocation prices, and EITF 08-01 preferences. Typically, full permissions is restricted to roles for accounting users and revenue managers who are entitled to create multiple element sales orders. You can also set the Revenue Management VSOE permission to determine which roles have permission to run scripts that update allocation amounts based on EITF 08-01 rules.

For more information about setting roles and permissions, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html) and [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html).

#### To set record permissions for EITF custom records: {#procedure_N1746809}

1.  Go to Customization > Lists, Records, & Fields > Record Types.
    
2.  Click **EITF Item Category Formulas**.
    
3.  Check the **Use Permissions** box.
    
4.  On the **Permissions** subtab, add roles and set the permission level.
    
5.  Click **Save**.
    
    Repeat the steps to set permissions for **EITF-08-01 Preferences** and **Multiple Allocation Price** records.
    

#### To set access permissions for roles: {#procedure_N1746857}

1.  Go to Setup > Users/Roles > Manage Roles.
    
2.  Click **Edit** or **Customize** for a role.
    
3.  On the **Permissions** subtab, go to **Custom Record** subtab.
    
4.  Add the following custom records:
    
    -   EITF Item Category Formulas
        
    -   EITF-08-01 Preferences
        
    -   Multiple Allocation Price
        
    
    For each record, in the Level column, set the level of permission for the role.
    
5.  Click **Save**.
    
    Repeat the steps for other roles as necessary.
    

#### To show VSOE columns by role: {#procedure_N1746934}

1.  Go to Setup > Users/Roles > Manage Roles.
    
2.  Click **Edit** or **Customize** for the role you want to allow view access.
    
3.  On the **Permissions** subtab, click **Lists**.
    
4.  Add **Revenue Management VSOE**, and then select the access level you want to assign to the role.
    
5.  Click **Save**.
    
    Repeat the steps for other roles as necessary.
    

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [EITF 08-01 Allocation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

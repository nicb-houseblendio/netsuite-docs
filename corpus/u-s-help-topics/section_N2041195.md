---
id: "section_N2041195"
type: "section"
title: "Importing the State Sales Tax Table"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Importing the State Sales Tax Table"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041195.html"
anchors: ["bridgehead_4731540106", "procedure_N2041292", "procedure_N2041421", "bridgehead_4731542249"]
sha256: "058e2d4f3d04aa05e2c46ef99ec4535261ac04976912496b68b451f4b7022467"
---

NetSuite enables you to import up-to-date sales tax codes for the states in which you charge sales tax. Each month, NetSuite updates its database table that stores the tax rates for all U.S. states. The **Version** field on the State Tax Import page indicates the effective date of the tax rate change.

NetSuite receives the tax table updates from Wolters Kluwer. You can visit [wolterskluwer.com](https://www.wolterskluwer.com/en/tax-and-accounting) for information. Updated tax rate tables are uploaded at the end of each month and are effective from the 1st of the month. To keep your state sales tax tables up-to-date, you must reimport tax rates on the last day of each month. Consult your tax agency to ascertain the dates when changes to the tax rates take effect. Then, reimport the updated tax table at the appropriate time.

Note:

NetSuite tax rates for U.S. are determined by zip codes. Zip codes are determined by the US Postal service and don't take into account administrative districts and boundaries. It is therefore possible that a single zip code can be assigned to multiple cities if required. For further information, see [All U.S. Postal Service ZIP Codes](http://business.cch.com/salestax/ZIPsalesZIPCodes.asp)

## Using the State Sales Tax Tables {#bridgehead_4731540106}

Perform the following steps to update U.S. sales tax codes.

#### To import sales tax tables: {#procedure_N2041292}

1.  Go to _Setup > Accounting > Taxes > Use State Sales Tax Tables_.
    
2.  In the **State** dropdown list on the State Tax Import page, select a state for which to import tax tables.
    
    Note:
    
    If the state for which you want to import tax rates does not appear in the State dropdown list, add the state to your nexuses list at Setup > Accounting > Taxes > Nexuses (Administrator). Then, change your Tax Codes Lists Include preference to **Tax Groups and Tax Codes** or **Tax Groups Only**.
    
3.  Select a tax agency and tax account for each type of tax. See [Changing a State's Tax Agency or Tax Account During Import of the State Sales Tax Table](#bridgehead_4731542249).
    
4.  Optionally you can check the **Force override of inactive tax items and reactivate them** checkbox, to update and reactivate inactive tax codes and groups.
    
5.  Click **Save**.
    

After the import, NetSuite sends a confirmation message to the email address on the Company Information page. To view the tax codes that you imported, go to _Setup > Accounting > Taxes > Tax Codes_.

Important:

If you import your tax tables again, any manual changes you made to your tax codes must be entered again.

Note:

If you operate a web store, NetSuite can automatically match your shoppers' ship-to address with the closest matching sales tax code and calculate the correct sales tax.

#### To manually edit a sales tax code: {#procedure_N2041421}

1.  Go to _Setup > Accounting > Taxes > Tax Codes_.
    
2.  Click **Edit** next to the tax code you want to update.
    
3.  On the tax code record, make necessary changes.
    
4.  Click **Save**.
    

## Changing a State's Tax Agency or Tax Account During Import of the State Sales Tax Table {#bridgehead_4731542249}

-   **Changing a state's tax agency** - When you change a state's tax agency for a specific tax type during the update of the sales tax table, the system also updates the **Tax Agency** field on the state's tax code records **of that tax type**.
    

-   **Changing a state's tax account** - When you change a state's tax account for a specific tax type during the update of the sales tax table, the system also updates the **Tax Account** field on the state's tax code records **of that tax type**.
    

The tax agencies and tax accounts you select when submitting the State Tax Import will be set on the tax codes of the corresponding tax types, regardless of the tax agency and tax account previously set on the tax code. This is also true regardless of whether the tax code's tax rate is updated or not.

Changes are not applied to tax codes that are inactivated by the sales tax import.

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Enabling U.S. Tax Lookup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041606.html)
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

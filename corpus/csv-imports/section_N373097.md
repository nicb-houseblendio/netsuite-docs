---
id: "section_N373097"
type: "section"
title: "Selecting General Ledger Accounts for Item Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Selecting General Ledger Accounts for Item Imports"
parent: "section_N370470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html"
anchors: []
sha256: "49fa2eea2657cd9fc61d29c63b57e2ca99f61e6b275a61bc0cb4714caffac599"
---

Different item types have different accounting requirements and considerations. If you're setting up your account for the first time, you should review this topic and consider creating General Ledger (GL) accounts before you import items.

In regard to their General Ledger (GL) impact, item types fall into two categories:

-   Some item types have no accounting component.
    
-   Some item types can optionally be created as posting items that require an account, or as non-posting items that don't.
    

For items in the second category, note that if you choose to make them non-posting, they can't be used on transactions and have no direct impact on your General Ledger. However, you might choose to make items non-posting if they're to be used as parent items, or as components of kits and assemblies.

The following table summarizes the primary accounting considerations for each item type that can be imported. Note that, for those item types that can be associated with one or more accounts, the list of valid account types you can choose from varies depending on whether the Expand Account Lists option has been enabled. If enabled (at _Setup > Accounting > Accounting Preferences_), Expand Account Lists let you choose from a greater number of account types than would otherwise be available. Except where noted, the table below assumes that you don't have this preference enabled. Note also that this table summarizes only the minimal accounting components that exist. Some items have additional optional accounting choices. For full details, see the help topic for the relevant item.

Map your account fields with some care. If you map to an account that is not considered valid for the item type, the import fails with an 'invalid account reference key' error. Of course, if you already have your accounts set up, you can double-check which accounts are valid by referring to the various Account lists on the forms where you manually create items.

| Item Type/Subtype | Accounting Component? | Valid Account Types to Choose when Adding | Valid Account Changes when Updating |
| --- | --- | --- | --- |
| Assembly/Bill of Materials | Yes, but you can make the item non-posting by mapping the Cost of Goods Sold (COGS), Asset, and Income account fields to values of 'null' (all lowercase) in your CSV file, or creating default values of null on the mapping page. | Cost of Goods Sold (COGS), Asset, and Income |
| Description | No | \- |
| Discount | Yes, but you can avoid entering an account by mapping the Non-Posting field to Yes. You can do this either by mapping to a Non-Posting column in your CSV file or creating a default value on the mapping page. | Expense or Income | You can update only to the same type of account selected when the record was created. For example, if you chose an expense account originally, the update can be only to another expense account. With Expand Account Lists enabled, the Account field can be updated to a different account type other than the one chosen when the item record was created. |
| Inventory | Yes, but you can make the item non-posting by mapping the Cost of Goods Sold (COGS), Asset, and Income account fields to values of 'null' (all lowercase) in your CSV file, or creating default values of null on the mapping page. | Cost of Goods Sold (COGS), Asset, and Income |
| Item Group | No | \- |
| Kit/Package | Yes, but you can make the item non-posting by mapping the Income account field to a value of 'null' (all lowercase) in your CSV file, or creating a default value of null on the mapping page. | Income |
| Markup | Yes, but you can avoid entering an account by mapping the Non-Posting field to Yes. You can do this either by mapping to a Non-Posting column in your CSV file or creating a default value on the mapping page. | Expense or Income | You can update only to the same type of account selected when the record was created. For example, if you chose an income account originally, the update can be only to another income account. With Expand Account Lists enabled, the Account field can be updated to a different account type other than the one chosen when the item record was created. |
| Non-inventory, Other Charge, and Service for Purchase | Yes, but you can make the item non-posting by mapping the Expense account field to a value of 'null' (all lowercase) in your CSV file, or creating a default value of null on the mapping page. | Expense |
| Non-inventory, Other Charge, and Service for Resale | Yes, but you can make the item non-posting by mapping the Income and Expense account fields to values of 'null' (all lowercase) in your CSV file, or creating default values of null on the mapping page. | Income and Expense |
| Non-inventory, Other Charge, and Service for Sale | Yes, but you can make the item non-posting by mapping the Income account field to a value of 'null' (all lowercase) in your CSV file, or creating a default value of null on the mapping page. | Income |
| Payment | Yes. You can select an account by including an Account mapping **and** by setting Group With Undeposited Funds to Yes. If you fail to do the latter, your account mapping is ignored. | Bank or Other Current Asset |
| Subtotal | No | \- |

### Related Topics

-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html)
-   [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html)
-   [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html)
-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html)
-   [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

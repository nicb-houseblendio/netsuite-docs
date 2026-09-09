---
id: "section_N480873"
type: "section"
title: "Personal Preferences for Transactions"
branch: "setting-personal-preferences"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Setting Personal Preferences > Personal Preferences for Transactions"
parent: "chapter_N475297"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N480873.html"
anchors: []
sha256: "3964976218bacd56aaeaf684066d0c948cf7d51b05ab276e5b39bb22ee2e50a7"
---

In the Transactions subtab, you can set preferences such as auto fill transactions, transaction warnings, printing, transaction email attachment, and other.

Go to _Home > Set Preferences_ and click the Transactions subtab to set any of the preferences in the following table.

The following fields are available, based on the features in your NetSuite account, and the permissions associated with your NetSuite role.

| **Field Name** | **Function** |
| --- | --- |
| **Basic** |
| Auto Fill Transactions | If you check this box, information about transaction pages is automatically filled in based on the last transaction for the entity you have chosen. If you use a custom form, NetSuite will load the same custom form as was used for the last transaction for the entity, as well. If you clear this box, click the Auto Fill button on transaction pages and information fills in based on the last transaction for the entity you have chosen. If you use a custom form, NetSuite will populate the custom form you currently have open with the information from the last transaction, and not the custom form that was used in the last transaction. The date and period information about any transaction remains current and all auto filled fields can be changed. |
| Alphabetize Items Regardless of Type | Check this box to list items in alphabetical order, regardless of item type. This preference applies when you search for items in the Item column on transactions such as Sales Orders, Purchase Orders, and Inventory Adjustments. Clear this box to display items listed in the Item column on transactions grouped by item type and listed in alphabetical order. This preference doesn't affect the order of items in the Items subtab on transactions. |
| **Warnings** |
| Duplicate Number Warnings | Choose from the list how NetSuite responds when you enter a document number you've used before. |
| Inventory Level Warnings | Check this box to see warnings when you sell inventory items with quantities at or below their reorder points. You must also set these minimum quantities in the Reorder Point field on item records at _Lists > Items_. |
| Customer Credit Limit Handling | Choose how you want to handle customer credit limits:
-   **Ignore** - Enables you to enter sales orders and invoices that exceed the customer's credit limit without a warning.
-   **Warn Only** - Generates a warning when you enter a sales order or invoice that exceeds the customer's credit limit. The warning displays in a popup window so you can choose to enter or cancel the transaction.
-   **Enforce Holds** - Blocks you from entering a sales order or invoice that exceeds the customer's credit limit.

 |
| Vendor Credit Limit Warnings | Check this box to receive a warning when you exceed the credit limit for a vendor. |
| **Printing** |
| Print Using HTML | Check this box to print transaction forms in HTML format. Clear this box if you prefer to print transactions forms in PDF format. You need Acrobat Reader to print PDF forms. |
| Print GL Impact Per Subsidiary | Print separate GL impact statements for transactions with multiple lines assigned to different subsidiaries (for example, an intercompany journal). NetSuite will print a statement for each subsidiary in the transaction. For more information, see [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html). |
| Transaction Email Attachment Format | Choose the format for which transaction email attachments are sent.

-   **HTML** - Sends email attachments in HTML format.
-   **PDF** - Sends email attachments in PDF format.

Note: If you select the HTML option as a transaction email attachment format, the system won't use the template set in custom transaction forms. |
| Horizontal Print Offset | Enter a positive number in inches to move the text to the right. Enter a negative number in inches to move the text to the left. |
| Vertical Print Offset | Enter a positive number in inches to move the text lower. Enter a negative number in inches to move the text higher. |

Your administrator can customize the layout of your printed forms using advanced PDF/HTML templates. For information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

### Related Topics

-   [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
-   [General Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N475661.html)
-   [Personal Preferences for Appearance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479574.html)
-   [Analytics Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html)
-   [Personal Preferences for Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N482375.html)
-   [Personal Preferences for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N483440.html)
-   [Personal Preferences for Telephony](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484162.html)
-   [Personal Preferences for Restricting Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484545.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

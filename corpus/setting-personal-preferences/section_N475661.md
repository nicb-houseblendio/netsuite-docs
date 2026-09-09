---
id: "section_N475661"
type: "section"
title: "General Personal Preferences"
branch: "setting-personal-preferences"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Setting Personal Preferences > General Personal Preferences"
parent: "chapter_N475297"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N475661.html"
anchors: []
sha256: "c875f39baecf55f281c110c6f2e9664bdbbc751f482a0e11f5311df26e5cea7e"
---

In the General subtab, you can set such preferences as a nickname, language, date and time formatting, warnings and notifications, and other.

Go to _Home > Set Preferences_. The General subtab is displayed by default. On this subtab you can set the preferences in the following table.

The following fields are available, based on the features in your NetSuite account, and the permissions associated with your NetSuite role.

| **Field Name** | **Function** |
| --- | --- |
| **User Profile** |
| Nickname | Enter the name that you want to appear in the From field of email messages you send from NetSuite. For example, you can send an email message by clicking the Email subtab on your employee record. |
| From Email Address | Enter the email address you want shown as the From address in email you send through the system. Replies to this email are sent to this email address as well. If you don't enter an email address here, email you send will show your login email address. |
| Signature | Enter a signature (in HTML markup) you want to appear at the end of email you send from NetSuite. Note: The HTML must be formatted correctly, including line breaks, hyperlinks, character formatting such as Bold, and any other special formatting. If the signature isn't correctly formatted, it won't display properly. For an example, see [Customizing Email Signatures and From Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514531.html). |
| Add Signature to Messages | Check this box if you want your signature automatically added to all fax and email messages you send. Note: If your signature is already included in the fax or email template you're using, your signature won't be added twice. |
| **Localization** |
| Language | Select the language for your NetSuite account. For more information, see [Choosing a Language for Your NetSuite User Interface](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479109.html). |
| Search Sorting | Select the alphabetical order to use for search results.
-   **Language Specific** - the alphabetical order specific to your NetSuite language settings.
-   **English (U.S.)** - the U.S. English alphabetical order.

 |
| Language of the Help Center | Select the language for the NetSuite Help Center. You can choose English, German, Japanese, and Spanish. Note: You can set a different language for the Help Center than the language you specify for the User Interface. Your preference takes effect the next time you open the Help Center and is maintained until you change it. For more information, see [Choosing a Language for Your NetSuite User Interface](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479109.html). Note: You can also set this preference directly from the NetSuite Help Center using the dropdown list at the top right corner of the page. For more information, see [Using the Help Center Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N336258.html). Whether you select the language preference directly in the Help Center or from _Home > Set Preferences_, the preference is maintained until you change it. |
| PDF Language | This option isn't used anymore. To print your reports in a different language, change your NetSuite language in the Language field. |
| Accounting Context | If you have a OneWorld account and one accounting context is defined at _Setup > Company > General Preferences._, this dropdown list appears. An accounting context can be a one-to-one relationship between a country's local GAAP (Generally Accepted Accounting Principles) reporting requirements and a statutory chart of accounts (COA). It can also be a unique relationship that meets your company's specific needs. Accounting contexts are useful if you want to work in a local GAAP context instead of the consolidated context with one centralized COA. When you select an accounting context from this dropdown list, all transactions including system-generated transactions post to the defined COA account name and number. This field is blank by default. When blank, all transactions including system-generated transactions post to the consolidated accounts across all subsidiaries. |
| Time Zone | Select the time zone where you work. Time zone names are in IANA/Olson Value format and follow daylight savings time rules for each time zone. Note that the displayed GMT offset value doesn't reflect daylight saving changes that the system applies automatically. Note: If you change your time zone, it affects all roles associated with your email and password. |
| First Day of Week | Select the day that you want to start your week on. Note: Some reports in NetSuite recognize only Sunday as the first day of the week, regardless of the day you select for this preference. |
| Calendar System | You can only set a calendar preference if you choose Japanese as the Language preference. Select the calendar to use within NetSuite.

-   **Gregorian Calendar** - This is the default and the internationally accepted civil calendar.
-   **Japanese Imperial Calendar** - This is a specialized Japanese calendar. The imperial date format is required for some government documents and applications used in Japan.

 |
| Use Furigana Field | The Furigana field is only available on records in the NetSuite Japan edition when you select Japanese as the Language preference. Check this box if you want to sort lists of records by the Furigana field. |
| **Formatting** |
| Date Format | Select the date format for all of your NetSuite roles. Note: If you change the date format, it affects all roles associated with your email and password. For more information, see [Formatting for Dates, Numbers, Phone Numbers, and Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N249143.html). |
| Long Date Format | Select how to display the month, day and year in NetSuite. Note: If you change the Long Date Format, it affects all roles associated with your email and password. For more information, see [Formatting for Dates, Numbers, Phone Numbers, and Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N249143.html). |
| Time Format | Select an option for how time displays in your NetSuite account. Note: If you change the time format, it affects all roles associated with your email and password. |
| Number Format | Select the format to display numbers online for transaction forms and entity forms for all of your NetSuite roles. For more information, see [Formatting for Dates, Numbers, Phone Numbers, and Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N249143.html). Note: If you change the Number Format, it affects all roles associated with your email and password. |
| Negative Number Format | Select the format to display negative numbers online for transaction forms, entity forms, and search results. For more information, see [Formatting for Dates, Numbers, Phone Numbers, and Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N249143.html). Note: If you change the Negative Number Format, it affects all roles associated with your email and password. |
| Phone Number Format | Select an option to display phone numbers in your NetSuite account. This phone number format is used on all online forms that you print. This setting only applies to seven and ten digit phone numbers. |
| Auto Place Decimal | Check this box to insert a decimal point between the second and third digit from the right when you enter numbers. When you first start using NetSuite, this preference is activated. Important: Clear this box if you're using the Software Verticals Contract Renewals module. Enabling this preference may cause unwanted updates to transaction amounts calculated by Contract Renewals transaction processing. For more information, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html). |
| CSV Column Delimiter | Select the symbol to be used as the default column separator when importing data from CSV files. For more information, see [Setting CSV Import Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html). |
| CSV Decimal Delimiter | Select whether you want to use a period or a comma as the default decimal mark in numbers in the CSV files you import. For more information, see [Setting CSV Import Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html). |
| **Defaults** |
| Use Multicurrency Expense Reports | If the Multiple Currencies feature is enabled in your account, check this box for expense reports to enable use of foreign currencies by default. When you enable this option, the Use Multi Currency box on Expense Report transactions is checked by default. |
| Download PDF Files | Check this box if you use PDF forms and save them as files. Clear the box if you use HTML forms, or if you print PDF forms without saving them as files. |
| Address Mapping Type | Select a service for generating maps for addresses on forms and records. You can click the Map icon next to an address on a form or record to see the map. For more information, see [Mapping Addresses on Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N478992.html). |
| Show Internal IDs | Check this box to be able to view the internal IDs for fields and records in the NetSuite application. Note: The Show Internal IDs field is only available when at least one of the following features is enabled in your account: Client SuiteScript, Server SuiteScript, SuiteScript Server Pages, SuiteFlow, or Web Services (on the SuiteCloud subtab) or Advanced Site Customization or SuiteCommerce Advanced (on the Web Presence subtab). For more information, see [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html). SOAP web services and SuiteScript code need to reference internal IDs to uniquely identify objects, so you should enable this preference whenever you're working with SOAP web services or SuiteScript. When this preference is enabled:

-   You can view the internal ID for a field by clicking on that field's label to open the field level help popup window. The internal ID is displayed in the lower right corner of this window.
-   You can view the internal ID for a record or a custom field in an Internal ID column that displays on a list or search results page for that type of record or custom field.

 |
| Only Show Last Subaccount | Check this box to indent subaccounts in list fields on transactions and forms. For example, with the box checked, subaccounts appear indented under the parent account: Parent account Subaccount 1 Subaccount 2 With the box cleared, subaccount names include the parent name: Parent account Parent account: Subaccount 1 Parent account: Subaccount 2 |
| Only Show Last Subentity | Check this box to indent subrecords in dropdown lists on transactions and forms. This applies to relationship records, such as customers, partners and leads. For example: Parent customer Subcustomer 1 Subcustomer 2 When the box is cleared, subentity record names include the parent name: Parent customer Parent customer: Subcustomer 1 Parent customer: Subcustomer 2 Note: When records display in popup lists, subentity names always include the parent name. |
| Only Show Last Subitem | Check this box to show only subitems and omit parent items in dropdown lists on transactions and forms. For example: Subitem 1 Subitem 2 When the box is cleared, subitem names include the parent name: Parent item Parent item: Subitem 1 Parent item: Subitem 2 Note: When records display in popup lists, subitem names always include the parent name. |
| Do not Display Customer Satisfaction Surveys | Check this box to opt out of in-page satisfaction surveys. |
| Enable NetSuite Guided Learning | Check this box to enable the NetSuite Guided Learning for your account. NetSuite Guided Learning tool provides step-by-step instructions to help you complete tasks in NetSuite. For more information, see [NetSuite Guided Learning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0824114548.html). |
| **Messages** |
| "Save Changes' Warnings | Check this box to see a warning when you're about to leave a page before submitting the transaction you were working on. |
| Limit CC Field to Contacts & Employees | Check this box so that email messages are only copied to contacts or employees. |
| Default Issue Email Notification | Select one of the following options to be notified at your login email address when an issue you have submitted or edited changes:

-   **Never** - Select this option if you don't want to receive any email notifications about changes to issue statuses.
-   **On Any Change** - Receive an email every time someone edits the issue record.
-   **When Base Status is Open** - Receive an email when the issue status changes to a base status of Open.
-   **When Base Status is On Hold** - Get an email when the issue status changes to a base status of On Hold.
-   **When Base Status is Resolved** - Get an email when the issue status changes to a base status of Resolved.
-   **When Base Status is Closed** - Get an email when the issue status changes to a base status of Closed.

Note: If you set issue notification preferences through the Customer Center, they go back to company default settings if your Customer Center access is suspended. |
| Notify Me Upon Issue Assignment | Check this box to receive a notification at your login email address when an issue is assigned to you. |
| Show Notification When AI Feature Is Used | Clear this box to stop showing the AI confirmation message when you use Text Enhance. This box is checked by default. You can also turn off this preference from the AI confirmation message. Leave the **Do not show this message again** box checked, and then click **OK** to close the AI confirmation message. |
| Notify me of successful manual bank imports | Check this box to receive an email notification when you complete a manual bank statement import successfully. Clear this box if you prefer not to receive success notifications for manual imports you perform. |
| Notify me of successful automatic bank imports | Check this box to receive an email notification when an automatic bank statement import completes successfully. Clear this box if you do not want to be notified of successful automatic imports. |
| Alert me of issues with automatic bank imports | Check this box to receive an email notification when an automatic bank statement import fails or completes with errors. Clear this box if you do not want to receive alerts about problems with automatic imports. |
| **Optimizing NetSuite** |
| Delay Loading of Sublists | Check this box to delay loading information about subtabs until you click the specific subtab. Note: Setting this preference improves page-load times. |
| Number of Rows in List Segments | Enter the maximum number of records to display in each segment. For example, if you have 200 customers, enter 25 in this field to see them in groups of 25 per page. To go through the list of results, select from the dropdown list or use the previous and next arrows on the toolbar. You can change this number up or down based on your visual and scrolling preferences. Note: Setting the list segment to 25 or less improves page-load times. |
| Maximum Entries in Dropdowns | Enter a number beyond which a dropdown list becomes a popup list. When the list reaches the maximum you set here, the list displays in a pop up window. Be aware that this number is a guideline. If the list of values displayed for a field is dynamic, you might still see a popup even for a smaller number of values. The use of a popup is especially likely for any custom field with values sourced from a dynamic list because the size of the list could sometimes be above the maximum. Note: Setting the maximum entries to 25 or less improves page-load times. Note: The Case/Task/Event field for time transactions is displayed as a dropdown list only if the sum of all company-wide case, task, and event records is less than 5000 and less than the number entered here. Roles that can enter time transactions on behalf of other employees will always have a pop-up field displayed. |
| Allow Favorites in Dropdowns | You can select up to five favorite items in the Customer, Add Multiple, and Items fields on sales orders. In the Add Multiple field, you can show only your favorite items by selecting the **Show favorites only** box. To mark an item as a favorite, click the star icon next to the item name in the dropdown list. Favorites are associated with your personal preferences and are specific to your NetSuite account and role. |
| Type-Ahead On List Fields | When you check this box, NetSuite shows a list of matching records you can select from when you type characters into a dropdown list field. This preference may enable you to enter data into list fields more quickly. |
| Require Exact Match on Item Type-Ahead | When you turn on the Type-Ahead On List Fields option (above), check this box so that NetSuite selects a record based on an exact match of the characters you type. Otherwise, NetSuite chooses a record based on the first character you typed. |
| Show Quick Add Row on Lists | Check this box to use quick add on lists that can be edited inline. Quick add enables you to create new records from lists and only add basic information. You can turn this preference off on individual lists. |
| Display Bounce Warning on Campaigns | Clear this box to restrict the automatic scanning of hard-bounced email addresses in your marketing campaign. When this preference is turned off, you can manually screen hard-bounced email addresses. |
| Do not Calculate Balances on Customer Record | Customer records include a Balance Information subtab. The information in this subtab is calculated when you open a customer record. Check this box to disable this calculation when you open a customer record. This may load customer records faster. |
| Prefer Native Select Fields over NS Dropdowns In Internet Explorer | Important: This field is only for users of the Internet Explorer browser. Select this box to use native dropdown lists rendered by your Internet Explorer browser rather than dropdown lists rendered by the NetSuite user interface. This can improve page performance, particularly on pages with many dropdown lists. Page performance varies due to the interaction of many factors, including:

-   the type and complexity of the page
-   whether the page has been customized
-   the number and type of features enabled in an account

If you continue to experience less-than-optimal page performance even with this option selected, please contact Technical Support. |
| **SuiteCloud Development Framework** |
| Show App ID Field | Check this box to display the App ID field on custom objects that are supported by SDF. |
| Show ID Field on Sublists | Check this box to display script ID fields in sublists that are supported by SuiteCloud Development Framework. |

### Related Topics

-   [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
-   [Personal Preferences for Appearance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479574.html)
-   [Personal Preferences for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N480873.html)
-   [Analytics Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html)
-   [Analytics Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html)
-   [Personal Preferences for Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N482375.html)
-   [Personal Preferences for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N483440.html)
-   [Personal Preferences for Telephony](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484162.html)
-   [Personal Preferences for Restricting Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484545.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

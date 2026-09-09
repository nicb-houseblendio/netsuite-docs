---
id: "section_N2842731"
type: "section"
title: "Field Type Descriptions for Custom Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Field Type Descriptions for Custom Fields"
parent: "chapter_N2826978"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html"
anchors: []
sha256: "214f2fde0b54022a45a47907293735da3bb1aa91229914b5011d414d07518165"
---

When creating a custom field, you select the type of field based on the information you want to store.

The following table describes all available field types for custom fields. Note that character limits are for English letters (1 byte per letter). For non-English languages, character limits are lower (up to 4 bytes per character). Non-English characters affect field limits, which may be lower than stated.

| **Field Type** | **Description** | **Example** |
| --- | --- | --- |
| Check box | Use a check box to record a true or false answer. | For example, create a Delivery check box custom field to track orders on sales transactions. Check the box for delivery orders. |
| Currency | Enter currency amounts up to 15 digits and 15 decimal points (999,999,999,999,999.999999999999999). Custom currency fields work differently than standard NetSuite currency fields. Without the Multi-currency feature, custom currency fields won't be hidden like standard NetSuite currency fields. Note: When you select Currency for the Type, a Currency Context subtab becomes available. For more information, see [Setting Currency Context for a Currency Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0511114806.html). | For example, create a currency field on employee records to track employee spending limits. |
| Date | Enter or select dates. Changing Date fields to Date/Time fields converts dates in existing records to date/times. The time defaults to midnight in your company's time zone. | For example, create a Projected Start Date custom field to track start dates on estimates. Dates entered must follow the date format selected at _Setup > Company > General Preferences_. Note: The date and time are based on the user's NetSuite Time Zone preference, set at _Home > Set Preferences_, not on the browser client time zone. |
| Date/Time | Store date and time in a single field. Date/time values are displayed in the user's preferred format and time zone. Time values are stored down to the second. you can also add Date/Time custom fields using the `form.addField(options)` method. **Important:** When using the `addField` method, you must specify 'datetimetz' for the **type** parameter. | For example, use a single field for date and time timestamp data. Note: Date and time are based on your NetSuite Time Zone preference, set at _Home > Set Preferences_, not your browser's time zone. |
| Decimal Number | Enter a decimal number in a custom field. The maximum input is 20 digits (10,000,000,000,000,000,000). Numbers larger than the maximum will be rounded down. | For example, you want to record the distance your customers are from your nearest retail outlet. Create a decimal number field to store this information in employee records. |
| Document | 
Select a File Cabinet document to preview or download. The field is searchable and can be added to search results.

**Note:** Users of this field need File Cabinet access to view, select, or upload documents.



 | For example, let employees search customer survey results. |
| Entity | Create custom fields of type **Entity**. To create a custom entity field, set the field type to List/Record and the List/Record type to Entity. By doing so, the new **generic** custom entity field will automatically include all records of type contact, customer, employee, group, other name, partner, and vendor. You can also use sourcing and filtering to limit the choices in the custom field's list to a subset of the supported entities. | For example, on the custom field's definition page, on the Sourcing & Filtering subtab, specify Type in the Filter Using column. In the Value Is column, select customer, partner, and vendor names. When the custom field of type Entity appears on your record, entities of only type customer, partner, and vendor will appear as available options in the field's list. |
| Email Address | Enter an email address (up to 254 characters). The email address field creates a link to open your default email client. | For example, create a custom record type for interns that includes a field for their email addresses. Click the email address on their records to send them an email message. |
| Free-Form Text | Enter up to 300 characters of text. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | For example, offer your customers monogramming on certain items by creating a Free-Form Text field as an item option to record the monogram. Note: Calculations in free-form text fields use scientific notation. To avoid scientific notation, use the ROUND({cost}/0.65,3) syntax to round digits. |
| Help | Add helpful text to record pages where users enter information (up to 999 characters). This help is for informational purposes only. It's not stored in your account. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | To create a Help custom field, select Help in the Type field and enter your text in the Help field. |
| Hyperlink | Enter a URL to link to another web page (up to 999 characters, with a hyperlink text limit of 10 characters). Hyperlink fields should start with http://, https:// or ftp://. Note: For safety reasons, files starting with file:// or \\\\ aren't supported. You can enter a file in this format, but the link won't work. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | For example, you want to link to a vendor's website. You create a hyperlink custom field called Website that appears on vendor records. First, you enter the company's URL. When you return to the vendor's record, you can click the URL to open the vendor's site in a new window. You can enter up to 999 characters in the field. |
| Image | Attach an image to a record. The image is rendered with a maximum width of 250 pixels in the form layout, and the image is resized proportionally. Image custom fields support the following file formats:

-   .bmp
-   .gif
-   .jpg
-   .jpeg
-   .pjpg
-   .pjpeg
-   .png
-   .tiff
-   .tif

Note: The TIF/TIFF file format may not be supported by all browsers. | For example, you can attach pictures of your employees to their records. |
| Inline HTML | Use Inline HTML on all types of fields. You can use HTML to create custom fields on record forms or to create custom fields to use on Suitelet custom pages. For more information about using HTML with Suitelets, see [SuiteScript 2.1 Suitelet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799600.html). The Inline HTML field has a 4000-byte limit. In English, 4000 bytes is 4000 characters, but in other languages, the character number may be fewer. Important: NetSuite Forms does not support manipulation through the Document Object Model (DOM) and custom scripting in Inline HTML fields. The use of Inline HTML fields on Form pages (except for Forms generated by Suitelets) won't be supported with a new user interface in a future NetSuite release. URLs in custom fields should use your account-specific domain. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). Important: The Inline HTML field type does not support labels, the UI does not display labels for Inline HTML fields. | For example, you could display to customers how many reward points they have earned. |
| Integer Number | Enter integers in a custom field. The maximum number is about 18000000000000000000 (20 digits). Note that this maximum can be affected by rounding and technical limitations. | For example, use this field to record a special ID number. |
| List/Record | Attach lists and records to custom fields. In the List/Record field, select the list or record type to attach. You can also select from **public** saved searches. You can use this option to script a custom printing solution. For more information, see [Scripting a Custom Printing Solution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4388569541.html#bridgehead_4546180398). | For example, track orders by the employee working on them by creating a custom body field for sales transactions. Attach your employee list to the List/Record field. Then, on sales transactions, select the employee for the order. |
| Long Text | A text area that can hold up to one million (1,000,000) characters. Use Long Text fields when you need more than 4,000 characters for a text area without rich text formatting. In the UI, long text field types have a 1,000,000 character limit. With SuiteScript, long text field types have a 100,000 character limit. Note: You can convert free form text or text area fields to long text fields. However, after the conversion is complete, the field **can't** be converted back. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | For example, use a Long Text custom field in a custom record to hold the text of an item Warranty. Or, add to an Online Form to hold the text of a End User License Agreement. |
| Multiple Select | Create a field for multiple selections from a list or list of records. Note: Multiple Select fields in saved search results have a 4000-character display limit. | For example, track how customers found your business. Create a multiple select field on customer records with possible sources. Sales reps use the field to select where customers heard about your business. |
| Password | Create a field that's encrypted in the database (up to 15 characters). The field always shows a fixed number of characters, regardless of password length. When validating, you pull the encrypted password value into a hidden field and use custom code to encrypt the value the user typed. Then, compare it with the real encrypted value. Make sure customizations handle sensitive fields properly. | For example, add a password field to a web page. |
| Percent | Create a field to store a percentage. The field accepts only integers from 0 to 100. | For example, track employee test results as a percentage. The percent sign (%) is added automatically. |
| Phone Number | Create a field for phone numbers on records and transactions (up to 32 characters). If phone number formatting is enabled, numbers are localized. The user's subsidiary country determines the localization. | For example, add a contact number to an event record using a CRM field. |
| Rich Text | Enter and format up to one million (1,000,000) characters of text in a custom field. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | For example, include a brief employee bio with details like marital status and family members. You can also format the text with lists, bold/italic text, and custom font sizes and colors. |
| Text Area | Enter up to 4,000 characters of text in a custom field. The Text Area field has a 4000-byte limit. Note that 4000 bytes is 4000 characters in English, but may be fewer characters in other languages. Use your account-specific domain for URLs in custom fields. For more information, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html). | For example, record notes about closing a customer by entering information into a text area field on the customer record. |
| Time of Day | Create a field for entering the time of day. | For example, create a Best Time To Call field for sales reps to enter the best time to call a prospect. |
| URL Fragment | Create a field for entering a URL Fragment in a custom field. Note: This field has a 200- character limit. | For example, use the URL Fragment field to create a precise web reference. |

For information about creating a custom field, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).

For information about account-specific domains, see [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html).

### Related Topics

-   [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html)
-   [Custom Fields Videos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0510123425.html)
-   [Using Account-Specific Domains for URLS in Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162263823971.html)
-   [System Notes for Changes Made in Text Type Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0429092902.html)
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Available Standard Fields and Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2843906.html)
-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Inactivating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4352401817.html)
-   [Editing a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314473404.html)
-   [Advanced Features for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4388569541.html)
-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

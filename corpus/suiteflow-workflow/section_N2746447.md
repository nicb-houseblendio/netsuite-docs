---
id: "section_N2746447"
type: "section"
title: "Send Email Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Send Email Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2746447.html"
anchors: ["bridgehead_4148812453"]
sha256: "d0b17ed26126729211d0710e9661d95356ea443d3722cb792e47bc4b1cd28c8f"
---

Use the Send Email action to send an email when the action executes. When you create a Send Email action, you can specify the sender, recipient, message content, and add attachments.

You can use the **Scheduled** trigger and specify in the **Schedule** section a time when the email will be sent. You can also schedule a Send Email action by scheduling a transition into a state that contains a Send Email action. See [Scheduling an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103059488.html) and [Scheduling a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103067244.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Send Email action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Send Email Action Parameters {#bridgehead_4148812453}

The following table describes the Send Email action parameters:

| Section | Parameter | Description |
| --- | --- | --- |
| Sender | Specific Sender | Use the email address of a NetSuite user as the sender. |
|  | From Field | Set the following options:
-   **Record (Join Field):** Select a record type that contains the field with the associated email address to use as the sender.
-   **Field:** Use the email address associated with this field. It can be a field that has an email address value or a field that references another record.

 |
| Recipient | Send To Current Record | Only available for some entity records. Send to the email address associated with the current record in the workflow. |
|  | Specific Recipient | Use the email address of a NetSuite user as the recipient. |
|  | Free Form Address | Email address or addresses to use. Separate multiple address with a comma, with no spaces in between. |
|  | From Field | Set the following properties:

-   **Record (Join Field):** Select a record type that contains the field with the associated email address to use as the recipient.
-   **Field:** Use the email address associated with this field value.

 |
|  | Cc | Email address or addresses to use as a **Cc**. Separate multiple address with a comma, with no spaces in between. Field is limited to 1000 characters. You can also reference internal NetSuite IDs. See [Using Internal IDs in an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148825528.html). |
|  | Bcc | Email address or addresses to use as a **Bcc**. Separate multiple address with a comma, with no spaces in between. Field is limited to 1000 characters. You can also reference internal NetSuite IDs. See [Using Internal IDs in an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148825528.html). |
| Content | Use Template | Select an email template to use for the email content. You must have the Mail Merge feature enabled to use email templates. |
|  | Custom | Select this option and manually enter the content in the **Subject** and **Body** fields. You can also use internal NetSuite IDs. See [Using Internal IDs in an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148825528.html). |
|  | Include View Record Link | Include a link to the current workflow record in NetSuite at the end of the email. A link appears in the email with the text **View Record**. The recipient can click the link and log in to NetSuite to view the record. |
| Attachment | File | Select this option files from the File Cabinet. The maximum file size is 10 MB. Form more information, see [Attaching Files to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148832559.html). |
|  | From Field | Select a **Record (Join Field)** record type and a **Field** from a record that has a reference to a document. The maximum file size is 10 MB. See [Attaching Files to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148832559.html). |
|  | Include Transaction | Attach transaction details for workflows based on any transaction record type. If selected, the transaction details sent are those that belong to the current record in the workflow. |
|  | Include Statement | Include a statement for workflows with Customer, Lead, or Prospect as their base record type. See [Attaching Statements to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148832855.html). |
|  | Type | The rendering style of the statement you are including in the email. Only active if you are including a statement with your email message. Choose one of the options:

-   **Inline - Above.** The statement information appears above the body text.
-   **Inline - Below.** The statement information appears below the body text.
-   **Default.** The statement is attached based on the customer's email preference from the **Preferences** subtab of the customer record. The default customer behavior is to attach the statement according to the email preference of the current user in the workflow.
-   **HTML.** The statement appears as an HTML attachment.
-   **PDF.** The statement appears as a PDF attachment.

 |
|  | Statement Date | Select the date when the statement was generated. This option applies to the statement you are including and is unavailable if you are not including a statement with your email message. |
|  | Start Date | Select a date for the earliest transactions you want to show on the statement. Leave this field blank if you want to show all transactions for this customer. This option applies to the statement you are including and is unavailable if you are not including a statement with your email message. |
|  | Show Only Open Transactions | This option applies to the statement you are including and is unavailable if you are not including a statement with your email message. |
|  | Consolidated Statement | Check the **Consolidated Statement** box to send a statement showing the overall balance for the customer-subcustomer hierarchy this customer is a part of. Clear this box to send a statement showing only the balance for this customer. Disable this option to show only a balance. |
|  | Use Customer's Locale | Select this option to generate the statement in the customer's locale, instead of the default company language. For a list of supported languages, see System Supported Languages in [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html). Only available for workflows based on the Customer record type. |

Note:

The options available in the **Attachment** section differ depending on the type of record.

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Internal IDs in an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148825528.html)
-   [Attaching Files to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148832559.html)
-   [Attaching Statements to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148832855.html)
-   [Attaching Transactions to an Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4148833302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

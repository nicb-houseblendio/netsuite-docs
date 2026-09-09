---
id: "section_N495192"
type: "section"
title: "Using Inline Editing"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Lists > Using Inline Editing"
parent: "section_N494311"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html"
anchors: ["procedure_N495214"]
sha256: "8b417dc95c2e3c8f08d8045612c7c830625f6051a56631cbba475b7a5d36cffd"
---

Inline list editing enables you to update records quickly by changing data directly in a record's row on the list page. This makes editing faster and easier since you don't have to open each record to make changes. You can also edit multiple records simultaneously by using keyboard commands. You can't edit addresses on list pages with inline editing.

Inline list editing is available when the Inline Editing feature is enabled. To enable the feature, go to _Setup > Company > Enable Features_. On the Company subtab in the Data Management section, check the Inline Editing box and click Save.

#### To use inline editing: {#procedure_N495214}

1.  Use the **Edit** switch at the top of the page to turn on inline editing. When editing is off, the switch displays an x. When editing is on, the switch has a green check.
    
    ![List record page with Edit switched on.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/InlineEditing_On.png)
    
    The list page refreshes to display an edit icon in each column header that contains editable fields. You can also identify editable fields by placing the cursor on them. A field is editable if the cursor turns into a hand when on the field.
    
    Important:
    
    Display types affect whether fields are available for editing or not. For more information, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).
    
    Important:
    
    Columns that display an edit icon in the header may include field values that aren't available for the inline editing due to data validation that prevents editing generally. The edit icon doesn't mean that you can use inline editing for every field in the column.
    
2.  Click the field where you want to enter or change information.
    
3.  Click away from the field to save your changes.
    

The data is automatically saved on that record.

Use the following keystrokes to move among editable fields:

-   Press Tab to move right.
    
-   Press Shift+Tab to move left.
    
-   Press Shift+Enter to move up.
    
-   Press Enter to move down.
    
-   Press Alt+X to edit the first editable field on the page.
    
-   Press Ctrl+Z to revert the value in a field back to the previous value.
    
-   Press Esc when you're done editing a field to save the new value and close the field.
    

You can also use the following tools to increase your data entry performance when inline editing is enabled:

-   Edit the same field on multiple records by pressing Ctrl and holding it as you select multiple fields.
    
    Note:
    
    Note that you can only edit multiple fields in the same column. You can't edit multiple fields across different columns at the same time.
    
-   Click **Add** above the list to open a Quick Add popup window for the current record type.
    
-   Click the ![New Record icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/WorkingWithRecords_NewRecordIcon.png) icon in the **New** column to open menu of related records. Select an option to create the new record on a separate page. The icon appears when you move your pointer over the column.
    

If you change many field values in one session using inline editing, NetSuite may have to update multiple records simultaneously. In this case, you may receive the following message: 'Too many inline edits. Please wait a few seconds and try the edit again.' You should be able to complete your most recent edit after a brief wait.

For more detailed information and considerations related to inline editing, see [Additional Notes about Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N495470.html).

### Additional Information

-   [Unable to Use Inline Editing Even When Feature Is Enabled](https://suiteanswers.custhelp.com/app/answers/detail/a_id/11844)
-   [Mass Delete Records in NetSuite through Inline Editing](https://suiteanswers.custhelp.com/app/answers/detail/a_id/26816)

### Related Topics

-   [Working with Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N494311.html)
-   [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html)
-   [Using the Recent Records Menu](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495728.html)
-   [Working with List Views, Sublist Views, and Dashboard Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495842.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

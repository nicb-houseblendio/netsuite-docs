---
id: "section_N691977"
type: "section"
title: "Creating Saved Searches for System Notes"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating Saved Searches for System Notes"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691977.html"
anchors: ["procedure_N692009"]
sha256: "f205961883857d70fd0763cdf5df34eb1f30a4b1f633df5df8efbf59e81ac378"
---

Note:

Note: The information in this topic applies to System Notes only. For information about searching System Notes v2, see [Searching and Filtering System Notes v2](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159499608205.html).

You can create saved searches for system notes using the System Notes Fields... filter. When you select this filter, you can choose which type of system note you want to search and enter your criteria to track changes on records. For more information about system notes, see [System Notes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158644279544.html).

#### To create a saved search for system notes: {#procedure_N692009}

1.  Go to Lists > Search > Saved Searches > New, and select a record type for the search.
    
2.  On the **Criteria** subtab, select **System Notes Fields...** in the **Filter** field.
    
3.  In the popup window, select the **System Note** field you want to filter your search by.
    
4.  Select the criteria based on the type of note you selected.
    
5.  Click **Add**.
    
6.  Click **Preview** or **Save & Run** to view your search results.
    

Note:

System notes descriptions are limited to 300 characters. Any additional characters are truncated.

Note:

The Log System Notes on Update Only preference prevents NetSuite from logging system notes when records are created. When this preference is set, system notes are logged only when records are updated. See [Setting General Account Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243797.html). Before you set this preference in an account that existed before that release, you should first review any saved searches containing system notes fields, as these searches may use data from record creation system notes. If your account includes searches that rely on record creation system notes, you can either revise the searches before setting the Log System Notes on Update Only preference, or you can leave this preference not set.

For example, a case search may use record creation system notes fields to retrieve dates when cases were first escalated. To make this search work with the Log System Notes on Update Only preference set, this search would need to be edited to use expressions and to return values for cases' Date Created field if the escalation date was not available through record update system notes fields.

For custom transaction body fields, if the Log System Notes on Update Only preference is not set, and you have the View access level to a field, the default value of your custom transaction body field is displayed in system notes fields when you create a transaction search. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

For more information about saving searches, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html)
-   [Creating Saved Searches for User Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N692249.html)
-   [Creating Saved Searches for Messages on Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N692421.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

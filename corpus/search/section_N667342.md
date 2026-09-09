---
id: "section_N667342"
type: "section"
title: "Defining a Mass Update"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Mass Updates > Defining a Mass Update"
parent: "article_1103335211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N667342.html"
anchors: ["procedure_N667359"]
sha256: "4b2c18a904e149b654201d9eef98d5088c59b52b03f8b8d2068951b876e6ab54"
---

You can define a mass update if you have the Mass Updates permission.

#### To define a mass update: {#procedure_N667359}

1.  Go to Lists > Mass Update > Mass Updates.
    
2.  On the Mass Updates list, expand a category and click a link.
    
    ![Mass Updates list with the Customer Support and Service category expanded.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/massupdates1.png)
3.  In the **Title of Action** field, enter a name for this update.
    
    If you are saving this mass update, create a name that describes the update so you can find it in the future.
    
4.  To enter the new information:
    
    -   If you are performing a General mass update on a record type:
        
        Click the **Mass Update Fields** subtab and review the fields that are available for update.
        
        Check the box in the **Apply** column next to each field you need to update, and enter or select the new data in the **Value** column. Or, you can enter a formula to dynamically calculate values to be entered. See [Entering Formulas for a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668091.html).
        
        Fields exposed for mass updates are the same as those available for inline editing and include the following: standard fields that are outside of subtab lists and do not have dependencies on other fields, and custom fields that are stored and do not have sourcing relationships.
        
        ![Mass Update Fields subtab on the Mass Update page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/mass1.png)
        
        Important:
        
        For transactions updates, fields that are not displayed on your preferred form for a transaction are not made available for mass updates. For example, if your preferred invoice form does not include the To Be Printed field, this field is not listed on the **Mass Update Fields** subtab for a mass update to invoices.
        
    -   If you are performing a specific type of update, such as Contact Management:
        
        To the right of the **Title of Action** field, select or enter the new data.
        
        On the **Criteria** subtab, select filters that you want to use to set criteria. When you select a filter, a window pops up where you can select criteria.
        
    
    ![Criteria subtab on the Mass Update page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/massupdate2.png)
5.  Define a filter or filters on the **Criteria** subtab.
    
    -   Select a field or formula in the dropdown list and enter values in the popup window that appears.
        
    -   For information, see [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html).
        
6.  Define display options for mass update results on the **Results** subtab.
    
    -   Select the order in which you want the results to sort.
        
    -   Choose to view the list as a report.
        
    -   Pick which columns you want to appear in the list.
        
    -   For information, see [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html).
        
7.  You can select internal and external roles as follows:
    
    Note:
    
    If the Public box is checked, the **Internal Roles** and **External Roles** fields are greyed out, the update is available to all roles and the selection cannot be edited. To select specific internal and external roles, you must clear the **Public** box first.
    
    -   **Internal Roles** - In the Internal Roles field, do one of the following:
        
        -   Check the **Select All** box next to Internal Roles to make the update available to all internal roles.
            
        -   Clear the **Select All** box and then select from the desired internal roles from the list.
            
    -   **External Roles** - To make the update available to specific external roles, select them from the list.
        
8.  If you are an administrator and you want to run the mass update on a recurring basis, set up this recurrence on the **Schedule** subtab. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html).
    
9.  Click Preview to see which records the mass update will change, and review the Mass Update Preview page.
    
    -   To modify the mass update, click Return to Criteria, and repeat steps 4-8 as necessary.
        
    -   If your list has less than 1000 entries, an **Apply** column is shown. (If you want to show the **Apply** column, select search criteria that return results with less than 1000 entries.) If any record listed should not be updated, clear the box in the **Apply** column.
        
10.  Choose one of the following options:
     
     -   Click **Perform Update** to make the mass update.
         
         Warning:
         
         After you click **Perform Update**, you cannot stop or cancel the mass update.
         
     -   Click **Save** to save this mass update for future use.
         
         -   When you save the update, it is not run. To make the mass update changes, go to _Lists > Mass Update > Saved Mass Updates_, and click Preview next to the name of the update. On the Mass Update Preview page, click Perform Update to make the changes.
             
         -   When you save a mass update, you can always return to the list to make changes to the same records by going to _Lists > Mass Update > Saved Mass Updates_.
             

Note:

You can update more than one field on records, by using the links under the General Updates heading on the Mass Updates list. Use the links under the Sales Force Automation, Contact Management, Activities, Files, Group Records, Customer Support and Service and Marketing headings to quickly create more specific updates that only affect one field.

### Related Topics

-   [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html)
-   [Entering Formulas for a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668091.html)
-   [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html)
-   [Translations for Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668849.html)
-   [Example Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669099.html)
-   [Available Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N669340.html)
-   [Mass Updates of Global Subscription Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N672926.html)
-   [Performing Mass Deletes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098351672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

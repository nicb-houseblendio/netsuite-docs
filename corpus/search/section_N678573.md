---
id: "section_N678573"
type: "section"
title: "Highlighting Search Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Defining a Saved Search > Highlighting Search Results"
parent: "section_N676039"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html"
anchors: ["bridgehead_N678703", "bridgehead_N678976", "bridgehead_4121652097", "bridgehead_N678993", "bridgehead_160987057592"]
sha256: "413053b3a1415d8d8840a792eaf2ea4484f93ace7a176a0be1867f28b24c0eff"
---

Saved searches let you highlighting rows to draw attention to selected results. You can highlight individual rows that meet certain conditions, or highlight grouped results like counts, sums, or averages.

Available highlighting options include:

-   Images
    
-   Text colors
    
-   Background colors
    
-   Bold text
    
-   Description for a highlighting legend in the results page.
    

For information about highlighting search results, see:

-   [To apply highlighting to search results:](#bridgehead_N678703)
    
-   [Conditions for Highlighting](#bridgehead_N678976)
    
-   [Summary Highlighting](#bridgehead_N678993)
    
-   [Adding a Legend to Highlighted Search Results](#bridgehead_160987057592)
    

#### To apply highlighting to search results: {#bridgehead_N678703}

1.  On the saved search page, click the **Highlighting** subtab.
    
2.  On the **Highlight If** or **Highlight If (Summary)** subtab, click the Set Options icon next to the **Condition** field to open a popup window.
    
    -   To use expressions in the condition filters, check the **Use Expressions** box. For information, see [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html).
        
    -   For summary results, choose from the **Summary Type** dropdown list. This selection must match the summary type you set on the **Results** subtab.
        
3.  In the popup, select a field or a formula to use as the filter for highlighting.
    
    -   To filter using a field from the selected record type:
        
        -   Select the field from the **Filter** dropdown list.
            
        -   Click **Set Options** to open a popup where you can enter a value and search logic (if available) for the filter.
            
    -   To use a formula as a filter:
        
        -   Select a **Formula** option from the Filter dropdown list.
            
        -   Click **Set Options** to open a popup where you can enter the formula.
            
        -   For more information about search formulas, see [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html).
            
    -   To use a join field from a related record type as a filter:
        
        -   Select the related record type in the **Filter** dropdown list.
            
        -   In the popup, select the join field from the **Filter** dropdown list.
            
        -   In the next popup, enter a value and search logic (if available) for the filter.
            
        -   For a list of related record types with join fields available for each record type search, see [Related Records Fields Available for Advanced Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N651952.html).
            
4.  Repeat step 3 for each filter you need. When you have added all filters, click the **Set** button in the popup.
    
5.  To use an image for highlighting results, select one from the **Image** dropdown list, or click the icon next to it to choose from the Icon Picker popup.
    
6.  To change the text color of results that meet the condition, click the Select Color icon in the **Text Color** column.
    
7.  To change the background color of results that meet the condition, click the Select Color icon in the **Background Color** column.
    
8.  To bold text for results that meet the condition, check the **Bold** box.
    
9.  To add a legend to the footer, enter a description for this highlight condition. For more information about legends, see [Adding a Legend to Highlighted Search Results](#bridgehead_160987057592).
    
10.  Click **Add**.
     
11.  Repeat steps 2-10 for each highlighting condition you need.
     
12.  Click **Save**.
     

## Conditions for Highlighting {#bridgehead_N678976}

You select the result rows to highlight by setting conditions on the Highlighting subtab of a saved search. You can add multiple conditions for each saved search, each with its own highlighting options. A condition has one or more filters. If a result matches any of them, it is highlighted using the options you set.

For example, you could highlight all customers in San Francisco with a balance greater than $5000 in green, and customers in San Diego with a balance over $5000 in blue.

A row can match more than one highlight condition. If that happens, what you see depends on the order. The first condition has the highest priority, and if it doesn't use all highlight options (Image, Text color, Background color, Bold) the next matching condition fills in the rest. If there are multiple conditions, the search results will be highlighted using the order of the conditions. For example, if a search result is a row with the following values.

| **Name** | **Email** |
| --- | --- |
| Adam | No@example.com |

For this example, the user sets up conditions in this order:

1.  Name starts with 'X', Background Color is 'Black', Bold is 'None', Text Color is 'White', and Image is 'None'.
    
2.  Name starts with 'A', Background Color is 'Green', Bold is 'None', Text Color is 'None', and Image is 'None'.
    
3.  Email starts with 'N', Background Color is 'Red', Bold is 'Y', Text Color is 'None', and Image is 'None'.
    

The first condition doesn't match, but the second one does, so the background is green. The third condition also matches (Email starts with N), so the row would be red. However, the criteria in the second condition takes priority. The 'Bold is Y' part of the third condition is a match, so it adds bold text.

## Highlighting Using Greater Than or Magnitude Greater {#bridgehead_4121652097}

**Greater Than** highlights one period only, whereas **Magnitude Greater Than** highlights both periods compared. For example, if you compare sales for this period to last period and you use **Magnitude Greater Than** as follows:

Highlight if = Magnitude Greater Than | Threshold = 'amount' | Period = All | Background Color = 'color'.

The result for both periods are highlighted. But if you use **Greater Than**, in this example it will highlight the results for 'This Period'.

## Summary Highlighting {#bridgehead_N678993}

If you've defined a summary type for a field, you can highlight grouped results for it in the **Highlight if... (Summary)** sublist in the **Highlighting** subtab. Available summary types include count, sum, minimum, maximum, and average.

For example, you can highlight customers with total sales over $100,000 in red if you use a summary type of Sum for the **Net Amount** field for a saved sales transactions search.

## Adding a Legend to Highlighted Search Results {#bridgehead_160987057592}

You can add a legend to highlighted results to make them easier to read.

#### To add a legend to highlighted search results:

1.  On the saved search page, click the **Highlighting** subtab.
    
2.  For each condition, add a description in the **Description** field.
    
    For example, if you highlight customers with the 504 area code in yellow, use '504 area code' as your description.
    
3.  When you've entered the description, click **Done**.
    
4.  Click **Save**.
    

### Related Topics

-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html)
-   [Defining Audiences for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678294.html)
-   [Marking a Search Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098463669.html)
-   [Editing or Deleting a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679137.html)
-   [Using a Saved Search as a View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679407.html)
-   [Defining a Saved Search as Preferred Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679861.html)
-   [Defining a Saved Search as a Preferred Search Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680007.html)
-   [Using a Saved Search as a Reminder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680807.html)
-   [Using Saved Searches for Customer Center Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3842991795.html)
-   [Change of Sign for Expense Account Amounts in Transaction Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891485192.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

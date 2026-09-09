---
id: "section_N637092"
type: "section"
title: "Tips for Effective Global Searches"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Global Search > Tips for Effective Global Searches"
parent: "article_8124535945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637092.html"
anchors: []
sha256: "1a3606d63778ec5eb6593c5d8a8a359a6c0080769c0b1149232e94a81cb2aa1f"
---

To increase the effectiveness of global search, try these tips:

-   **Use search prefixes.** Add a prefix to your search to focus on one record type, speed the search, and skip irrelevant results. A search prefix uses some or all letters of a record type, plus a colon or a caret.
    
    -   Enter **cu:max** or **cu^max** to search for customers with records containing the letters max.
        
        Note:
        
        Enable the **Global Search Customer Prefix Includes Leads and Prospect** option to include also leads and prospects, together with customers, when you use the **cu:** prefix. You can do this at _Home > Set Preferences_ on the **Analytics** subtab.
        
    -   Note that the colon (:) and caret (^) are special characters that separate the type from your keywords in global search.
        
        -   If you enter characters that end with a colon or caret, you receive an error requesting keywords. Avoid this problem by leaving off the colon or caret.
            
        -   If you enter a hierarchical entity name such as **1000P:100SUB** (where 1000P is a customer and 100SUB is a subcustomer), the text before the colon is treated as a type, so you don't get any results. To fix this, add a space before the colon. For example, enter **1000P :100SUB**. You can still add a type if you need, for example, enter **cu:1000P :100SUB**.
            
    
    For more information, see [Global Search Prefixes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639669.html).
    
-   **Use keywords with at least 3 characters.** More specific keywords are better, especially if you're searching through a large amount of data. Short or common keywords may not give you the results you want.
    
-   **Search for multiple text strings at the same time.** Use OR between keywords to search for more than one text string.
    
    -   Enter **max OR macs OR machs** to search for records containing any of these three strings in one search.
        
    -   Ensure that OR is uppercase so that it works as a separator.
        
    
    You can also use a space or a hyphen instead of OR. If a string has spaces, each word is treated as a keyword, and results return exact matches for each one of them.
    
-   **Include inactive records.** Add a **+** to your keywords to include inactive records. For example, **cu:max+** finds both active and inactive customers with "max" in their records.
    
    To always include inactive records, go to _Home > Set Preferences_, click the **Analytics** subtab, and check the **Include Inactives in Global and Quick Search** box.
    
-   **Go directly to a customer dashboard.** Use the dash: prefix with a customer name to open that customer's dashboard. For example, enter **dash:Acme Supply**, then press Enter or click Go to open that dashboard.
    
-   **Use % as a wildcard in numeric keywords.** By default, global search only returns exact matches for numbers unless you add %. Do this to avoid getting large result sets for numeric keywords.
    
    -   If you enter **inv:115**, you only get invoice #115.
        
    -   If you enter **inv:115%**, you get all invoices with numbers starting with 115.
        
    -   If you enter **inv:%115**, you get any invoice with 115 anywhere in the invoice.
        
-   Use the SQL % wildcard to select columns that begin with certain characters. For example, to see customers in Minneapolis and Minnetonka, use the SQL % wildcard to get all cities starting with 'Minn':
    
                  `SELECT * FROM Customers WHERE City LIKE 'Minn%';` 
                
    
-   Use the SQL % wildcard to select columns that contain certain characters. For example, to see Customers in Dulles and Los Angeles, use the SQL % wildcard to get all cities containing 'es':
    
                  `SELECT * FROM Customers WHERE City LIKE '%es%';` 
                
    
-   Use the SQL \_ wildcard to find all customers with a city starting with any character, followed by "erlin":
    
                  `SELECT * FROM Customers WHERE City LIKE '_erlin';` 
                
    
-   **Keep keyword length to 32 characters or less.** Longer keywords may not return results.
    
-   **Search for exact text matches only.** Enclose the search string in quotation marks, or add a backslash, to search for records containing only exact matches. For example, **cu:"max'** or **cu:max\\** only find customers named Max, not Maxam, Lomax, or Maximum Tires.
    
    You don't need quotation marks or backslashes for numbers, these searches return only exact matches.
    
-   **Search for exact record type matches only.** Use the full record type name as a prefix and enclose it in quotation marks.
    
    This is helpful if you have custom record types with similar names, for example Customer Survey. Using the 'customer' prefix returns only customer records, not customer survey records. Without the quotation marks, you get both.
    
-   **Return a single result in edit mode.** By default, a single global search result opens in view mode. You can override this by capitalizing the first letter of a search prefix. (This prefix has no effect when the Show List When Only One Result preference is enabled.)
    
    -   Enter **Cu:'Maximum Tires'** to open this customer's record in edit mode.
        
    -   Enter **In:115** to open invoice #115 in edit mode.
        
        Note:
        
        You can open a suggested record in edit mode by clicking **Edit** on the right when your hover over it in the list.
        
-   **Return search results in a new browser window.** To open search results in a new browser window, add an extra colon between the prefix and the search string. This works for both list pages and single records, in view or edit mode.
    
    -   Enter **in::115%** to open a new window with all invoices starting with 115.
        
    -   Enter **In::115** to open invoice #115 in a new window in edit mode.
        
-   **Index custom fields to be included in global search.** You can search for custom fields as well as name/ID fields. See [Including Custom Fields in Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html).
    
-   **Edit fields directly on the global search results page.** You can quickly edit records without having to change the page. See [Inline Editing of Global Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N641270.html).
    
-   **Email a list of global search results.** To email search results, click the Email button at the bottom of the results list page. A popup window opens, and you can select recipients, add comments, and choose a format.
    

For more information, see the following topics:

-   [Global Search by Email Address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637807.html)
    
-   [Global Search by IP Address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639465.html)
    
-   [Global Search by Document Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554367380.html)
    

### Related Topics

-   [Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8124535945.html)
-   [Global Search Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161899349589.html)
-   [How to Use Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0713121656.html)
-   [Global Search Prefixes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639669.html)
-   [Including Custom Fields in Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html)
-   [Inline Editing of Global Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N641270.html)
-   [User Preferences for Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642323.html)
-   [Notes about Global Search Auto Suggest](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642700.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N639669"
type: "section"
title: "Global Search Prefixes"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Global Search > Global Search Prefixes"
parent: "article_8124535945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639669.html"
anchors: ["bridgehead_N639921", "bridgehead_4615925459"]
sha256: "1f188a05738b52317ab7b741df088d3528482f0c24c2e9ce7a9b84093a9d02ee"
---

You can use record type prefixes in global search to narrow results to one record type. A search prefix uses some or all letters of a record type name, plus a colon or caret. For example:

-   **cu:** or **cu^** for customer searches.
    
-   **em:** or **em^** for employee searches.
    
-   **bu:** or **bu^** for budget searches.
    

Important:

The prefixes that work for you may be different from the prefixes listed on this page. Your account administrator may have renamed some records, or you may have set a different language at _Home > Set Preferences_.

The system uses starts-with matching for prefixes, so you get results for record types that start with or contain those letters.

For example, to search for an inventory item, you can use any of the following prefixes:

-   **i:**
    
-   **it:**
    
-   **inv:**
    
-   **inve:**
    

Some of these prefixes may return extra results if they match more than one record type. For example, **inv:** can return results for both inventory items and invoices.

For more details, see [Examples of Global Search Prefixes](#bridgehead_N639921).

For example, to search for results with a record type of plain text file, you could use any of the following prefixes:

-   **p:**
    
-   **pl:**
    
-   **t:**
    
-   **te:**
    
-   **fi:**
    
-   **fil:**
    

However, some of these prefixes may return results for more than one record type, because they may not be unique. For example, **p:** could return record types of plain text file, phone call, promotion code, partner, page, and others.

Note:

The colon and caret are special characters that separate the record type from your keywords. If you end with a colon or caret, you get an error asking for the keywords.

You can use a full record type name as a prefix and enclose it in quotation marks to search for records that type only. This is helpful if you have custom record types with similar names, for example Customer Survey. Using the "customer" prefix in quotation marks returns only customer records, not customer survey records. Without the quotation marks, you get both record types.

By default, the **cu:** prefix returns records only for customers, not for leads or prospects. Enable the **Global Search Customer Prefix Includes Leads and Prospect** option to include also leads and prospects, together with customers, when you use the **cu:** prefix. You can do this at _Home > Set Preferences_ on the **Analytics** subtab.

Note:

Use the **dash:** prefix with a customer name to go directly to their dashboard.

## Examples of Global Search Prefixes {#bridgehead_N639921}

Important:

The following examples use English (U.S.) and default record names. Your prefixes may be different.

You don't need to select a prefix from this list, use the first few letters of the record type name as a prefix. Keep the prefix unique so it doesn't match other types.

| Prefix | Record Type |
| --- | --- |
| **cam** | Campaign |
| **cash** | Cash Sale |
| **con** | Contact |
| **cust** | Customer |
| **emp** | Employee |
| **est** | Estimate |
| **ev** | Event |
| **exp** | Expense Report |
| **fi** | File |
| **invo** | Invoice |
| **iss** | Issue |
| **it** | Item |
| **opp** | Opportunity |
| **par** | Partner |
| **ph** | Phone Call |
| **sales** | Sales Order |

## Using Global Search to Find Help Topics {#bridgehead_4615925459}

The NetSuite Help Center has its own search, but you can also use global search to search for a help topic directly from any NetSuite page.

To search the Help Center, use the **help:** prefix in the Search field in the upper right corner. For example, enter **help:dashboards** to find help topics about dashboards.

### Related Topics

-   [Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8124535945.html)
-   [Global Search Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161899349589.html)
-   [How to Use Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0713121656.html)
-   [Tips for Effective Global Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637092.html)
-   [Including Custom Fields in Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html)
-   [Inline Editing of Global Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N641270.html)
-   [User Preferences for Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642323.html)
-   [Notes about Global Search Auto Suggest](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642700.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

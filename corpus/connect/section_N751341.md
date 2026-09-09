---
id: "section_N751341"
type: "section"
title: "Custom Columns, Lists, and Records in the Connect Service"
branch: "connect"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Connect > Connect Service Considerations > Custom Columns, Lists, and Records in the Connect Service"
parent: "chapter_N751003"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N751341.html"
anchors: ["subsect_163595580414", "bridgehead_4781145588", "bridgehead_164249008644", "subsect_163595584583"]
sha256: "298bb78cd85080704b60035713953e746327332736d9140af126bfea7261e810"
---

Important:

Support ends for the NetSuite.com data source in 2025.1, and it will be removed in 2026.1. Start transitioning to the NetSuite2.com as soon as possible to avoid disruption when this change occurs.

To work with the Connect Service and custom records, see the following examples and considerations:

-   [General Considerations for Connect](#subsect_163595580414)
    
-   _Considerations for NetSuite.com_
    
-   [Considerations for NetSuite2.com](#subsect_163595584583)
    

## General Considerations for Connect {#subsect_163595580414}

The following considerations apply to both data sources:

-   [Custom Field Limitations](#bridgehead_4781145588)
    
-   [Newly Created Custom Records](#bridgehead_164249008644)
    

## Custom Field Limitations {#bridgehead_4781145588}

Due to an internal limitation, queries over SuiteAnalytics Connect that have more than 1000 columns only work if you retrieve 1000 columns or less in the query. For example, if the Transactions table has more than 1000 columns due to the number of custom fields that have been added to the Transaction record type, attempting to query the table using the 'Select \* From' construct results in the following error: 'Error: Could not find any column information for table:transactions'.

You may also see this error when joining multiple tables and trying to retrieve all fields.

To query over a table with more than 1000 columns, you must enumerate the specific columns that you want to retrieve or, if you have to use the 'Select \* From' construct, you must deactivate some of the custom fields that have been added to the table so that there are 1000 columns or less.

## Newly Created Custom Records {#bridgehead_164249008644}

If you are using Connect and at the same time you create a new custom table or column using the same account, the newly custom record is not considered yet in your queries. After you created the custom table or column, you need to log out and open a new Connect session.

## Considerations for NetSuite2.com {#subsect_163595584583}

For details about general considerations for NetSuite2.com, see the following:

-   [Querying Data with Connect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159006290517.html)
    
-   [SuiteQL Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3903316302.html#subsect_163595191063)
    
-   [Record Types and Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164312261929.html)
    

### Related Topics

-   [Connect Service Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N751003.html)
-   [Query Language Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3903316302.html)
-   [Connections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4153627846.html)
-   [Exceptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4153646644.html)
-   _Column Joins in the Connect Service_
    
-   [Driver Access for a Sandbox or Release Preview Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3963862712.html)
-   [Operating System Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0801115551.html)
-   [Third-Party Application Access](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3963861118.html)
-   [Server Restarts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162071870533.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

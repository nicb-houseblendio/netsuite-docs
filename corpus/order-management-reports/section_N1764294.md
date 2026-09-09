---
id: "section_N1764294"
type: "section"
title: "Using Gross Profit Values in CSV Import, SOAP Web Services, and SuiteScript"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Using Gross Profit Fields > Using Gross Profit Values in CSV Import, SOAP Web Services, and SuiteScript"
parent: "section_N1762134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html"
anchors: ["bridgehead_N1764363", "bridgehead_N1764500", "bridgehead_N1764562"]
sha256: "cba9a61cf2ea7c2f2dfdd6e93bdcaa04f062de918b3605382165bf252580e838"
---

After the Gross Profit feature has been enabled, gross profit fields are available for CSV Import, SOAP web services, and SuiteScript. For details, see:

-   [Gross Profit Fields in CSV Import](#bridgehead_N1764363)
    
-   [Gross Profit Fields in SOAP Web Services](#bridgehead_N1764500)
    
-   [Gross Profit Fields in SuiteScript](#bridgehead_N1764562)
    

## Gross Profit Fields in CSV Import {#bridgehead_N1764363}

CSV Import supports the following transaction types that may include gross profit fields: Cash Sale, Estimate, Invoice, Opportunity, and Sales Order. For each type of transaction, the Import Assistant's Field Mapping page lists the NetSuite fields that can be mapped to columns in your CSV file. You can import data for any field listed on this page.

By default, the Field Mapping page includes the NetSuite fields available on your preferred form for the record type. Fields can be mapped for the import job if they are displayed (not hidden) and not disabled on your preferred form. So if gross profit fields are shown on your preferred form for a transaction type, their data can be imported.

The default form for your role may not include all the fields you need to import, so you have the option of specifying another form to provide mappable fields. For record types that allow custom forms, you can specify an existing custom form available to your role, or you can create a custom form specifically for this purpose.

For more information, see:

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
    
-   [Cash Sale Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N407231.html)
    
-   [Estimate Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411251.html)
    
-   [Invoice Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411794.html)
    
-   [Opportunity Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N421452.html)
    
-   [Sales Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N426302.html)
    

## Gross Profit Fields in SOAP Web Services {#bridgehead_N1764500}

SOAP web services support gross profit fields for applicable transaction types.

[SOAP Schema Browser](https://www.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/account.html) details available fields for each supported record type.

-   See **transactions sales.xsd** for the Cash Sale, Estimate, Invoice, Opportunity, and Sales Order transaction types.
    
-   See **transactions customers.xsd** for the Cash Refund, Credit Memo, and Return Authorization transaction types.
    

For more information about SOAP web services, see [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html).

## Gross Profit Fields in SuiteScript {#bridgehead_N1764562}

SuiteScript is supported for a subset of gross profit fields on the following transaction types: Cash Refund, Cash Sale, Estimate, Invoice, Opportunity, and Sales Order.

Fields are supported as follows:

| Field | Internal ID | SuiteScript Support |
| --- | --- | --- |
| Est. Gross Profit | estgrossprofit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| Est. Gross Profit Percent | estgrossprofitpercent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| Est. Extended Cost | totalcostestimate | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

For more information, see:

-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
    
-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
    

### Related Topics

-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)
-   [Using Gross Profit Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762134.html)
-   [Using Gross Profit Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html)
-   [Including Gross Profit Values in Reports, Searches, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1763752.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

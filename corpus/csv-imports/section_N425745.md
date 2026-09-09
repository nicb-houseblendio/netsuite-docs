---
id: "section_N425745"
type: "section"
title: "Return Authorization Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Return Authorization Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N425745.html"
anchors: ["bridgehead_N425847", "bridgehead_N425898", "bridgehead_N426008", "bridgehead_4314743520"]
sha256: "60d59ba9c7100dc3d3d335e109b2013ec300b2ba6b9b9f567263b85ce82167b0"
---

Return authorization records track information about items returned by customers. These records store data such as quantity and value of returned items, and return status. The return authorization record is updated at each point in the return process, including when the return is initiated, when the returned item is received, and when the refund is issued. The return process can vary based on return management preferences, enabled features, and other account-specific factors. For more information about return authorizations, see [Customer Return Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302852.html).

Note:

Return Authorization imports aren't available unless the Return Authorizations feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Transactions subtab, check the Return Authorizations box.

This import supports the import of standalone return authorizations, but not linked return authorizations (those created from cash sales or invoices and linked to these original sales transactions).

Review the following guidelines for Return Authorization imports:

-   [Setting the Form for a Return Authorization Import](#bridgehead_N425847)
    
-   [Notes on Return Authorization Import Field Values](#bridgehead_N425898)
    
-   [Supported Return Authorization Sublist Data Imports](#bridgehead_N426008)
    
-   [Supported Return Authorization Subrecord Data Imports](#bridgehead_4314743520)
    

## Setting the Form for a Return Authorization Import {#bridgehead_N425847}

By default, the Field Mapping page for a return authorization import displays the NetSuite fields from your preferred return authorization form. You can select a different return authorization form in the Advanced Options area of the Import Assistant's Import Options page. See [Custom Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751044597.html).

Two different categories of return authorization forms are usually available:

-   'Credit' return authorization forms that authorize the issuing of a credit memo for the returned items. The credit memo can either be applied to an account balance or refunded.
    
-   'Cash' return authorization forms that authorize a direct refund for the returned items. This type of authorization can't later be processed as a credit memo.
    

## Notes on Return Authorization Import Field Values {#bridgehead_N425898}

-   You need to map either an external ID or internal ID as a unique ID for each record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the Rtn. Auth. # field, which serves as a transaction ID for return authorization records. This way, external IDs show up on return authorization forms in NetSuite.
    
-   Each imported return authorization record should include a reference to a NetSuite customer record, mapped to the return authorization's Customer field. This reference must be a unique identifier; use internal ID or external ID, rather than a name reference. If you don't map a reference number field, reference number values are generated automatically.
    
-   Although the Status field is required, you don't have to map it to a column in your CSV file. If you don't map the Status field, it's automatically mapped with default values of the default return authorization status, as set at _Setup > Accounting > Preferences > Accounting Preferences_, on the Order Management subtab, under Returns. The default is Pending Approval if your company uses the approval process for return authorizations, and Pending Fulfillment if your company doesn't use this process.
    
-   You also don't have to map the required Date field. If you don't map the Date field, it's automatically mapped with default values of the current date.
    
-   If the Multiple Currencies feature is enabled, map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced customers. If your customers use currencies other than the currency in which your company manages its financials, map the Currency field. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    

For more details about fields that can be mapped in the return authorization record, see the SOAP Schema Browser's [return authorization](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/returnauthorization.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Supported Return Authorization Sublist Data Imports {#bridgehead_N426008}

The Return Authorization import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | Selectively updatable based on Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Partner key field. |
| Sales Team | When Team Selling feature enabled. Selectively updatable based on Employee key field. |

For imports that update existing Return Authorization records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Supported Return Authorization Subrecord Data Imports {#bridgehead_4314743520}

The Return Authorization import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Billing Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Items - Inventory Detail | When Advanced Bin/Numbered Inventory Management feature enabled. |
| Shipping Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

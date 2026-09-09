---
id: "bridgehead_N276747"
type: "bridgehead"
title: "Assigning Subsidiaries to a Customer"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Associate Subsidiaries with Entities and Items > Assigning Subsidiaries to a Customer"
parent: "section_N276477"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html"
anchors: []
sha256: "57072d623a8bee7de3a48f752cce3f3b87b60d2241a3677fcc9b2320d7999589"
---

The Multi-Subsidiary Customer feature lets you share customer and sub-customer records with multiple subsidiaries, and then select those subsidiaries on core transactions. The primary subsidiary assigned to a customer is generally associated with any transactions involving that customer. However, you can also associate transactions with any secondary subsidiary assigned to the customer. The subsidiary you select on transactions persists throughout the transaction workflow. For example, when you select a subsidiary on a sales order, that subsidiary appears on the invoice. For detailed instructions about assigning subsidiaries to a customer record, [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).

The Multi-Subsidiary Customer feature enables you to save a multi-subsidiary customer as a multi-subsidiary vendor to create a single entity. It is useful when you want to have one entity represent both a customer and a vendor. You can also view a multi-subsidiary customer's hierarchy (primary subsidiary, any assigned secondary subsidiary, and any subcustomer).

Note:

In the customer hierarchy, users can view only those subsidiaries to which they are granted access.

The Multi-Subsidiary Customer feature also enables you to view the following:

-   Customer balance information on the customer record
    
-   Secondary subsidiary information on core reports
    
-   Customer Statement by currency and by subsidiary
    

When a lead or contact is generated from an online form, the country associated with the form is matched to the country of the subsidiary. Then, that subsidiary is associated with the new record. If multiple subsidiaries are related to a country or no country is entered, the root subsidiary is the primary subsidiary with the new entity.

Note:

If you use the Accept Payment Through Top Level Customer preference, note the following. Parent customers and their sub-customers must be associated with the same subsidiaries, and both must use the same currencies.

Important:

You can define multiple secondary subsidiaries though the user interface and SuiteScript. To define secondary subsidiaries in SuiteScript, use the [Customer-Subsidiary Relationship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1507907354.html) record type. To mass create and update customer records through CSV files, see [Customer-Subsidiary Relationship Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529503002.html).

If you shared multiple subsidiaries with a vendor record, you can share a customer record that is also paired with a vendor record. Such pairings display on the Relationships subtab on the customer record.

To use the subsidiary logo and address from the transaction record when printing, use advanced templates. For more information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html). If you print transactions using basic layouts, the logo and address are sourced from the customer's primary subsidiary.

### Additional Information

-   [Merging Customer Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509542900.html)

### Related Topics

-   [Multi-Subsidiary Customer Feature Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509460470.html)
-   [Best Practices for Using the Multi-Subsidiary Customer Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509372257.html)
-   [Enable the Multi-Subsidiary Customer Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509460991.html)
-   [Customer Balances for Assigned Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509462110.html)
-   [Customer Searches for Multi-Subsidiary Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509462401.html)
-   [Mass Create and Update Multi-Subsidiary Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1528201145.html)
-   [Customization of the Subsidiaries Subtab on the Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1528201575.html)
-   [Multi-Subsidiary Customer Support for Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1555423774.html)
-   [Multi-Subsidiary Customer Vendor Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509462960.html)
-   [Multi-Subsidiary Customer Hierarchy](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509463883.html)
-   [Transactions Available for Multi-Subsidiary Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509464317.html)
-   [Assigning a Subsidiary to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276604.html)
-   [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html)
-   [Assigning a Subsidiary to a Partner](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276702.html)
-   [Associate Subsidiaries With Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276948.html)
-   [Associate Subsidiaries With Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N277674.html)
-   [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

---
id: "section_N394436"
type: "section"
title: "Understanding Leads, Prospects, and Customers"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Understanding Leads, Prospects, and Customers"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html"
anchors: []
sha256: "1ae3d2cdcc97944f077ada7023152d70cfd49f05ccf3fb9d30e64596f2a24342"
---

When you import Lead, Prospect, or Customer data into NetSuite, you import into the Customer record. The Stage field on the Customer record defines the stage of 'Customer' that is currently in the system - a Customer can be a Lead, Prospect, or Customer. Leads can automatically become Prospects, and Prospects can become Customers.

Following are specific definitions of the three record types:

-   **Lead** : lets you track all the information you need to convert a lead into a customer. Leads have no estimates, opportunities or transactions associated with them. If an estimate or opportunity is created for a lead, the lead becomes a prospect. If you create a sales transaction for a lead, the lead becomes a customer.
    
-   **Prospect** : lets you track all the information you need to convert a prospect into a customer. Prospects have no sales orders, invoices, cash sales or other sales transactions associated with them. They can have opportunities and estimates associated with them, however. If a sales transaction is created for a prospect, or an opportunity is closed for a prospect, the prospect becomes a customer.
    
-   **Customer** : lets you track all the information about your current customers.
    

For details about fields that can be mapped in the customer record, see the SOAP Schema Browser's [customer](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customer.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

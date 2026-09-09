---
id: "section_N1179020"
type: "section"
title: "Basic Projects Overview"
branch: "basic-projects"
category: "projects"
breadcrumb: "Projects > Basic Projects > Basic Projects Overview"
parent: "chapter_N1178959"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179020.html"
anchors: []
sha256: "a2e4cb1019259b03635c072543983d818aff301cdaa3a36664ae11b562caaafb"
---

Use the Projects feature to track information about projects you are working on for customers, including time, contacts, and transactions.

On the project record, you can track time associated with the project. You can also create transactions associated with the project, and add CRM information such as activities and communication.

To create a project record with Projects, go to Lists > Customers and click View next to the customer the project is for. When the customer record opens, click Project in the Create New menu. For detailed instructions, see [Creating a Basic Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179164.html).

You can also import basic projects using CSV import. For more information, see [Projects (Jobs) Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N385885.html).

After you've entered project records, you can associate a project with a transaction by selecting the project in the Project field on the transaction form or by creating a new transaction directly from the project record from the Create New menu.

Note:

Auto-generated numbering creates a single sequence for all projects.

If you use the basic Projects feature (Project Management and Advanced Project Tracking are not enabled), be aware of how the system determines the tax code to apply to an invoice for a project.

Prior to NetSuite Version 2015 Release 2, when a project is selected on an invoice, the tax code is determined by the following:

-   The tax schedule on the item
    
-   The shipping address of the project or customer, depending on which is available first in the hierarchy
    

As of NetSuite Version 2015 Release 2:

-   If the customer to which the project belongs has a default tax code on its record, the system uses that tax code for the invoice.
    
-   If the customer to which the project belongs doesn't have a default tax code on its record, the tax code is determined by the tax schedule on the item and on the shipping address of the project or customer.
    

Note:

The NetSuite tax lookup based on shipping address varies depending on the country.

### Related Topics:

-   [Basic Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1178959.html)
-   [Creating a Basic Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179164.html)
-   [Additional Basic Project Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588475450.html)
-   [Attach Contacts to Basic Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1179740.html)
-   [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
